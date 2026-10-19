# Sprint 03 Backlog

Sprint 03 | October 18–23, 2026 | **PLANNED** | Proposed points: **15**

Sprint Goal: Verify private communication, completion, reviews and trust controls with security checks.

All sprint allocations and estimates are PLANNED proposals, not meeting commitments. Existing implementation is a code-inspection finding, not proof of passing tests or Product Owner acceptance. No sprint outcomes are recorded. Change work to IN PROGRESS only when actual work starts; record evidence and dates. Do not infer IN PROGRESS from a future schedule.

## Selected User Stories (proposed)

| Story | Selected scope | Points | Acceptance criteria |
| --- | --- | --- | --- |
| US-11 | exchange messages with my selected worker | 5 | Customer and selected worker access their job conversation; valid messages persist and read tracking updates; outsiders, blocked pairs and ineligible senders cannot send; throttling applies. |
| US-12 | mark an assigned job completed | 2 | Only the active owner completes an assigned job with an accepted application; selected worker, outsiders and other job states are denied. |
| US-13 | review my worker after completion | 3 | Each active participant may review the counterpart once on a completed selected job; ratings are integers 1–5; invalid/duplicate/pre-completion reviews fail; hidden reviews do not affect public ratings. |
| US-14 | report inappropriate users or content | 3 | Authenticated active users report user/job/review/message targets with a reason; message reports require participant access; hidden reviews cannot be reported; reports start pending and are rate limited. |
| US-15 | block or unblock another user | 2 | Active users can block/unblock another user; blocking prevents messages between the pair; self-blocking is rejected; viewing history follows participant authorization. |

## Planned Tasks

| Task | Expected work | Task Owner | Planned timing | Planned status |
| --- | --- | --- | --- | --- |
| T1 | Confirm priority, criteria and proposed estimates | Bahara Noorzai | Planning / start | PLANNED |
| T2 | Facilitate events, update traceability and collect genuine evidence | Ahmad Khalid Safi | Every sprint day | PLANNED |
| T3 | Verify US-11, US-12, US-13, US-14, US-15; run relevant existing tests and document findings | Sahar Haidary | Early/middle sprint | PLANNED |
| T4 | Triage evidenced defects and agree scope; implement approved sprint fixes | Sahar Haidary (Bahara prioritizes) | Middle sprint | PLANNED |
| T5 | Check requirements/UML consistency and review technical artifacts | Sahar Haidary; Ahmad assists | Before review | PLANNED |
| T6 | Demonstrate criteria and record actual accept/reject decisions | Bahara Noorzai; Sahar demonstrates; Ahmad records | Sprint Review | PLANNED |

## Definition of Done

- [ ] Story acceptance criteria satisfied and linked evidence recorded.
- [ ] Applicable implementation/fix completed; documentation-only work is accurate and complete.
- [ ] Work committed and pushed to GitHub with meaningful messages.
- [ ] Peer review performed where practical; record reviewer or reason unavailable.
- [ ] Relevant automated tests pass for behavior changes; record actual command/date/result.
- [ ] Applicable manual workflow and important failure paths verified.
- [ ] Requirements, diagrams and documentation updated with working links.
- [ ] No known blocking defects; unresolved issues recorded honestly.
- [ ] Bahara accepts the story at the real Sprint Review.

Documentation-only tasks require source accuracy, readable Markdown, correct links and peer/product review as applicable; software tests apply only when relevant. Existing implementation alone does not satisfy assignment verification or Product Owner acceptance.

## Commitment and progress

Final selection/capacity decisions: TO BE COMPLETED AFTER MEETING.

Actual task progress, remaining effort and defects: TO BE UPDATED DURING SPRINT.

[Goal](sprint-goal.md) · [Task details](tasks.md)
