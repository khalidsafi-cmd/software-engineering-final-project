# Sprint 01 Backlog

Sprint 01 | October 6–11, 2026 | **PLANNED** | Proposed points: **15**

Sprint Goal: Verify requirements, architecture, public discovery, authentication and worker profiles; establish Scrum documentation.

All sprint allocations and estimates are PLANNED proposals, not meeting commitments. Existing implementation is a code-inspection finding, not proof of passing tests or Product Owner acceptance. No sprint outcomes are recorded. Change work to IN PROGRESS only when actual work starts; record evidence and dates. Do not infer IN PROGRESS from a future schedule.

## Selected User Stories (proposed)

| Story | Selected scope | Points | Acceptance criteria |
| --- | --- | --- | --- |
| US-01 | browse and filter public jobs | 3 | Open jobs of active customers appear; keyword/category/location filters combine; pagination retains filters; empty results and missing records are handled. |
| US-02 | discover workers and view public profiles | 3 | Only active worker profiles appear; filters combine; profiles expose skills and real visible-review averages without private account fields. |
| US-03 | register as a customer or worker | 3 | Valid customer/worker registration succeeds; worker profile is created; admin/invalid role injection is rejected; duplicate identity fields are validated. |
| US-04 | log in and manage account credentials | 3 | Valid login and logout work; invalid credentials fail; reset tokens and email verification are checked with their existing Auth tests; profile changes preserve protected fields. |
| US-05 | maintain my skills and worker profile | 3 | Own bio, experience, location, availability, trades and valid photo can be updated; invalid trades/uploads fail; other roles and suspended workers cannot edit. |

## Planned Tasks

| Task | Expected work | Task Owner | Planned timing | Planned status |
| --- | --- | --- | --- | --- |
| T1 | Confirm priority, criteria and proposed estimates | Bahara Noorzai | Planning / start | PLANNED |
| T2 | Facilitate events, update traceability and collect genuine evidence | Ahmad Khalid Safi | Every sprint day | PLANNED |
| T3 | Verify US-01, US-02, US-03, US-04, US-05; run relevant existing tests and document findings | Sahar Haidary | Early/middle sprint | PLANNED |
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
