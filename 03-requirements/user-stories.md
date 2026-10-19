# Product Backlog User Stories

All sprint allocations and estimates are PLANNED proposals, not meeting commitments. Existing implementation is a code-inspection finding, not proof of passing tests or Product Owner acceptance. No sprint outcomes are recorded. Change work to IN PROGRESS only when actual work starts; record evidence and dates. Do not infer IN PROGRESS from a future schedule.

Exactly 20 main stories. Points estimate verification, tests, documentation and evidenced refinement during October, not original development. Product Owner must validate estimates and priorities during planning.

## US-01 — Browse and filter public jobs

As a Visitor, I want to browse and filter public jobs, so that I can find relevant open work.

- Backlog rank: 1
- Priority: Must Have
- Story Points: 3 (proposed)
- Status: IMPLEMENTED (existing code); assignment verification PLANNED
- Assigned Sprint: Sprint 01
- Acceptance Criteria: Open jobs of active customers appear; keyword/category/location filters combine; pagination retains filters; empty results and missing records are handled.
- Existing code evidence: [app/Actions/GetPublicJobs.php](../../app/Actions/GetPublicJobs.php)
- Verification: existing [test file](../../tests/Feature/PublicWebsiteTest.php) plus manual workflow demonstration. Results: TO BE UPDATED DURING SPRINT.

## US-02 — Discover workers and view public profiles

As a Visitor, I want to discover workers and view public profiles, so that I can compare skills and reputation.

- Backlog rank: 2
- Priority: Must Have
- Story Points: 3 (proposed)
- Status: IMPLEMENTED (existing code); assignment verification PLANNED
- Assigned Sprint: Sprint 01
- Acceptance Criteria: Only active worker profiles appear; filters combine; profiles expose skills and real visible-review averages without private account fields.
- Existing code evidence: [app/Actions/GetPublicWorkers.php](../../app/Actions/GetPublicWorkers.php)
- Verification: existing [test file](../../tests/Feature/PublicWebsiteTest.php) plus manual workflow demonstration. Results: TO BE UPDATED DURING SPRINT.

## US-03 — Register as a customer or worker

As a Visitor, I want to register as a customer or worker, so that I can participate with the correct role.

- Backlog rank: 3
- Priority: Must Have
- Story Points: 3 (proposed)
- Status: IMPLEMENTED (existing code); assignment verification PLANNED
- Assigned Sprint: Sprint 01
- Acceptance Criteria: Valid customer/worker registration succeeds; worker profile is created; admin/invalid role injection is rejected; duplicate identity fields are validated.
- Existing code evidence: [app/Http/Controllers/Auth/RegisteredUserController.php](../../app/Http/Controllers/Auth/RegisteredUserController.php)
- Verification: existing [test file](../../tests/Feature/ProfileAuthorizationTest.php) plus manual workflow demonstration. Results: TO BE UPDATED DURING SPRINT.

## US-04 — Log in and manage account credentials

As a Customer, I want to log in and manage account credentials, so that I can access my account securely.

- Backlog rank: 4
- Priority: Must Have
- Story Points: 3 (proposed)
- Status: IMPLEMENTED (existing code); assignment verification PLANNED
- Assigned Sprint: Sprint 01
- Acceptance Criteria: Valid login and logout work; invalid credentials fail; reset tokens and email verification are checked with their existing Auth tests; profile changes preserve protected fields.
- Existing code evidence: [app/Http/Controllers/Auth/AuthenticatedSessionController.php](../../app/Http/Controllers/Auth/AuthenticatedSessionController.php)
- Verification: existing [test file](../../tests/Feature/Auth/AuthenticationTest.php) plus manual workflow demonstration. Results: TO BE UPDATED DURING SPRINT.

## US-05 — Maintain my skills and worker profile

As a Worker/Ustaad, I want to maintain my skills and worker profile, so that I can present my services accurately.

