# Software Requirements Specification

## 1. Introduction

Ustaad.af connects customers in Afghanistan with skilled blue-collar workers. This specification documents the inspected repository baseline and proposed assignment verification.

## 2. Purpose

Provide a shared, testable contract for the three-person Scrum team, Product Owner review and academic evidence collection.

## 3. Scope

Public jobs/workers, accounts, worker profiles, customer jobs, applications/hiring, private messages, completion, mutual reviews, reports/blocks, administrative users/jobs/categories/reports/reviews and contact enquiries are present in code. Online payments, escrow, real-time sockets, mobile applications and certified identity verification are outside this assignment baseline.

## 4. User types

Visitor: public discovery and registration/contact. Customer: requests work, selects workers and completes jobs. Worker/Ustaad: manages skills, applies and communicates. Admin: moderates the marketplace. Customer and selected worker both may review the counterpart after completion.

## 5. Assumptions

Inspection baseline: 2026-10-06, Git HEAD `405b1da`. Code and existing tests indicate implementation; tests have not been run as part of this documentation task. Repository history includes marketplace work before October (e.g. `2a3fe64`, September 24, messaging/admin). No historical contribution is attributed to a team member from their Scrum role. Deployment availability, mail delivery configuration and instructor requirements need human confirmation.

## 6. Functional Requirements

See [FR-01–FR-20](functional-requirements.md) and [exactly 20 stories](user-stories.md). IMPLEMENTED means present in the inspected code. PLANNED means future assignment work. IN PROGRESS requires a dated actual update; no feature is currently asserted IN PROGRESS without evidence.

## 7. Non-Functional Requirements

See [NFR-01–NFR-08](non-functional-requirements.md). Quality targets and manual checks remain pending until measured.

## 8. Constraints

Laravel 12 and the existing application structure/dependencies must be preserved. Three actual members serve roles despite the assignment template referencing 4–5 members; instructor approval has not been claimed. Four fixed sprint ranges precede November 1, 2026 at 11:59 PM. All assignment documentation stays in this directory. No fabricated meetings, outcomes or evidence are permitted.

## 9. Acceptance overview

Sahar demonstrates behavior and failure modes; Ahmad maintains traceability and evidence; Bahara accepts or rejects stories using their criteria in the real review. Existing code does not imply acceptance. Documentation-only tasks require accurate sources, readable Markdown and working links. Definition of Done and actual results remain separate from the plan.

## Requirements Traceability

| Functional Requirement | User Story | Sprint | Test / verification approach |
| --- | --- | --- | --- |
| FR-01 | US-01 | 1 | [tests/Feature/PublicWebsiteTest.php](../../tests/Feature/PublicWebsiteTest.php); demonstrate acceptance criteria and failure paths |
| FR-02 | US-02 | 1 | [tests/Feature/PublicWebsiteTest.php](../../tests/Feature/PublicWebsiteTest.php); demonstrate acceptance criteria and failure paths |
| FR-03 | US-03 | 1 | [tests/Feature/ProfileAuthorizationTest.php](../../tests/Feature/ProfileAuthorizationTest.php); demonstrate acceptance criteria and failure paths |
| FR-04 | US-04 | 1 | [tests/Feature/Auth/AuthenticationTest.php](../../tests/Feature/Auth/AuthenticationTest.php); demonstrate acceptance criteria and failure paths |
| FR-05 | US-05 | 1 | [tests/Feature/ProfileAuthorizationTest.php](../../tests/Feature/ProfileAuthorizationTest.php); demonstrate acceptance criteria and failure paths |
| FR-06 | US-06 | 2 | [tests/Feature/JobMarketplaceTest.php](../../tests/Feature/JobMarketplaceTest.php); demonstrate acceptance criteria and failure paths |
| FR-07 | US-07 | 2 | [tests/Feature/JobMarketplaceTest.php](../../tests/Feature/JobMarketplaceTest.php); demonstrate acceptance criteria and failure paths |
| FR-08 | US-08 | 2 | [tests/Feature/JobMarketplaceTest.php](../../tests/Feature/JobMarketplaceTest.php); demonstrate acceptance criteria and failure paths |
| FR-09 | US-09 | 2 | [tests/Feature/JobMarketplaceTest.php](../../tests/Feature/JobMarketplaceTest.php); demonstrate acceptance criteria and failure paths |
| FR-10 | US-10 | 2 | [tests/Feature/JobMarketplaceTest.php](../../tests/Feature/JobMarketplaceTest.php); demonstrate acceptance criteria and failure paths |
| FR-11 | US-11 | 3 | [tests/Feature/CommunicationTest.php](../../tests/Feature/CommunicationTest.php); demonstrate acceptance criteria and failure paths |
| FR-12 | US-12 | 3 | [tests/Feature/CompletionReviewTest.php](../../tests/Feature/CompletionReviewTest.php); demonstrate acceptance criteria and failure paths |
| FR-13 | US-13 | 3 | [tests/Feature/CompletionReviewTest.php](../../tests/Feature/CompletionReviewTest.php); demonstrate acceptance criteria and failure paths |
| FR-14 | US-14 | 3 | [tests/Feature/ModerationTest.php](../../tests/Feature/ModerationTest.php); demonstrate acceptance criteria and failure paths |
| FR-15 | US-15 | 3 | [tests/Feature/ModerationTest.php](../../tests/Feature/ModerationTest.php); demonstrate acceptance criteria and failure paths |
| FR-16 | US-16 | 4 | [tests/Feature/ModerationTest.php](../../tests/Feature/ModerationTest.php); demonstrate acceptance criteria and failure paths |
| FR-17 | US-17 | 4 | [tests/Feature/ModerationTest.php](../../tests/Feature/ModerationTest.php); demonstrate acceptance criteria and failure paths |
| FR-18 | US-18 | 4 | [tests/Feature/ModerationTest.php](../../tests/Feature/ModerationTest.php); demonstrate acceptance criteria and failure paths |
| FR-19 | US-19 | 4 | [tests/Feature/ModerationTest.php](../../tests/Feature/ModerationTest.php); demonstrate acceptance criteria and failure paths |
| FR-20 | US-20 | 4 | [tests/Feature/ContactTest.php](../../tests/Feature/ContactTest.php); demonstrate acceptance criteria and failure paths |

NFR verification is shared across all sprints; Sprint 4 consolidates evidence. Actual verification results: TO BE UPDATED DURING SPRINT.
