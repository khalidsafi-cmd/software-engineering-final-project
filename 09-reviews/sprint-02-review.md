# Sprint 02 Review

## Sprint goal

Verify the complete job, application and worker-selection workflow and resolve evidenced defects.

Dates: October 12–17, 2026

## Stories reviewed and acceptance criteria

| Story | Selected scope | Points | Acceptance criteria |
| --- | --- | --- | --- |
| US-06 | post a categorized job | 3 | Valid title/category/description/location and optional budget create an open job owned by the authenticated active customer; invalid inputs and other roles fail. |
| US-07 | edit or cancel my open job | 3 | Only the active owner changes an open job; ownership/status injection fails; cancellation preserves application history; closed jobs cannot be edited or cancelled. |
| US-08 | apply to an open job | 3 | One pending application per eligible worker/job accepts optional message and price; duplicate applications, closed jobs and ineligible accounts fail. |
| US-09 | track my applications | 2 | My Applications shows only my records with job context and pagination; forged worker filters do not expose other workers; unauthorized roles are denied. |
| US-10 | inspect applicants and hire one worker | 5 | Only owner views applicants and accepts an eligible pending application for that job; selected status is accepted, others rejected, job assigned and conversation ensured atomically; repeat selection fails. |

[Review meeting record](../07-meetings/sprint-review/2026-10-17-sprint-review.md) · [Sprint backlog](../06-sprints/sprint-02/sprint-backlog.md) · [Definition of Done](../06-sprints/sprint-02/definition-of-done.md)

Recording: No recording is linked in the review meeting record.

## Review summary

The review covers the five stories above against their acceptance criteria. Sahar Haidary presents the technical baseline, Bahara Noorzai owns acceptance decisions, and Ahmad Khalid Safi maintains review records. Existing implementation and test files are available, but completed story-specific execution results are absent.

## Product Owner feedback

Bahara assesses the customer and worker journey story by story. Editing and cancellation need separate checks, and a working application submission does not establish list privacy. Sahar describes selection as coupled job/application/conversation changes; rollback and repeated requests require evidence. A valid assigned job and accepted application are prerequisites for Sprint 3 messaging.

## Acceptance decisions

**Accepted stories: none recorded.** All five stories remain pending verification. The following checks are required before acceptance:

| Story | Outcome | Evidence required for acceptance |
| --- | --- | --- |
| US-06 | Pending verification | Valid/invalid job posting, optional budget, active-customer role, authenticated ownership and initial open state. |
| US-07 | Pending verification | Active-owner editing/cancellation, protected fields, closed-state rejection and preserved application history. |
| US-08 | Pending verification | Eligible worker application, optional message/price, duplicate prevention and closed/ineligible-account rejection. |
| US-09 | Pending verification | Own application list, pagination/job context and rejection of forged worker filters or unauthorized roles. |
| US-10 | Pending verification | Eligible same-job selection, accepted/rejected application states, assigned job, conversation, repeated-selection rejection and transaction rollback. |

## Incomplete work

All five stories retain incomplete verification. No confirmed defect-based rejection or passing result is recorded. Sahar owns the remaining checks and separates unavailable setup, unexecuted verification and reproducible defects. Points remain uncredited until the Definition of Done and Product Owner acceptance are satisfied.

## Carry-over items

Prioritize US-06 through US-10 against Sprint 3 work. Hiring consistency and application privacy remain unresolved. A valid assigned job and accepted application are prerequisites for private communication.

Bahara orders carry-over against product priorities. Unresolved work remains visible without automatically expanding another sprint's point commitment.

## Lessons learned

- Verify ownership and job state together.
- Check selection as one transaction across jobs, applications and conversations.
- Preserve unresolved hiring checks as messaging dependencies.

[Related retrospective](../07-meetings/retrospectives/2026-10-17-sprint-retrospective.md)

## Decisions and follow-up

- Retain pending acceptance until criterion-level evidence supports a Product Owner decision.
- Prioritize the carry-over above and retain reasons for scope changes.
- Keep incomplete work visible in tasks, review outcomes and progress records; reaching the sprint end does not satisfy Done.

| Owner | Follow-up responsibility |
| --- | --- |
| Sahar Haidary | Identify remaining checks and setup, attach results by story and document confirmed defects with actor and workflow-state details. |
| Bahara Noorzai | Maintain acceptance decisions, order carry-over and keep criteria and backlog status consistent. |
| Ahmad Khalid Safi | Link review records, tasks, recordings and progress notes; follow up on missing evidence and assigned actions. |