- Backlog rank: 5
- Priority: Must Have
- Story Points: 3 (proposed)
- Status: IMPLEMENTED (existing code); assignment verification PLANNED
- Assigned Sprint: Sprint 01
- Acceptance Criteria: Own bio, experience, location, availability, trades and valid photo can be updated; invalid trades/uploads fail; other roles and suspended workers cannot edit.
- Existing code evidence: [app/Actions/UpdateWorkerProfile.php](../../app/Actions/UpdateWorkerProfile.php)
- Verification: existing [test file](../../tests/Feature/ProfileAuthorizationTest.php) plus manual workflow demonstration. Results: TO BE UPDATED DURING SPRINT.

## US-06 — Post a categorized job

As a Customer, I want to post a categorized job, so that I can request skilled help.

- Backlog rank: 6
- Priority: Must Have
- Story Points: 3 (proposed)
- Status: IMPLEMENTED (existing code); assignment verification PLANNED
- Assigned Sprint: Sprint 02
- Acceptance Criteria: Valid title/category/description/location and optional budget create an open job owned by the authenticated active customer; invalid inputs and other roles fail.
- Existing code evidence: [app/Actions/CreateJob.php](../../app/Actions/CreateJob.php)
- Verification: existing [test file](../../tests/Feature/JobMarketplaceTest.php) plus manual workflow demonstration. Results: TO BE UPDATED DURING SPRINT.

## US-07 — Edit or cancel my open job

As a Customer, I want to edit or cancel my open job, so that I can keep requests accurate.

- Backlog rank: 7
- Priority: Must Have
- Story Points: 3 (proposed)
- Status: IMPLEMENTED (existing code); assignment verification PLANNED
- Assigned Sprint: Sprint 02
- Acceptance Criteria: Only the active owner changes an open job; ownership/status injection fails; cancellation preserves application history; closed jobs cannot be edited or cancelled.
- Existing code evidence: [app/Actions/UpdateJob.php](../../app/Actions/UpdateJob.php)
- Verification: existing [test file](../../tests/Feature/JobMarketplaceTest.php) plus manual workflow demonstration. Results: TO BE UPDATED DURING SPRINT.

## US-08 — Apply to an open job

As a Worker/Ustaad, I want to apply to an open job, so that I can offer my services.

- Backlog rank: 8
- Priority: Must Have
- Story Points: 3 (proposed)
- Status: IMPLEMENTED (existing code); assignment verification PLANNED
- Assigned Sprint: Sprint 02
- Acceptance Criteria: One pending application per eligible worker/job accepts optional message and price; duplicate applications, closed jobs and ineligible accounts fail.
- Existing code evidence: [app/Actions/ApplyToJob.php](../../app/Actions/ApplyToJob.php)
- Verification: existing [test file](../../tests/Feature/JobMarketplaceTest.php) plus manual workflow demonstration. Results: TO BE UPDATED DURING SPRINT.

## US-09 — Track my applications

As a Worker/Ustaad, I want to track my applications, so that I can understand selection progress.

- Backlog rank: 9
- Priority: Should Have
- Story Points: 2 (proposed)
- Status: IMPLEMENTED (existing code); assignment verification PLANNED
- Assigned Sprint: Sprint 02
- Acceptance Criteria: My Applications shows only my records with job context and pagination; forged worker filters do not expose other workers; unauthorized roles are denied.
- Existing code evidence: [app/Http/Controllers/JobApplicationController.php](../../app/Http/Controllers/JobApplicationController.php)
- Verification: existing [test file](../../tests/Feature/JobMarketplaceTest.php) plus manual workflow demonstration. Results: TO BE UPDATED DURING SPRINT.

## US-10 — Inspect applicants and hire one worker

As a Customer, I want to inspect applicants and hire one worker, so that I can choose a suitable Ustaad.

- Backlog rank: 10
- Priority: Must Have
- Story Points: 5 (proposed)
- Status: IMPLEMENTED (existing code); assignment verification PLANNED
- Assigned Sprint: Sprint 02
- Acceptance Criteria: Only owner views applicants and accepts an eligible pending application for that job; selected status is accepted, others rejected, job assigned and conversation ensured atomically; repeat selection fails.
- Existing code evidence: [app/Actions/AcceptApplication.php](../../app/Actions/AcceptApplication.php)
- Verification: existing [test file](../../tests/Feature/JobMarketplaceTest.php) plus manual workflow demonstration. Results: TO BE UPDATED DURING SPRINT.

