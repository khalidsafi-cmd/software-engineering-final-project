# Sprint 02 Backlog

Sprint 02 | October 12–17, 2026 | **PLANNED** | Proposed points: **16**

Sprint Goal: Verify the complete job, application and worker-selection workflow and resolve evidenced defects.

All sprint allocations and estimates are PLANNED proposals, not meeting commitments. Existing implementation is a code-inspection finding, not proof of passing tests or Product Owner acceptance. No sprint outcomes are recorded. Change work to IN PROGRESS only when actual work starts; record evidence and dates. Do not infer IN PROGRESS from a future schedule.

## Selected User Stories (proposed)

| Story | Selected scope | Points | Acceptance criteria |
| --- | --- | --- | --- |
| US-06 | post a categorized job | 3 | Valid title/category/description/location and optional budget create an open job owned by the authenticated active customer; invalid inputs and other roles fail. |
| US-07 | edit or cancel my open job | 3 | Only the active owner changes an open job; ownership/status injection fails; cancellation preserves application history; closed jobs cannot be edited or cancelled. |
| US-08 | apply to an open job | 3 | One pending application per eligible worker/job accepts optional message and price; duplicate applications, closed jobs and ineligible accounts fail. |
| US-09 | track my applications | 2 | My Applications shows only my records with job context and pagination; forged worker filters do not expose other workers; unauthorized roles are denied. |
| US-10 | inspect applicants and hire one worker | 5 | Only owner views applicants and accepts an eligible pending application for that job; selected status is accepted, others rejected, job assigned and conversation ensured atomically; repeat selection fails. |

## Planned Tasks

| Task | Expected work | Task Owner | Planned timing | Planned status |
| --- | --- | --- | --- | --- |
| T1 | Confirm priority, criteria and proposed estimates | Bahara Noorzai | Planning / start | PLANNED |
| T2 | Facilitate events, update traceability and collect genuine evidence | Ahmad Khalid Safi | Every sprint day | PLANNED |
| T3 | Verify US-06, US-07, US-08, US-09, US-10; run relevant existing tests and document findings | Sahar Haidary | Early/middle sprint | PLANNED |
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
