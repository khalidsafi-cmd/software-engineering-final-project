# Sprint 01 Review

## Sprint goal

Verify requirements, architecture, public discovery, authentication and worker profiles; establish Scrum documentation.

Dates: October 6–11, 2026

## Stories reviewed and acceptance criteria

| Story | Selected scope | Points | Acceptance criteria |
| --- | --- | --- | --- |
| US-01 | browse and filter public jobs | 3 | Open jobs of active customers appear; keyword/category/location filters combine; pagination retains filters; empty results and missing records are handled. |
| US-02 | discover workers and view public profiles | 3 | Only active worker profiles appear; filters combine; profiles expose skills and real visible-review averages without private account fields. |
| US-03 | register as a customer or worker | 3 | Valid customer/worker registration succeeds; worker profile is created; admin/invalid role injection is rejected; duplicate identity fields are validated. |
| US-04 | log in and manage account credentials | 3 | Valid login and logout work; invalid credentials fail; reset tokens and email verification are checked with their existing Auth tests; profile changes preserve protected fields. |
| US-05 | maintain my skills and worker profile | 3 | Own bio, experience, location, availability, trades and valid photo can be updated; invalid trades/uploads fail; other roles and suspended workers cannot edit. |

[Review meeting record](../07-meetings/sprint-review/2026-10-11-sprint-review.md) · [Sprint backlog](../06-sprints/sprint-01/sprint-backlog.md) · [Definition of Done](../06-sprints/sprint-01/definition-of-done.md)

Recording: [Sprint review recording](https://drive.google.com/file/d/1JV8ylYkiOl9XLxBIFxd2mkFtwCiVVg2a/view?usp=drive_link).

## Review summary

The review covers the five stories above against their acceptance criteria. Sahar Haidary presents the technical baseline, Bahara Noorzai owns acceptance decisions, and Ahmad Khalid Safi maintains review records. Existing implementation and test files are available, but completed story-specific execution results are absent.

## Product Owner feedback

Bahara requires separate evidence for each discovery and account story. A successful login does not establish reset-token, verification-email or profile-field behavior. Public browsing remains available without login, while private data and protected roles remain restricted. Sahar distinguishes missing checks from confirmed defects so each item has the correct next step.

## Acceptance decisions

**Accepted stories: none recorded.** All five stories remain pending verification. The following checks are required before acceptance:

| Story | Outcome | Evidence required for acceptance |
| --- | --- | --- |
| US-01 | Pending verification | Combined job filters, retained pagination, empty/missing results and open jobs from active customers. |
| US-02 | Pending verification | Active-worker discovery, combined filters, visible-review averages and exclusion of private account data. |
| US-03 | Pending verification | Customer/worker registration, automatic worker profile, invalid/admin-role rejection and duplicate identity validation. |
| US-04 | Pending verification | Login/logout, invalid credentials, reset tokens, email verification and protected account fields. |
| US-05 | Pending verification | Own-profile updates, valid trades/photos and rejection of invalid uploads, other roles and suspended workers. |

## Incomplete work

All five stories retain incomplete verification. No confirmed defect-based rejection or passing result is recorded. Sahar owns the remaining checks and separates unavailable setup, unexecuted verification and reproducible defects. Points remain uncredited until the Definition of Done and Product Owner acceptance are satisfied.

## Carry-over items

Compare US-01 through US-05 with Sprint 2 job-workflow priorities. Discovery, registration, credentials and profile verification remain incomplete; account checks also support the later customer-worker workflow.

Bahara orders carry-over against product priorities. Unresolved work remains visible without automatically expanding another sprint's point commitment.

## Lessons learned

- Prepare customer and worker accounts before verification.
- Keep discovery, credentials and profile checks separate so each acceptance criterion has evidence.
- Distinguish missing setup from defects using the actor, request and expected result.

[Related retrospective](../07-meetings/retrospectives/2026-10-11-sprint-retrospective.md)

## Decisions and follow-up

- Retain pending acceptance until criterion-level evidence supports a Product Owner decision.
- Prioritize the carry-over above and retain reasons for scope changes.
- Keep incomplete work visible in tasks, review outcomes and progress records; reaching the sprint end does not satisfy Done.

| Owner | Follow-up responsibility |
| --- | --- |
| Sahar Haidary | Identify remaining checks and setup, attach results by story and document confirmed defects with actor and workflow-state details. |
| Bahara Noorzai | Maintain acceptance decisions, order carry-over and keep criteria and backlog status consistent. |
| Ahmad Khalid Safi | Link review records, tasks, recordings and progress notes; follow up on missing evidence and assigned actions. |
