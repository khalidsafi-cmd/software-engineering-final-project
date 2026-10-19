# Use Case Diagram

Status: IMPLEMENTED code baseline; model prepared for verification. Mermaid flowchart provides a use-case-style view; it is not strict UML actor notation.

```mermaid
flowchart LR
    V[Visitor]
    C[Customer]
    W[Worker / Ustaad]
    A[Admin]
    subgraph System[Ustaad.af]
        Browse([Browse jobs and workers])
        Auth([Register / login / manage account])
        Profile([Maintain worker profile])
        Job([Post / edit / cancel own open job])
        Apply([Apply / track own applications])
        Hire([Inspect applicants / select worker])
        Msg([Read / send participant messages])
        Complete([Complete assigned job])
        Review([Review counterpart after completion])
        Trust([Report / block / unblock])
        Moderate([Moderate users / jobs / reports / reviews])
        Categories([Manage categories])
        Contact([Send contact enquiry])
    end
    V --> Browse
    V --> Auth
    V --> Contact
    C --> Browse
    W --> Browse
    C --> Auth
    W --> Auth
    A --> Auth
    C --> Job
    C --> Hire
    W --> Profile
    W --> Apply
    C --> Msg
    W --> Msg
    C --> Complete
    C --> Review
    W --> Review
    C --> Trust
    W --> Trust
    A --> Moderate
    A --> Categories
```

Visitors discover jobs/workers, register/login and contact the platform. Customers manage their own open jobs, inspect applicants, select one worker, communicate and complete assigned work. Workers manage profiles, apply, track applications and communicate after selection. Both participants can review after completion and use reporting/blocking. Admins moderate users, jobs, reports/reviews and maintain categories. Public browsing remains available without authentication.

Role/status middleware and policies constrain use cases: active account and correct ownership/participation are required; public signup cannot grant admin. Reviews require completion; conversations relate to accepted applications. Admin is an existing role, not an additional Scrum team member. [Source routes](../../routes/web.php) · [requirements](../03-requirements/functional-requirements.md).