## US-11 — Exchange messages with my selected worker

As a Customer, I want to exchange messages with my selected worker, so that I can coordinate the job privately.

- Backlog rank: 11
- Priority: Must Have
- Story Points: 5 (proposed)
- Status: IMPLEMENTED (existing code); assignment verification PLANNED
- Assigned Sprint: Sprint 03
- Acceptance Criteria: Customer and selected worker access their job conversation; valid messages persist and read tracking updates; outsiders, blocked pairs and ineligible senders cannot send; throttling applies.
- Existing code evidence: [app/Actions/SendMessage.php](../../app/Actions/SendMessage.php)
- Verification: existing [test file](../../tests/Feature/CommunicationTest.php) plus manual workflow demonstration. Results: TO BE UPDATED DURING SPRINT.

## US-12 — Mark an assigned job completed

As a Customer, I want to mark an assigned job completed, so that I can close the work and enable feedback.

- Backlog rank: 12
- Priority: Must Have
- Story Points: 2 (proposed)
- Status: IMPLEMENTED (existing code); assignment verification PLANNED
- Assigned Sprint: Sprint 03
- Acceptance Criteria: Only the active owner completes an assigned job with an accepted application; selected worker, outsiders and other job states are denied.
- Existing code evidence: [app/Actions/CompleteJob.php](../../app/Actions/CompleteJob.php)
- Verification: existing [test file](../../tests/Feature/CompletionReviewTest.php) plus manual workflow demonstration. Results: TO BE UPDATED DURING SPRINT.

## US-13 — Review my worker after completion

As a Customer, I want to review my worker after completion, so that I can share trustworthy feedback.

- Backlog rank: 13
- Priority: Should Have
- Story Points: 3 (proposed)
- Status: IMPLEMENTED (existing code); assignment verification PLANNED
- Assigned Sprint: Sprint 03
- Acceptance Criteria: Each active participant may review the counterpart once on a completed selected job; ratings are integers 1–5; invalid/duplicate/pre-completion reviews fail; hidden reviews do not affect public ratings.
- Existing code evidence: [app/Actions/CreateReview.php](../../app/Actions/CreateReview.php)
- Verification: existing [test file](../../tests/Feature/CompletionReviewTest.php) plus manual workflow demonstration. Results: TO BE UPDATED DURING SPRINT.

## US-14 — Report inappropriate users or content

As a Worker/Ustaad, I want to report inappropriate users or content, so that I can request moderator intervention.

- Backlog rank: 14
- Priority: Must Have
- Story Points: 3 (proposed)
- Status: IMPLEMENTED (existing code); assignment verification PLANNED
- Assigned Sprint: Sprint 03
- Acceptance Criteria: Authenticated active users report user/job/review/message targets with a reason; message reports require participant access; hidden reviews cannot be reported; reports start pending and are rate limited.
- Existing code evidence: [app/Actions/CreateReport.php](../../app/Actions/CreateReport.php)
- Verification: existing [test file](../../tests/Feature/ModerationTest.php) plus manual workflow demonstration. Results: TO BE UPDATED DURING SPRINT.

## US-15 — Block or unblock another user

As a Worker/Ustaad, I want to block or unblock another user, so that I can control unwanted communication.

- Backlog rank: 15
- Priority: Should Have
- Story Points: 2 (proposed)
- Status: IMPLEMENTED (existing code); assignment verification PLANNED
- Assigned Sprint: Sprint 03
- Acceptance Criteria: Active users can block/unblock another user; blocking prevents messages between the pair; self-blocking is rejected; viewing history follows participant authorization.
- Existing code evidence: [app/Http/Controllers/UserBlockController.php](../../app/Http/Controllers/UserBlockController.php)
- Verification: existing [test file](../../tests/Feature/ModerationTest.php) plus manual workflow demonstration. Results: TO BE UPDATED DURING SPRINT.

