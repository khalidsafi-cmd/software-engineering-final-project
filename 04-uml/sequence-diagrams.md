# Sequence Diagrams

Status: models of inspected existing code, not observed runtime results. Routes, Form Requests, controllers, Action classes and Eloquent persistence determine these flows. Vue/Inertia submits requests and receives redirect-driven updated page props. Rejection paths stop writes; no realtime transport is claimed.

## Customer posts a job

```mermaid
sequenceDiagram
    actor User as User/Browser
    participant UI as Vue/Inertia frontend
    participant Controller as Laravel CustomerJobController
    participant Action as CreateJob
    participant DB as Database
    User->>UI: Submit workflow form
    UI->>Controller: POST /jobs
    Controller->>Controller: Validate StoreJobRequest and active customer
    alt Authorized and valid
        Controller->>Action: handle(user, validated input / bound models)
        Action->>Action: Authorize create#59; persist owned open job
        Action->>DB: INSERT jobs#59; authenticated customer_id
        DB-->>Action: Persisted state
        Action-->>Controller: Success / transaction commit
        Controller-->>UI: Redirect to My Jobs
        UI-->>User: Updated page / feedback
    else Invalid or unauthorized
        Controller-->>UI: Validation errors / forbidden response
        UI-->>User: Error feedback#59; no successful write
    end
```

Action-level state or authorization failures also abort/roll back and return an error. Evidence: [CustomerJobController](../../app/Http/Controllers/CustomerJobController.php), [CreateJob](../../app/Actions/CreateJob.php).

## Worker applies for a job

```mermaid
sequenceDiagram
    actor User as User/Browser
    participant UI as Vue/Inertia frontend
    participant Controller as Laravel JobApplicationController
    participant Action as ApplyToJob
    participant DB as Database
    User->>UI: Submit workflow form
    UI->>Controller: POST /jobs/{job}/applications
    Controller->>Controller: Validate StoreApplicationRequest and active worker
    alt Authorized and valid
        Controller->>Action: handle(user, validated input / bound models)
        Action->>Action: Transaction#59; lock job#59; authorize#59; reject duplicate
        Action->>DB: INSERT pending application
        DB-->>Action: Persisted state
        Action-->>Controller: Success / transaction commit
        Controller-->>UI: Redirect to job detail
        UI-->>User: Updated page / feedback
    else Invalid or unauthorized
        Controller-->>UI: Validation errors / forbidden response
        UI-->>User: Error feedback#59; no successful write
    end
```

Action-level state or authorization failures also abort/roll back and return an error. Evidence: [JobApplicationController](../../app/Http/Controllers/JobApplicationController.php), [ApplyToJob](../../app/Actions/ApplyToJob.php).

## Customer selects a worker

```mermaid
sequenceDiagram
    actor User as User/Browser
    participant UI as Vue/Inertia frontend
    participant Controller as Laravel JobApplicationController
    participant Action as AcceptApplication
    participant DB as Database
    User->>UI: Submit workflow form
    UI->>Controller: POST /my-jobs/{job}/applications/{application}/accept
    Controller->>Controller: Scoped job/application binding#59; active customer
    alt Authorized and valid
        Controller->>Action: handle(user, validated input / bound models)
        Action->>Action: Transaction#59; authorize owner#59; check pending eligible worker
        Action->>DB: Accept selected#59; reject other pending#59; assign job
        DB-->>Action: Persisted state
        Action->>Action: EnsureJobConversation (within transaction)
        Action->>DB: First-or-create selected job conversation
        Action-->>Controller: Success / transaction commit
        Controller-->>UI: Redirect to applicants
        UI-->>User: Updated page / feedback
    else Invalid or unauthorized
        Controller-->>UI: Validation errors / forbidden response
        UI-->>User: Error feedback#59; no successful write
    end
```

Action-level state or authorization failures also abort/roll back and return an error. Evidence: [JobApplicationController](../../app/Http/Controllers/JobApplicationController.php), [AcceptApplication](../../app/Actions/AcceptApplication.php).

## Customer and worker send messages

```mermaid
sequenceDiagram
    actor User as User/Browser
    participant UI as Vue/Inertia frontend
    participant Controller as Laravel ConversationController
    participant Action as SendMessage
    participant DB as Database
    User->>UI: Submit workflow form
    UI->>Controller: POST /messages/{conversation}
    Controller->>Controller: Validate StoreMessageRequest#59; auth/active#59; throttle
    alt Authorized and valid
        Controller->>Action: handle(user, validated input / bound models)
        Action->>Action: Lock participants#59; authorize participant and block/status checks
        Action->>DB: INSERT message#59; touch conversation
        DB-->>Action: Persisted state
        Action-->>Controller: Success / transaction commit
        Controller-->>UI: Redirect to conversation
        UI-->>User: Updated page / feedback
    else Invalid or unauthorized
        Controller-->>UI: Validation errors / forbidden response
        UI-->>User: Error feedback#59; no successful write
    end
```

Action-level state or authorization failures also abort/roll back and return an error. Evidence: [ConversationController](../../app/Http/Controllers/ConversationController.php), [SendMessage](../../app/Actions/SendMessage.php).

## Customer completes job and participant reviews

```mermaid
sequenceDiagram
    actor User as Customer / Browser
    participant UI as Vue/Inertia frontend
    participant CompleteController as Laravel JobCompletionController
    participant CompleteAction as CompleteJob
    participant ReviewController as Laravel ReviewController
    participant ReviewAction as CreateReview
    participant DB as Database
    User->>UI: Mark assigned job completed
    UI->>CompleteController: POST /jobs/{job}/complete
    CompleteController->>CompleteAction: handle(customer, job)
    CompleteAction->>DB: Transaction#59; lock job
    CompleteAction->>CompleteAction: Authorize active owner#59; assigned and selected
    alt Completion allowed
        CompleteAction->>DB: UPDATE job status completed#59; commit
        CompleteAction-->>CompleteController: Success
        CompleteController-->>UI: Back redirect with feedback
        User->>UI: Submit counterpart rating and optional comment
        UI->>ReviewController: POST /jobs/{job}/reviews
        ReviewController->>ReviewController: StoreReviewRequest authorization and rating 1–5 validation
        ReviewController->>ReviewAction: handle(user, job, validated data)
        ReviewAction->>DB: Transaction#59; lock completed job
        ReviewAction->>ReviewAction: Authorize participant#59; reject duplicate#59; choose counterpart
        ReviewAction->>DB: INSERT review#59; commit
        ReviewAction-->>ReviewController: Review created
        ReviewController-->>UI: Back redirect with feedback
        UI-->>User: Updated review state
    else Completion denied
        CompleteAction-->>CompleteController: Authorization failure#59; rollback
        CompleteController-->>UI: Forbidden response
    end
```

The selected worker may separately review the customer after completion; the worker cannot mark the job completed. Invalid ratings, nonparticipants, premature or duplicate reviews are rejected before persistence. Sources: [CompleteJob](../../app/Actions/CompleteJob.php), [CreateReview](../../app/Actions/CreateReview.php), [StoreReviewRequest](../../app/Http/Requests/StoreReviewRequest.php). Controllers redirect; the updated Inertia page is loaded through the ensuing request.
