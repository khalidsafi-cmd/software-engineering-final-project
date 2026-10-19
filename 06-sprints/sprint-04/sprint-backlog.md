# Sprint 04 Backlog

Sprint 04 | October 24–30, 2026 | **PLANNED** | Proposed points: **13**

Sprint Goal: Verify administration, integrate workflows, refine UX, finalize models and prepare submission evidence.

All sprint allocations and estimates are PLANNED proposals, not meeting commitments. Existing implementation is a code-inspection finding, not proof of passing tests or Product Owner acceptance. No sprint outcomes are recorded. Change work to IN PROGRESS only when actual work starts; record evidence and dates. Do not infer IN PROGRESS from a future schedule.

## Selected User Stories (proposed)

| Story | Selected scope | Points | Acceptance criteria |
| --- | --- | --- | --- |
| US-16 | inspect and suspend or restore users | 3 | Only active admins access filtered/paginated users; valid active/suspended transitions work; administrator accounts cannot be suspended through this endpoint. |
| US-17 | inspect and cancel inappropriate jobs | 3 | Admin filters jobs and cancels only open/assigned jobs; pending applications are rejected and history preserved; non-admin writes fail. |
| US-18 | manage skill categories | 2 | Admin creates/updates valid categories with unique slugs and deletes unused categories; categories referenced by jobs or worker profiles cannot be deleted. |
| US-19 | resolve reports and hide or restore reviews | 3 | Admin marks reports reviewed/dismissed and hides/restores reviews; reported messages expose only reported content; non-admin access fails; hidden reviews are excluded from public ratings. |
| US-20 | send a contact enquiry | 2 | Valid enquiry sends to configured recipient with visitor reply-to; required/invalid fields fail; sixth request within rate-limit window is blocked; delivery failure returns safe feedback without false success. |

## Planned Tasks

| Task | Expected work | Task Owner | Planned timing | Planned status |
| --- | --- | --- | --- | --- |
| T1 | Confirm priority, criteria and proposed estimates | Bahara Noorzai | Planning / start | PLANNED |
| T2 | Facilitate events, update traceability and collect genuine evidence | Ahmad Khalid Safi | Every sprint day | PLANNED |
| T3 | Verify US-16, US-17, US-18, US-19, US-20; run relevant existing tests and document findings | Sahar Haidary | Early/middle sprint | PLANNED |
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
