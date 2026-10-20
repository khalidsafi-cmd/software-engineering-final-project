# Sprint 01 Planning

> Record basis: Completed from the [matching meeting meeting](../../meetings/2026-10-06-sprint-planning-meeting.md). The source is a rehearsal dialogue. Updates, decisions and actions below summarize that dialogue; they do not certify a held meeting, executed tests or actual acceptance.

Date: 2026-10-06

Time: Clock time is not specified in the source meeting (Asia/Kabul; before first stand-up).

Facilitator: Ahmad Khalid Safi

Expected Participants: Ahmad Khalid Safi, Bahara Noorzai, Sahar Haidary

Recording Link: No recording URL is supplied by the source meeting; this record has no linked recording.

## PLANNED Sprint Goal

Verify requirements, architecture, public discovery, authentication and worker profiles; establish Scrum documentation.

## Candidate Backlog / Selected User Stories (proposed)

| Story | Selected scope | Points | Acceptance criteria |
| --- | --- | --- | --- |
| US-01 | browse and filter public jobs | 3 | Open jobs of active customers appear; keyword/category/location filters combine; pagination retains filters; empty results and missing records are handled. |
| US-02 | discover workers and view public profiles | 3 | Only active worker profiles appear; filters combine; profiles expose skills and real visible-review averages without private account fields. |
| US-03 | register as a customer or worker | 3 | Valid customer/worker registration succeeds; worker profile is created; admin/invalid role injection is rejected; duplicate identity fields are validated. |
| US-04 | log in and manage account credentials | 3 | Valid login and logout work; invalid credentials fail; reset tokens and email verification are checked with their existing Auth tests; profile changes preserve protected fields. |
| US-05 | maintain my skills and worker profile | 3 | Own bio, experience, location, availability, trades and valid photo can be updated; invalid trades/uploads fail; other roles and suspended workers cannot edit. |

## Expected Capacity

One formal Developer; individual available hours are not quantified in the source meeting. Proposed 15 points for assignment verification/refinement. The meeting leaves capacity and the point commitment provisional; points are not hours.

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

The meeting retains all five proposed stories. It clarifies combined discovery filters and pagination, active public worker profiles, private-field exclusion, customer/worker registration, rejection of administrator-role injection, and own-profile editing. The existing application is the baseline for verification; no additional story or finalized capacity estimate is introduced.

## Final commitment

The meeting planning outcome is to begin verification of US-01 through US-05 within the stated Sprint 1 goal. The 15-point total remains a proposal: the meeting does not establish individual availability or a final capacity-backed commitment. Bahara owns criteria and priorities, Sahar owns the Sprint Backlog and technical work, and Ahmad owns process records and progress tracking. Acceptance remains a separate evidence-based review decision on 2026-10-11.

## Meeting decisions

- Begin with requirements-to-test mapping and normal browsing/account flows, then check invalid inputs and unauthorized requests.
- Keep three points per story provisional until availability and initial findings establish feasibility. If scope must shrink, Bahara prioritizes core account access and discovery.
- Require criterion-level evidence and important failure cases before acceptance; retain command, date, environment and result together.
- Sahar compares use-case actors and sequence behavior with the source; Ahmad links observations to stories and remaining work.

### Assigned Actions

| Owner | Assigned action | Planned checkpoint |
| --- | --- | --- |
| Bahara Noorzai | Review story wording and resolve ambiguities in discovery, registration and account permissions. | Start 2026-10-06; follow up through the sprint |
| Sahar Haidary | Map public-website, authorization and authentication tests to the five stories; start public browsing and account setup. | Start 2026-10-06; follow up through the sprint |
| Ahmad Khalid Safi | Maintain the schedule, meeting records, story references and burndown. | Start 2026-10-06; follow up through the sprint |
| Sahar Haidary; Bahara Noorzai; Ahmad Khalid Safi | Technical diagram comparison, business-rule review and traceability check, respectively. | 2026-10-10 |
| Bahara Noorzai; Sahar Haidary; Ahmad Khalid Safi | Acceptance decisions, technical walkthrough and minutes, respectively. | 2026-10-11 |

## Meeting Summary from the meeting

Ahmad opened with the October 11 goal and the existing marketplace baseline. Bahara described visitor, customer and worker needs and the evidence required for acceptance. Sahar outlined normal-flow, invalid-input and authorization checks, plus the UML comparison. The group retained the 15-point proposal as provisional, assigned product, technical and process responsibilities, and placed review preparation on October 10.
