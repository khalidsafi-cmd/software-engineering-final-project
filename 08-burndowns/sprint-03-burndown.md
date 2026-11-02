# Sprint 03 Burndown

Project: **Ustaad.af - Digital Marketplace for Skilled Workers**

Dates: **October 18-23, 2026** (6 scheduled calendar workdays)

Sprint goal: Verify private communication, completion, reviews and trust controls with security checks.

## Baseline and evidence basis

The [sprint backlog](../06-sprints/sprint-03/sprint-backlog.md) proposes **15 story points**. The [planning record](../07-meetings/sprint-planning/2026-10-18-sprint-planning.md) retains the proposal without establishing individual availability or a final capacity-backed commitment. **Final committed total is not established in the project records.** The proposed total supplies the chart baseline.

Daily records describe intended checks and scripted actions, not measured end-of-day balances. The [review record](../07-meetings/sprint-review/2026-10-23-sprint-review.md) leaves all five stories pending verification and records no accepted story. Therefore **0 points are credited as Done and 15 proposed points remain uncredited** in this reconciliation. This records documented acceptance; it does not claim that no work occurred.

## Story-point reconciliation

| Story | Proposed scope | Proposed points | Credited Done points | Uncredited points |
| --- | --- | ---: | ---: | ---: |
| US-11 | exchange messages with my selected worker | 5 | 0 | 5 |
| US-12 | mark an assigned job completed | 2 | 0 | 2 |
| US-13 | review my worker after completion | 3 | 0 | 3 |
| US-14 | report inappropriate users or content | 3 | 0 | 3 |
| US-15 | block or unblock another user | 2 | 0 | 2 |
| **Total** | **Five stories pending verification** | **15** | **0** | **15** |

Credit requires the [Definition of Done](../06-sprints/sprint-03/definition-of-done.md), including supporting verification and Bahara Noorzai's acceptance. Existing implementation, test-file presence, planned checks and partial functionality do not earn story points. Sahar Haidary owns technical evidence; Bahara owns acceptance; Ahmad maintains progress records.

## Daily burndown

Start-of-sprint ideal: **15 points**. For scheduled day d, ideal remaining = max(0, 15 * (1 - d / 6)), rounded to two decimals. All scheduled dates count, including weekends, matching the daily sprint schedule.

Uncredited proposed points = 15 minus documented accepted points. This reconstructed balance stays at 15 because the sources supply no dated Done decision. **Actual daily remaining-effort measurements are absent.** These balances must not be labeled measured actuals. Each date links to its stand-up; the final date also uses the review cited above.

| Date | Ideal remaining points | Uncredited proposed points | Recorded focus and evidence status |
| --- | ---: | ---: | --- |
| [2026-10-18](../07-meetings/daily-standups/2026-10-18-daily-standup.md) | 12.50 | 15 | Retain the 15-point proposal and hiring dependencies; prepare roles and assigned-job states. |
| [2026-10-19](../07-meetings/daily-standups/2026-10-19-daily-standup.md) | 10.00 | 15 | Plan messaging, read tracking, completion, mutual reviews, reports and blocking checks. |
| [2026-10-20](../07-meetings/daily-standups/2026-10-20-daily-standup.md) | 7.50 | 15 | Check outsider access, blocked pairs, throttling and invalid completion/review/report requests. |
| [2026-10-21](../07-meetings/daily-standups/2026-10-21-daily-standup.md) | 5.00 | 15 | Prioritize privacy; separate missing setup from defects and retain moderation dependencies. |
| [2026-10-22](../07-meetings/daily-standups/2026-10-22-daily-standup.md) | 2.50 | 15 | Compare messaging, completion and review rules with UML; organize evidence by actor and state. |
| [2026-10-23](../07-meetings/daily-standups/2026-10-23-daily-standup.md) | 0.00 | 15 | Scripted review retains all five stories pending verification; carry moderation dependencies into Sprint 4. |

## Burndown chart

First line: ideal remaining points. Second line: uncredited proposed points reconstructed from the records. Start is the baseline before the first workday. The table above provides the same data when Mermaid is unavailable.

```mermaid
xychart-beta
    title "Sprint 03: ideal and uncredited proposed points"
    x-axis ["Start", "Oct 18", "Oct 19", "Oct 20", "Oct 21", "Oct 22", "Oct 23"]
    y-axis "Story points" 0 --> 15
    line [15, 12.50, 10.00, 7.50, 5.00, 2.50, 0.00]
    line [15, 15, 15, 15, 15, 15, 15]
```

## Interpretation and close-out

The ideal reaches **0** on October 23; the acceptance reconciliation ends at **15 uncredited points**, a **15-point gap** against the proposed ideal. This identifies unresolved verification and acceptance. It does not establish 15 points of coding left or prove software failure. Actual velocity and commitment completion rate cannot be established without confirmed commitment and dated acceptance evidence.

No quantified scope addition, removal or re-estimation is recorded in the sources used here. The original proposed baseline is preserved. Earlier unresolved work remains a dependency and prioritization concern; it is not silently added to this sprint total or counted twice. Documentation, UML, integration and meeting tasks have no separate point allocation in this baseline.

Prioritize privacy and core-workflow gaps at October 24 planning; carry hidden-review/public-rating dependencies into administration and reserve integration time.

Any later correction requires dated story acceptance or a scope decision and a linked source. Preserve this baseline and the original daily record when recording that revision.
