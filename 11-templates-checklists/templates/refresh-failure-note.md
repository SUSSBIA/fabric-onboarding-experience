# Refresh Failure Note

Use this template when reporting or documenting a refresh, connection, gateway, pipeline, notebook, semantic model, or dataflow failure.

This is especially useful for workspace owners, report developers, data engineers, department representatives, and users escalating an issue to BIA, IT, a vendor, or a data source owner.

## 1. Failure Summary

| Field                          | Response                                                                                      |
| ------------------------------ | --------------------------------------------------------------------------------------------- |
| Asset name                     |                                                                                               |
| Workspace                      |                                                                                               |
| Item type                      | Report / Semantic Model / Dataflow Gen2 / Pipeline / Notebook / Lakehouse / Warehouse / Other |
| Owner                          |                                                                                               |
| Reported by                    |                                                                                               |
| Failure date and time          |                                                                                               |
| Last successful refresh or run |                                                                                               |
| Issue status                   | New / Investigating / Resolved / Escalated / Monitoring                                       |
| Business impact                | Low / Medium / High / Unsure                                                                  |

## 2. Data Source and Connection

| Field                       | Response                                                                                           |
| --------------------------- | -------------------------------------------------------------------------------------------------- |
| Data source name            |                                                                                                    |
| Data source type            | File / Database / API / Lakehouse / Warehouse / SharePoint / OneDrive / On-premises source / Other |
| Source owner                |                                                                                                    |
| Connection owner            |                                                                                                    |
| Credential or identity used | Personal credential / Shared credential / Workspace identity / Service account / Unsure            |
| Gateway required?           | Yes / No / Unsure                                                                                  |
| Gateway name, if known      |                                                                                                    |

## 3. Refresh or Run Details

| Field                      | Response                                                    |
| -------------------------- | ----------------------------------------------------------- |
| Refresh or run type        | Manual / Scheduled / Pipeline / Dataflow / Notebook / Other |
| Refresh frequency          |                                                             |
| Expected refresh time      |                                                             |
| Actual failure time        |                                                             |
| Duration before failure    |                                                             |
| Number of failed attempts  |                                                             |
| Is this a recurring issue? | Yes / No / Unsure                                           |

## 4. Error Message

| Field                                               | Response |
| --------------------------------------------------- | -------- |
| Error message shown                                 |          |
| Error code, if any                                  |          |
| Screenshot available?                               | Yes / No |
| Link to failed run or refresh history, if available |          |

## 5. Recent Changes

| Question                                                                         | Response          |
| -------------------------------------------------------------------------------- | ----------------- |
| Was the source file moved, renamed, or replaced?                                 | Yes / No / Unsure |
| Did the source schema change?                                                    | Yes / No / Unsure |
| Were columns renamed, removed, or added?                                         | Yes / No / Unsure |
| Did credentials change or expire?                                                | Yes / No / Unsure |
| Did workspace access or permissions change?                                      | Yes / No / Unsure |
| Did the gateway status change?                                                   | Yes / No / Unsure |
| Was the report, semantic model, pipeline, notebook, or dataflow recently edited? | Yes / No / Unsure |

## 6. Initial Checks Completed

| Check                                                         | Response                  |
| ------------------------------------------------------------- | ------------------------- |
| Confirmed asset name and workspace                            | Yes / No                  |
| Checked refresh or run history                                | Yes / No                  |
| Checked error message                                         | Yes / No                  |
| Checked whether data source is available                      | Yes / No / Not applicable |
| Checked whether credentials are still valid                   | Yes / No / Not applicable |
| Checked whether gateway is online                             | Yes / No / Not applicable |
| Checked whether source schema changed                         | Yes / No / Not applicable |
| Checked whether capacity or performance issue may be involved | Yes / No / Unsure         |

## 7. Impact

| Question                                                 | Response          |
| -------------------------------------------------------- | ----------------- |
| Who is affected?                                         |                   |
| Which reports or downstream assets are affected?         |                   |
| Are users currently relying on stale data?               | Yes / No / Unsure |
| Is this used for official reporting or decision support? | Yes / No / Unsure |
| Is communication to users needed?                        | Yes / No / Unsure |

## 8. Escalation

| Field                                      | Response                                                           |
| ------------------------------------------ | ------------------------------------------------------------------ |
| Escalation needed?                         | Yes / No / Unsure                                                  |
| Escalation route                           | BIA / IT / Vendor / Department owner / Source system owner / Other |
| Reason for escalation                      |                                                                    |
| Information still needed before escalation |                                                                    |
| Person or team contacted                   |                                                                    |
| Date escalated                             |                                                                    |

## 9. Resolution

| Field                        | Response          |
| ---------------------------- | ----------------- |
| Root cause, if known         |                   |
| Resolution action taken      |                   |
| Resolved by                  |                   |
| Resolution date and time     |                   |
| Follow-up monitoring needed? | Yes / No / Unsure |
| Preventive action needed?    | Yes / No / Unsure |

## 10. Follow-Up Actions

| Action | Owner | Target Date | Status                           |
| ------ | ----- | ----------- | -------------------------------- |
|        |       |             | Not started / In progress / Done |
|        |       |             | Not started / In progress / Done |
|        |       |             | Not started / In progress / Done |

## 11. Notes

| Area                  | Response |
| --------------------- | -------- |
| Additional notes      |          |
| Recommended next step |          |
| Follow-up owner       |          |
| Follow-up date        |          |