## US-16 — Inspect and suspend or restore users

As a Admin, I want to inspect and suspend or restore users, so that I can protect marketplace participation.

- Backlog rank: 16
- Priority: Must Have
- Story Points: 3 (proposed)
- Status: IMPLEMENTED (existing code); assignment verification PLANNED
- Assigned Sprint: Sprint 04
- Acceptance Criteria: Only active admins access filtered/paginated users; valid active/suspended transitions work; administrator accounts cannot be suspended through this endpoint.
- Existing code evidence: [app/Http/Controllers/AdminUserController.php](../../app/Http/Controllers/AdminUserController.php)
- Verification: existing [test file](../../tests/Feature/ModerationTest.php) plus manual workflow demonstration. Results: TO BE UPDATED DURING SPRINT.

## US-17 — Inspect and cancel inappropriate jobs

As a Admin, I want to inspect and cancel inappropriate jobs, so that I can moderate marketplace requests.

- Backlog rank: 17
- Priority: Must Have
- Story Points: 3 (proposed)
- Status: IMPLEMENTED (existing code); assignment verification PLANNED
- Assigned Sprint: Sprint 04
- Acceptance Criteria: Admin filters jobs and cancels only open/assigned jobs; pending applications are rejected and history preserved; non-admin writes fail.
- Existing code evidence: [app/Http/Controllers/AdminJobController.php](../../app/Http/Controllers/AdminJobController.php)
- Verification: existing [test file](../../tests/Feature/ModerationTest.php) plus manual workflow demonstration. Results: TO BE UPDATED DURING SPRINT.

## US-18 — Manage skill categories

As a Admin, I want to manage skill categories, so that I can maintain a useful service taxonomy.

- Backlog rank: 18
- Priority: Should Have
- Story Points: 2 (proposed)
- Status: IMPLEMENTED (existing code); assignment verification PLANNED
- Assigned Sprint: Sprint 04
- Acceptance Criteria: Admin creates/updates valid categories with unique slugs and deletes unused categories; categories referenced by jobs or worker profiles cannot be deleted.
- Existing code evidence: [app/Http/Controllers/AdminCategoryController.php](../../app/Http/Controllers/AdminCategoryController.php)
- Verification: existing [test file](../../tests/Feature/ModerationTest.php) plus manual workflow demonstration. Results: TO BE UPDATED DURING SPRINT.

## US-19 — Resolve reports and hide or restore reviews

As a Admin, I want to resolve reports and hide or restore reviews, so that I can address abuse while preserving evidence.

- Backlog rank: 19
- Priority: Must Have
- Story Points: 3 (proposed)
- Status: IMPLEMENTED (existing code); assignment verification PLANNED
- Assigned Sprint: Sprint 04
- Acceptance Criteria: Admin marks reports reviewed/dismissed and hides/restores reviews; reported messages expose only reported content; non-admin access fails; hidden reviews are excluded from public ratings.
- Existing code evidence: [app/Http/Controllers/AdminReportController.php](../../app/Http/Controllers/AdminReportController.php)
- Verification: existing [test file](../../tests/Feature/ModerationTest.php) plus manual workflow demonstration. Results: TO BE UPDATED DURING SPRINT.

## US-20 — Send a contact enquiry

As a Visitor, I want to send a contact enquiry, so that I can ask the platform for assistance.

- Backlog rank: 20
- Priority: Could Have
- Story Points: 2 (proposed)
- Status: IMPLEMENTED (existing code); assignment verification PLANNED
- Assigned Sprint: Sprint 04
- Acceptance Criteria: Valid enquiry sends to configured recipient with visitor reply-to; required/invalid fields fail; sixth request within rate-limit window is blocked; delivery failure returns safe feedback without false success.
- Existing code evidence: [app/Http/Controllers/ContactController.php](../../app/Http/Controllers/ContactController.php)
- Verification: existing [test file](../../tests/Feature/ContactTest.php) plus manual workflow demonstration. Results: TO BE UPDATED DURING SPRINT.
