# Non-Functional Requirements

These are testable quality requirements, not claims that measurements have been achieved.

| ID | Area | Requirement | Status | Verification |
| --- | --- | --- | --- | --- |
| NFR-01 | Security | Unauthorized roles, outsiders and suspended actors must be denied protected marketplace operations; passwords/private fields must not appear in public props. | IMPLEMENTED controls; verification PLANNED | ProfileAuthorizationTest.php and ModerationTest.php; inspect public props |
| NFR-02 | Integrity | Hiring must leave exactly one accepted application and consistent assigned job/conversation; failed transaction must roll back. | IMPLEMENTED controls; verification PLANNED | JobMarketplaceTest.php rollback and duplicate-selection checks |
| NFR-03 | Privacy | Only conversation participants access history; moderators receive only the reported message rather than unrelated conversation history. | IMPLEMENTED controls; verification PLANNED | CommunicationTest.php and ModerationTest.php |
| NFR-04 | Usability | Core browse/post/apply/hire/message flows must be usable at 360 px and 1280 px widths with readable labels, errors and empty states. | PLANNED verification; no accessibility certification claimed | Manual browser checklist with device width, route and screenshots |
| NFR-05 | Performance | Public/admin lists must remain paginated; public job/worker query relations must be eager loaded. Response-time target: p95 under 2 seconds across 30 requests on a documented test dataset/environment. | IMPLEMENTED pagination; performance target PLANNED | PublicWebsiteTest.php pagination plus measured timings; record dataset and environment |
| NFR-06 | Reliability | Invalid forms and mail failures must not create false success; duplicate applications/reviews must be rejected. | IMPLEMENTED controls; verification PLANNED | JobMarketplaceTest.php, CompletionReviewTest.php and ContactTest.php |
| NFR-07 | Maintainability | Changed behavior must have meaningful regression coverage; final verification must record command, environment, date and actual result. | PLANNED assignment quality gate | Affected Pest tests; npm run build; record failures and fixes |
| NFR-08 | Repository hygiene | Submission must contain no committed .env/credentials, no fabricated evidence and no broken internal documentation links. | PLANNED final verification | Tracked-file/secrets inspection and documentation link check |
