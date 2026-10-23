# Sprint 03 Review Meeting

Date: 2026-10-23

Time: Clock time is not specified in the source script (Asia/Kabul; after daily stand-up, before retrospective).

Facilitator: Ahmad Khalid Safi

Expected Participants: Ahmad Khalid Safi, Bahara Noorzai, Sahar Haidary

Recording URL: 

## Purpose / PLANNED Sprint Goal

Inspect verified work against the goal: Verify private communication, completion, reviews and trust controls with security checks.

## Planned Stories

| Story | Selected scope | Points | Acceptance criteria |
| --- | --- | --- | --- |
| US-11 | exchange messages with my selected worker | 5 | Customer and selected worker access their job conversation; valid messages persist and read tracking updates; outsiders, blocked pairs and ineligible senders cannot send; throttling applies. |
| US-12 | mark an assigned job completed | 2 | Only the active owner completes an assigned job with an accepted application; selected worker, outsiders and other job states are denied. |
| US-13 | review my worker after completion | 3 | Each active participant may review the counterpart once on a completed selected job; ratings are integers 1–5; invalid/duplicate/pre-completion reviews fail; hidden reviews do not affect public ratings. |
| US-14 | report inappropriate users or content | 3 | Authenticated active users report user/job/review/message targets with a reason; message reports require participant access; hidden reviews cannot be reported; reports start pending and are rate limited. |
| US-15 | block or unblock another user | 2 | Active users can block/unblock another user; blocking prevents messages between the pair; self-blocking is rejected; viewing history follows participant authorization. |

## Agenda

1. Revisit goal and proposed scope.
2. Demonstrate actual verified work and failure cases.
3. Inspect acceptance criteria with Bahara.
4. Discuss gaps and product feedback.
5. Record acceptance/rejection and proposed backlog changes.

## Demo / Acceptance Criteria and Evidence Status

- **Pending verification evidence** - US-11: demonstrate exchange messages with my selected worker and verify: Customer and selected worker access their job conversation; valid messages persist and read tracking updates; outsiders, blocked pairs and ineligible senders cannot send; throttling applies.
- **Pending verification evidence** - US-12: demonstrate mark an assigned job completed and verify: Only the active owner completes an assigned job with an accepted application; selected worker, outsiders and other job states are denied.
- **Pending verification evidence** - US-13: demonstrate review my worker after completion and verify: Each active participant may review the counterpart once on a completed selected job; ratings are integers 1–5; invalid/duplicate/pre-completion reviews fail; hidden reviews do not affect public ratings.
- **Pending verification evidence** - US-14: demonstrate report inappropriate users or content and verify: Authenticated active users report user/job/review/message targets with a reason; message reports require participant access; hidden reviews cannot be reported; reports start pending and are rate limited.
- **Pending verification evidence** - US-15: demonstrate block or unblock another user and verify: Active users can block/unblock another user; blocking prevents messages between the pair; self-blocking is rejected; viewing history follows participant authorization.

## Product Owner Responses

- **Criteria satisfied:** The script does not establish that all criteria passed; acceptance remains pending.
- **Gaps preventing acceptance:** Dated, story-specific verification results are absent; the acceptance table identifies the checks required.
- **Priority for remaining work:** Prioritize privacy and core-workflow problems in carry-over while reserving final-sprint time for administration and the integrated customer-worker journey.

## Participation in the Script

- Ahmad Khalid Safi (Scrum Master and facilitator)
- Bahara Noorzai (Product Owner)
- Sahar Haidary (Developer)

All three members have speaking parts in the source script. This records scripted participation; actual attendance is not established by that source.

## Completed Stories and Evidence Status

No story is established as verified and complete by the source script. US-11 through US-15 are covered in the technical walkthrough, but implementation and test presence do not supply dated execution evidence or satisfy acceptance. This is an explicit outcome for all five stories, not an unfilled completion field.

## Product Owner acceptance

In the scripted review, Bahara keeps US-11 through US-15 pending verification. No story is recorded as accepted.

| Story | Scripted acceptance outcome | Evidence required for a decision |
| --- | --- | --- |
| US-11 | Pending verification | Participant reads/sends, message persistence/read tracking, outsider rejection, blocked/ineligible senders and throttling. |
| US-12 | Pending verification | Active-owner completion of an assigned job with an accepted application; worker, outsider and wrong-state rejection. |
| US-13 | Pending verification | One counterpart review per participant after completion, integer ratings 1-5, invalid/duplicate/early-review rejection and visible-review-only averages. |
| US-14 | Pending verification | Accessible report targets, reason/pending status, rate limit, private-message participation and hidden-review restrictions. |
| US-15 | Pending verification | Block/unblock, prevention of sends in both directions, self-block rejection and participant-authorized history access. |

## Rejected/incomplete work

All five stories retain incomplete verification as described above. The script supplies no confirmed defect-based rejection and no passing result. Sahar owns the remaining checks and separates unavailable setup, unexecuted verification and confirmed defects. Prioritize privacy and core-workflow problems in carry-over while reserving final-sprint time for administration and the integrated customer-worker journey.

## Feedback

Bahara requires evidence for privacy, completion permissions and duplicate-review behavior. Reading history and sending messages are separate permissions. The selected worker can review the customer after completion but cannot complete the job. Report access must not expose unrelated private content, and hidden-review/public-rating behavior connects to Sprint 4 moderation.

## Decisions from the Script

- Retain pending acceptance until criterion-level evidence supports a Product Owner decision.
- Prioritize privacy and core-workflow problems in carry-over while reserving final-sprint time for administration and the integrated customer-worker journey.
- Keep incomplete work visible in tasks, review outcomes and progress records; the sprint end does not automatically satisfy Done.

| Owner | Assigned follow-up | Planned checkpoint |
| --- | --- | --- |
| Sahar Haidary | Identify missing checks and setup, attach technical results by story and document confirmed defects with reproducible context. | 2026-10-24 next-sprint planning |
| Bahara Noorzai | Maintain acceptance outcomes and order carry-over against product priorities. | 2026-10-24 next-sprint planning |
| Ahmad Khalid Safi | Link minutes, outcome records and available recording evidence; reconcile remaining work with progress notes. | 2026-10-23 close-out and 2026-10-24 next-sprint planning |

## Meeting Summary from the Script

Ahmad ordered the review around coordination, completion and trust. Sahar described the baseline and required checks without claiming dated results. Bahara examined messaging, completion, mutual reviews, reports and blocking, and kept US-11 through US-15 pending verification. The group linked moderation dependencies and unresolved items to October 24 planning. Defect records require actor, job state and reproduction steps.

[Structured outcome record](../../09-reviews/sprint-03-review.md)
