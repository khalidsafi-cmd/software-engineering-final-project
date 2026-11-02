# Sprint 04 Review

## Sprint goal

Verify administration, integrate workflows, refine UX, finalize models and prepare submission evidence.

Dates: October 24–30, 2026

## Stories reviewed and acceptance criteria

| Story | Selected scope | Points | Acceptance criteria |
| --- | --- | --- | --- |
| US-16 | inspect and suspend or restore users | 3 | Only active admins access filtered/paginated users; valid active/suspended transitions work; administrator accounts cannot be suspended through this endpoint. |
| US-17 | inspect and cancel inappropriate jobs | 3 | Admin filters jobs and cancels only open/assigned jobs; pending applications are rejected and history preserved; non-admin writes fail. |
| US-18 | manage skill categories | 2 | Admin creates/updates valid categories with unique slugs and deletes unused categories; categories referenced by jobs or worker profiles cannot be deleted. |
| US-19 | resolve reports and hide or restore reviews | 3 | Admin marks reports reviewed/dismissed and hides/restores reviews; reported messages expose only reported content; non-admin access fails; hidden reviews are excluded from public ratings. |
| US-20 | send a contact enquiry | 2 | Valid enquiry sends to configured recipient with visitor reply-to; required/invalid fields fail; sixth request within rate-limit window is blocked; delivery failure returns safe feedback without false success. |

[Review meeting record](../07-meetings/sprint-review/2026-10-30-sprint-review.md) · [Sprint backlog](../06-sprints/sprint-04/sprint-backlog.md) · [Definition of Done](../06-sprints/sprint-04/definition-of-done.md)

Recording: No recording is linked in the review meeting record.

## Review summary

The review covers the five stories above against their acceptance criteria. Sahar Haidary presents the technical baseline, Bahara Noorzai owns acceptance decisions, and Ahmad Khalid Safi maintains review records. Existing implementation and test files are available, but completed story-specific execution results are absent. The source describes a scripted walkthrough; it does not establish completed runtime verification.

## Product Owner feedback

Bahara keeps incomplete stories and earlier carry-over visible. Sahar requires separate evidence for administrator reads and writes, customer versus administrator cancellation, both category-reference types and privacy effects of moderation. Contact results need mail configuration. Integration must follow post, apply, select, message, complete and review, with responsive checks at 360 and 1280 pixels, build results and performance measurements tied to environment/dataset.

## Acceptance decisions

**Accepted stories: none recorded.** All five stories remain pending verification. The following checks are required before acceptance:

| Story | Outcome | Evidence required for acceptance |
| --- | --- | --- |
| US-16 | Pending verification | Filtered/paginated active-admin user access, suspension/restoration, administrator-account protection and rejection of other roles. |
| US-17 | Pending verification | Admin cancellation of open/assigned jobs, rejected pending applications, preserved history and rejected states/non-admin writes. |
| US-18 | Pending verification | Category creation/update, unique slugs, unused deletion and prevention of deletion when jobs or worker profiles reference the category. |
| US-19 | Pending verification | Report reviewed/dismissed states, review hide/restore, limited reported-message visibility, non-admin rejection and public-rating effects. |
| US-20 | Pending verification | Configured mail recipient and visitor reply-to, invalid fields, sixth-request throttling and safe mail-failure feedback without false success. |

## Incomplete work

All five stories retain incomplete verification. No confirmed defect-based rejection or passing result is recorded. Sahar owns the remaining checks and separates unavailable setup, unexecuted verification and reproducible defects. Points remain uncredited until the Definition of Done and Product Owner acceptance are satisfied.

## Carry-over items

Retain US-16 through US-20 and earlier unresolved stories in the Product Backlog for final preparation. Integration, responsive observations, build evidence and performance measurements still require completed results. Bahara owns product records, Sahar owns technical artifacts, and Ahmad owns process records, access and submission preparation.

Bahara orders carry-over against product priorities. Unresolved work remains visible without automatically expanding another sprint's point commitment.

## Lessons learned

- Keep technical gaps separate from submission-evidence gaps.
- Tie performance measurements to the environment and dataset.
- Keep acceptance and carry-over consistent across product, technical and process records.

[Related retrospective](../07-meetings/retrospectives/2026-10-30-sprint-retrospective.md)

## Decisions and follow-up

- Retain pending acceptance until criterion-level evidence supports a Product Owner decision.
- Prioritize the carry-over above and retain reasons for scope changes.
- Keep incomplete work visible in tasks, review outcomes and progress records; reaching the sprint end does not satisfy Done.

| Owner | Follow-up responsibility |
| --- | --- |
| Sahar Haidary | Identify remaining checks and setup, attach results by story and document confirmed defects with actor and workflow-state details. |
| Bahara Noorzai | Maintain acceptance decisions, order carry-over and keep criteria and backlog status consistent. |
| Ahmad Khalid Safi | Link review records, tasks, recordings and progress notes; follow up on missing evidence and assigned actions. |
