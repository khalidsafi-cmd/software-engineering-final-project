# Sprint 02 Burndown

Project: **Ustaad.af - Digital Marketplace for Skilled Workers**

Dates: **October 12-17, 2026** (6 scheduled calendar workdays)

Sprint goal: Verify the complete job, application and worker-selection workflow and resolve evidenced defects.

## Baseline and evidence basis

The [sprint backlog](../06-sprints/sprint-02/sprint-backlog.md) proposes **16 story points**. The [planning record](../07-meetings/sprint-planning/2026-10-12-sprint-planning.md) retains the proposal without establishing individual availability or a final capacity-backed commitment. **Final committed total is not established in the project records.** The proposed total supplies the chart baseline.

Daily records describe intended checks and scripted actions, not measured end-of-day balances. The [review record](../07-meetings/sprint-review/2026-10-17-sprint-review.md) leaves all five stories pending verification and records no accepted story. Therefore **0 points are credited as Done and 16 proposed points remain uncredited** in this reconciliation. This records documented acceptance; it does not claim that no work occurred.

## Story-point reconciliation

| Story | Proposed scope | Proposed points | Credited Done points | Uncredited points |
| --- | --- | ---: | ---: | ---: |
| US-06 | post a categorized job | 3 | 0 | 3 |
| US-07 | edit or cancel my open job | 3 | 0 | 3 |
| US-08 | apply to an open job | 3 | 0 | 3 |
| US-09 | track my applications | 2 | 0 | 2 |
| US-10 | inspect applicants and hire one worker | 5 | 0 | 5 |
| **Total** | **Five stories pending verification** | **16** | **0** | **16** |

Credit requires the [Definition of Done](../06-sprints/sprint-02/definition-of-done.md), including supporting verification and Bahara Noorzai's acceptance. Existing implementation, test-file presence, planned checks and partial functionality do not earn story points. Sahar Haidary owns technical evidence; Bahara owns acceptance; Ahmad maintains progress records.

## Daily burndown

Start-of-sprint ideal: **16 points**. For scheduled day d, ideal remaining = max(0, 16 * (1 - d / 6)), rounded to two decimals. All scheduled dates count, including weekends, matching the daily sprint schedule.

Uncredited proposed points = 16 minus documented accepted points. This reconstructed balance stays at 16 because the sources supply no dated Done decision. **Actual daily remaining-effort measurements are absent.** These balances must not be labeled measured actuals. Each date links to its stand-up; the final date also uses the review cited above.

| Date | Ideal remaining points | Uncredited proposed points | Recorded focus and evidence status |
| --- | ---: | ---: | --- |
| [2026-10-12](../07-meetings/daily-standups/2026-10-12-daily-standup.md) | 13.33 | 16 | Retain the 16-point proposal and account dependencies; prepare role-specific data. |
| [2026-10-13](../07-meetings/daily-standups/2026-10-13-daily-standup.md) | 10.67 | 16 | Plan posting, editing, applications, private lists and selection checks by story. |
| [2026-10-14](../07-meetings/daily-standups/2026-10-14-daily-standup.md) | 8.00 | 16 | Check ownership, duplicates, closed jobs, repeated selection and rollback; no failure is established. |
| [2026-10-15](../07-meetings/daily-standups/2026-10-15-daily-standup.md) | 5.33 | 16 | Prioritize hiring consistency and authorization; partial functionality does not complete a story. |
| [2026-10-16](../07-meetings/daily-standups/2026-10-16-daily-standup.md) | 2.67 | 16 | Compare post/apply/select diagrams with authorization and transactional conversation creation. |
| [2026-10-17](../07-meetings/daily-standups/2026-10-17-daily-standup.md) | 0.00 | 16 | Review retains all five stories pending verification; assignment evidence remains a messaging dependency. |

## Burndown chart

First line: ideal remaining points. Second line: uncredited proposed points reconstructed from the records. Start is the baseline before the first workday. The table above provides the same data when Mermaid is unavailable.

```mermaid
xychart-beta
    title "Sprint 02: ideal and uncredited proposed points"
    x-axis ["Start", "Oct 12", "Oct 13", "Oct 14", "Oct 15", "Oct 16", "Oct 17"]
    y-axis "Story points" 0 --> 16
    line [16, 13.33, 10.67, 8.00, 5.33, 2.67, 0.00]
    line [16, 16, 16, 16, 16, 16, 16]
```

## Interpretation and close-out

The ideal reaches **0** on October 17; the acceptance reconciliation ends at **16 uncredited points**, a **16-point gap** against the proposed ideal. This identifies unresolved verification and acceptance. It does not establish 16 points of coding left or prove software failure. Actual velocity and commitment completion rate cannot be established without confirmed commitment and dated acceptance evidence.

No quantified scope addition, removal or re-estimation is recorded in the sources used here. The original proposed baseline is preserved. Earlier unresolved work remains a dependency and prioritization concern; it is not silently added to this sprint total or counted twice. Documentation, UML, integration and meeting tasks have no separate point allocation in this baseline.

Prioritize hiring consistency and application privacy at October 18 planning; retain assignment and accepted-application dependencies for messaging.

Any later correction requires dated story acceptance or a scope decision and a linked source. Preserve this baseline and the original daily record when recording that revision.
