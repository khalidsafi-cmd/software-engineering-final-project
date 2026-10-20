# Sprint 03 Planning

> Record basis: Completed from the [matching meeting meeting](../../meetings/2026-10-18-sprint-planning-meeting.md). The source is a rehearsal dialogue. Updates, decisions and actions below summarize that dialogue; they do not certify a held meeting, executed tests or actual acceptance.

Date: 2026-10-18

Time: Clock time is not specified in the source meeting (Asia/Kabul; before first stand-up).

Facilitator: Ahmad Khalid Safi

Expected Participants: Ahmad Khalid Safi, Bahara Noorzai, Sahar Haidary

Recording Link: No recording URL is supplied by the source meeting; this record has no linked recording.

## PLANNED Sprint Goal

Verify private communication, completion, reviews and trust controls with security checks.

## Candidate Backlog / Selected User Stories (proposed)

| Story | Selected scope | Points | Acceptance criteria |
| --- | --- | --- | --- |
| US-11 | exchange messages with my selected worker | 5 | Customer and selected worker access their job conversation; valid messages persist and read tracking updates; outsiders, blocked pairs and ineligible senders cannot send; throttling applies. |
| US-12 | mark an assigned job completed | 2 | Only the active owner completes an assigned job with an accepted application; selected worker, outsiders and other job states are denied. |
| US-13 | review my worker after completion | 3 | Each active participant may review the counterpart once on a completed selected job; ratings are integers 1–5; invalid/duplicate/pre-completion reviews fail; hidden reviews do not affect public ratings. |
| US-14 | report inappropriate users or content | 3 | Authenticated active users report user/job/review/message targets with a reason; message reports require participant access; hidden reviews cannot be reported; reports start pending and are rate limited. |
| US-15 | block or unblock another user | 2 | Active users can block/unblock another user; blocking prevents messages between the pair; self-blocking is rejected; viewing history follows participant authorization. |

## Expected Capacity

One formal Developer; individual available hours are not quantified in the source meeting. Proposed 15 points for assignment verification/refinement. The meeting leaves capacity and the point commitment provisional; points are not hours.

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

## Changes made during meeting

The meeting retains messaging, completion, reviews, reports and blocking. It clarifies the dependency on an assigned job with an accepted application, customer-only completion, reviews by both participants after completion, and separate permissions for reading history and sending messages. Estimates remain five, two, three, three and two points respectively. Unresolved hiring work is a visible dependency, not an implicitly completed prerequisite.

## Final commitment

The meeting planning outcome is to begin verification of US-11 through US-15 within the stated Sprint 3 goal. The 15-point total remains a proposal: the meeting does not establish individual availability or a final capacity-backed commitment. Bahara owns criteria and priorities, Sahar owns the Sprint Backlog and technical work, and Ahmad owns process records and progress tracking. Acceptance remains a separate evidence-based review decision on 2026-10-23.

## Meeting decisions

- Prepare customer, selected-worker and outsider accounts against a valid assigned job before communication checks.
- Check participant privacy, blocked/suspended senders, validation, throttling and read tracking; reporting a private message still requires participant access.
- Permit completion only by the active job owner and one counterpart review per participant after completion; ratings are integers from one to five and exclude hidden reviews from public averages.
- Prioritize privacy and unauthorized access, link moderation dependencies to Sprint 4 and compare messaging/completion diagrams on October 22.

### Assigned Actions

| Owner | Assigned action | Planned checkpoint |
| --- | --- | --- |
| Bahara Noorzai | Review participant, completion, review, report and blocking criteria; retain moderation priorities in the Product Backlog. | Start 2026-10-18; follow up through the sprint |
| Sahar Haidary | Prepare account/job states and communication, completion-review and relevant moderation checks; link technical evidence by story. | Start 2026-10-18; follow up through the sprint |
| Ahmad Khalid Safi | Maintain blocker follow-up, meeting records and burndown; connect the October 23 review to all five stories. | Start 2026-10-18; follow up through the sprint |
| Sahar Haidary; Bahara Noorzai; Ahmad Khalid Safi | Technical diagram comparison, business-rule review and traceability check, respectively. | 2026-10-22 |
| Bahara Noorzai; Sahar Haidary; Ahmad Khalid Safi | Acceptance decisions, technical walkthrough and minutes, respectively. | 2026-10-23 |

## Meeting Summary from the meeting

Ahmad introduced the 15-point proposal and October 23 review. Sahar identified hiring as the prerequisite for messaging and completion. Bahara clarified participant privacy, customer-only completion and counterpart reviews. The team separated blocking from history access, kept moderation dependencies visible and assigned diagram comparison to October 22. No availability figures or final point commitment are recorded in the dialogue.
