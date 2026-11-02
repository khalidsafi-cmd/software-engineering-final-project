# Sprint 04 Planning

Date: 2026-10-24

Facilitator: Ahmad Khalid Safi

Expected Participants: Ahmad Khalid Safi, Bahara Noorzai, Sahar Haidary

Recording Link: No recording URL is supplied by the source script; this record has no linked recording.

## PLANNED Sprint Goal

Verify administration, integrate workflows, refine UX, finalize models and prepare submission evidence.

## Candidate Backlog / Selected User Stories (proposed)

| Story | Selected scope | Points | Acceptance criteria |
| --- | --- | --- | --- |
| US-16 | inspect and suspend or restore users | 3 | Only active admins access filtered/paginated users; valid active/suspended transitions work; administrator accounts cannot be suspended through this endpoint. |
| US-17 | inspect and cancel inappropriate jobs | 3 | Admin filters jobs and cancels only open/assigned jobs; pending applications are rejected and history preserved; non-admin writes fail. |
| US-18 | manage skill categories | 2 | Admin creates/updates valid categories with unique slugs and deletes unused categories; categories referenced by jobs or worker profiles cannot be deleted. |
| US-19 | resolve reports and hide or restore reviews | 3 | Admin marks reports reviewed/dismissed and hides/restores reviews; reported messages expose only reported content; non-admin access fails; hidden reviews are excluded from public ratings. |
| US-20 | send a contact enquiry | 2 | Valid enquiry sends to configured recipient with visitor reply-to; required/invalid fields fail; sixth request within rate-limit window is blocked; delivery failure returns safe feedback without false success. |

## Expected Capacity

One formal Developer; individual available hours are not quantified in the source script. Proposed 13 points for assignment verification/refinement. The script leaves capacity and the point commitment provisional; points are not hours.

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

The script retains user administration, job moderation, categories, report/review moderation and contact enquiries. It protects time for the integrated customer-worker journey, responsive checks at 360 and 1280 pixels, measured quality evidence and final UML comparison. Earlier carry-over remains subject to prioritization. October 31 is final preparation outside the sprint; no additional sprint meeting is proposed.

## Final commitment

The scripted planning outcome is to begin verification of US-16 through US-20 within the stated Sprint 4 goal. The 13-point total remains a proposal: the script does not establish individual availability or a final capacity-backed commitment. Bahara owns criteria and priorities, Sahar owns the Sprint Backlog and technical work, and Ahmad owns process records and progress tracking. Acceptance remains a separate evidence-based review decision on 2026-10-30.

## Meeting decisions

- Verify active-admin access, protected administrator accounts, allowed cancellation states, preserved history, unique category slugs and deletion restrictions for referenced categories.
- Restrict moderation to reported message content and check the effect of hidden reviews on public ratings.
- Check contact delivery, recipient/reply-to, invalid fields, throttling and safe mail-failure feedback.
- Reserve integration and responsive-check time; attach dataset/environment to measurements and state missing measurements explicitly.
- Compare final UML on October 29 and review on October 30. For October 31, Bahara owns product records, Sahar technical/repository checks and Ahmad submission/process evidence.

### Assigned Actions

| Owner | Assigned action | Planned checkpoint |
| --- | --- | --- |
| Bahara Noorzai | Prioritize administration and carry-over, align the deliverables checklist and retain reasons for scope changes. | Start 2026-10-24; follow up through the sprint |
| Sahar Haidary | Prepare moderation/contact cases and integrated workflow checks; organize responsive and quality evidence. | Start 2026-10-24; follow up through the sprint |
| Ahmad Khalid Safi | Identify missing meeting evidence and recording access, coordinate final preparation and verify platform timezone against the November 1, 11:59 PM deadline. | Start 2026-10-24; follow up through the sprint |
| Sahar Haidary; Bahara Noorzai; Ahmad Khalid Safi | Technical diagram comparison, business-rule review and traceability check, respectively. | 2026-10-29 |
| Bahara Noorzai; Sahar Haidary; Ahmad Khalid Safi | Acceptance decisions, technical walkthrough and minutes, respectively. | 2026-10-30 |

## Meeting Summary from the Script

Ahmad set the final sprint boundary and protected preparation time. Bahara prioritized the five administration/contact stories alongside integration and carry-over. Sahar outlined permissions, moderation visibility, category dependencies, mail failures and quality checks. The 13-point proposal remained conditional on availability. The team assigned the October 29 UML comparison, October 30 review and October 31 product/technical/process hand-off.
