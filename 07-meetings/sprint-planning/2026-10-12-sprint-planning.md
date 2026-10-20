# Sprint 02 Planning

> Record basis: Completed from the [matching meeting script](../../scripts/2026-10-12-sprint-planning-script.md). The source is a rehearsal dialogue. Updates, decisions and actions below summarize that dialogue; they do not certify a held meeting, executed tests or actual acceptance.

Date: 2026-10-12

Time: Clock time is not specified in the source script (Asia/Kabul; before first stand-up).

Facilitator: Ahmad Khalid Safi

Expected Participants: Ahmad Khalid Safi, Bahara Noorzai, Sahar Haidary

Recording Link: No recording URL is supplied by the source script; this record has no linked recording.

## PLANNED Sprint Goal

Verify the complete job, application and worker-selection workflow and resolve evidenced defects.

## Candidate Backlog / Selected User Stories (proposed)

| Story | Selected scope | Points | Acceptance criteria |
| --- | --- | --- | --- |
| US-06 | post a categorized job | 3 | Valid title/category/description/location and optional budget create an open job owned by the authenticated active customer; invalid inputs and other roles fail. |
| US-07 | edit or cancel my open job | 3 | Only the active owner changes an open job; ownership/status injection fails; cancellation preserves application history; closed jobs cannot be edited or cancelled. |
| US-08 | apply to an open job | 3 | One pending application per eligible worker/job accepts optional message and price; duplicate applications, closed jobs and ineligible accounts fail. |
| US-09 | track my applications | 2 | My Applications shows only my records with job context and pagination; forged worker filters do not expose other workers; unauthorized roles are denied. |
| US-10 | inspect applicants and hire one worker | 5 | Only owner views applicants and accepts an eligible pending application for that job; selected status is accepted, others rejected, job assigned and conversation ensured atomically; repeat selection fails. |

## Expected Capacity

One formal Developer; individual available hours are not quantified in the source script. Proposed 16 points for assignment verification/refinement. The script leaves capacity and the point commitment provisional; points are not hours.

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

These are completion criteria agreed for the work, not a report that the criteria have been met.

- Story acceptance criteria satisfied and linked evidence recorded.
- Applicable implementation/fix completed; documentation-only work is accurate and complete.
- Work committed and pushed to GitHub with meaningful messages.
- Peer review performed where practical; record reviewer or reason unavailable.
- Relevant automated tests pass for behavior changes; record actual command/date/result.
- Applicable manual workflow and important failure paths verified.
- Requirements, diagrams and documentation updated with working links.
- No known blocking defects; unresolved issues recorded honestly.
- Bahara accepts the story at the real Sprint Review.

Documentation-only tasks require source accuracy, readable Markdown, correct links and peer/product review as applicable; software tests apply only when relevant. Existing implementation alone does not satisfy assignment verification or Product Owner acceptance.

## Agenda

1. Confirm product priorities and existing-code baseline.
2. Confirm Sprint Goal and story criteria.
3. Discuss availability, dependencies and risks.
4. Select feasible scope and task ownership.
5. Confirm Definition of Done and evidence responsibilities.

## Participation in the Script

- Ahmad Khalid Safi (Scrum Master and facilitator)
- Bahara Noorzai (Product Owner)
- Sahar Haidary (Developer)

All three members have speaking parts in the source script. This records scripted participation; actual attendance is not established by that source.

## Changes made during meeting

The script retains posting, open-job management, applications, private application tracking and worker selection. It explicitly includes optional budget, protected ownership/status fields, duplicate applications, forged worker filters, cross-job selection, repeated selection and rollback. US-10 retains five proposed points because of its coupled state changes. Earlier account work remains identified separately; the script does not add it to a final commitment.

## Final commitment

The scripted planning outcome is to begin verification of US-06 through US-10 within the stated Sprint 2 goal. The 16-point total remains a proposal: the script does not establish individual availability or a final capacity-backed commitment. Bahara owns criteria and priorities, Sahar owns the Sprint Backlog and technical work, and Ahmad owns process records and progress tracking. Acceptance remains a separate evidence-based review decision on 2026-10-17.

## Meeting decisions

- Use owner, other-customer and worker accounts, several applications on one job and an application belonging to another job.
- Verify selection as one operation: accept one application, reject other pending applications, assign the job and ensure the participant conversation; check rollback and repeated selection.
- Prioritize ownership and hiring-consistency defects before presentation changes.
- Compare post/apply/select diagrams on October 16, then record individual acceptance outcomes and any carry-over at the October 17 review.

### Assigned Actions

| Owner | Assigned action | Planned checkpoint |
| --- | --- | --- |
| Bahara Noorzai | Clarify ownership, optional budget, open-job management and hiring criteria; prioritize any earlier carry-over explicitly. | Start 2026-10-12; follow up through the sprint |
| Sahar Haidary | Prepare role-specific accounts and application data; organize job-marketplace checks in customer/worker journey order. | Start 2026-10-12; follow up through the sprint |
| Ahmad Khalid Safi | Keep carry-over visible in event/progress records and link diagrams, stories and evidence. | Start 2026-10-12; follow up through the sprint |
| Sahar Haidary; Bahara Noorzai; Ahmad Khalid Safi | Technical diagram comparison, business-rule review and traceability check, respectively. | 2026-10-16 |
| Bahara Noorzai; Sahar Haidary; Ahmad Khalid Safi | Acceptance decisions, technical walkthrough and minutes, respectively. | 2026-10-17 |

## Meeting Summary from the Script

Ahmad introduced the job workflow and the need to retain unfinished account work. Bahara set the business rules for job ownership, applications and one-worker selection. Sahar described test data, protected-field checks and the selection transaction, including rollback. The discussion retained 16 provisional points, assigned criteria and technical evidence owners, and scheduled diagram comparison before the October 17 review.
