# Sprint 03 Review

## Sprint goal

Verify private communication, completion, reviews and trust controls with security checks.

Dates: October 18–23, 2026

## Stories reviewed and acceptance criteria

| Story | Selected scope | Points | Acceptance criteria |
| --- | --- | --- | --- |
| US-11 | exchange messages with my selected worker | 5 | Customer and selected worker access their job conversation; valid messages persist and read tracking updates; outsiders, blocked pairs and ineligible senders cannot send; throttling applies. |
| US-12 | mark an assigned job completed | 2 | Only the active owner completes an assigned job with an accepted application; selected worker, outsiders and other job states are denied. |
| US-13 | review my worker after completion | 3 | Each active participant may review the counterpart once on a completed selected job; ratings are integers 1–5; invalid/duplicate/pre-completion reviews fail; hidden reviews do not affect public ratings. |
| US-14 | report inappropriate users or content | 3 | Authenticated active users report user/job/review/message targets with a reason; message reports require participant access; hidden reviews cannot be reported; reports start pending and are rate limited. |
| US-15 | block or unblock another user | 2 | Active users can block/unblock another user; blocking prevents messages between the pair; self-blocking is rejected; viewing history follows participant authorization. |

[Review meeting record](../07-meetings/sprint-review/2026-10-23-sprint-review.md) · [Sprint backlog](../06-sprints/sprint-03/sprint-backlog.md) · [Definition of Done](../06-sprints/sprint-03/definition-of-done.md)

Recording: [Sprint review recording](https://drive.google.com/file/d/1K8r1imkHpvgC9fetpACaLHvT9svTxFCF/view?usp=drive_link).

## Review summary

The review covers the five stories above against their acceptance criteria. Sahar Haidary presents the technical baseline, Bahara Noorzai owns acceptance decisions, and Ahmad Khalid Safi maintains review records. Existing implementation and test files are available, but completed story-specific execution results are absent. The source describes a scripted walkthrough; it does not establish completed runtime verification.

## Product Owner feedback

Bahara requires evidence for privacy, completion permissions and duplicate-review behavior. Reading history and sending messages are separate permissions. The selected worker can review the customer after completion but cannot complete the job. Report access must not expose unrelated private content, and hidden-review/public-rating behavior connects to Sprint 4 moderation.

## Acceptance decisions

**Accepted stories: none recorded.** All five stories remain pending verification. The following checks are required before acceptance:

| Story | Outcome | Evidence required for acceptance |
| --- | --- | --- |
| US-11 | Pending verification | Participant reads/sends, message persistence/read tracking, outsider rejection, blocked/ineligible senders and throttling. |
| US-12 | Pending verification | Active-owner completion of an assigned job with an accepted application; worker, outsider and wrong-state rejection. |
| US-13 | Pending verification | One counterpart review per participant after completion, integer ratings 1-5, invalid/duplicate/early-review rejection and visible-review-only averages. |
| US-14 | Pending verification | Accessible report targets, reason/pending status, rate limit, private-message participation and hidden-review restrictions. |
| US-15 | Pending verification | Block/unblock, prevention of sends in both directions, self-block rejection and participant-authorized history access. |

## Incomplete work

All five stories retain incomplete verification. No confirmed defect-based rejection or passing result is recorded. Sahar owns the remaining checks and separates unavailable setup, unexecuted verification and reproducible defects. Points remain uncredited until the Definition of Done and Product Owner acceptance are satisfied.

## Carry-over items

Carry unresolved US-11 through US-15 into Sprint 4 prioritization. Address privacy and core-workflow gaps, connect hidden-review/public-rating checks to moderation, and reserve integration time.

Bahara orders carry-over against product priorities. Unresolved work remains visible without automatically expanding another sprint's point commitment.

## Lessons learned

- Separate permission to read history from permission to send messages.
- Prepare customer, selected-worker and outsider cases for the relevant job states.
- Carry moderation visibility and hidden-review dependencies into administration.

[Related retrospective](../07-meetings/retrospectives/2026-10-23-sprint-retrospective.md)

## Decisions and follow-up

- Retain pending acceptance until criterion-level evidence supports a Product Owner decision.
- Prioritize the carry-over above and retain reasons for scope changes.
- Keep incomplete work visible in tasks, review outcomes and progress records; reaching the sprint end does not satisfy Done.

| Owner | Follow-up responsibility |
| --- | --- |
| Sahar Haidary | Identify remaining checks and setup, attach results by story and document confirmed defects with actor and workflow-state details. |
| Bahara Noorzai | Maintain acceptance decisions, order carry-over and keep criteria and backlog status consistent. |
| Ahmad Khalid Safi | Link review records, tasks, recordings and progress notes; follow up on missing evidence and assigned actions. |
