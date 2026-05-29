# Refresh and Monitoring Checklist

Use this checklist before setting up, relying on, or reviewing recurring refreshes, pipeline runs, notebook runs, Dataflow Gen2 refreshes, or semantic model refreshes.

This checklist helps ensure that data remains current, refresh failures are noticed, and ownership is clear.

## 1. Basic Information

| Field                                 | Response                                                                                      |
| ------------------------------------- | --------------------------------------------------------------------------------------------- |
| Asset name                            |                                                                                               |
| Workspace                             |                                                                                               |
| Workspace type                        | Personal / Sandbox / Department / BIA Production                                              |
| Item type                             | Report / Semantic Model / Dataflow Gen2 / Pipeline / Notebook / Lakehouse / Warehouse / Other |
| Asset status                          | Sandbox / Draft / Prototype / UAT / Department / Production                                   |
| Business owner                        |                                                                                               |
| Technical owner                       |                                                                                               |
| Workspace owner                       |                                                                                               |
| Deputy workspace owner, if applicable |                                                                                               |
| Reviewer                              |                                                                                               |
| Review date                           |                                                                                               |

## 2. Workspace Context

| Workspace Type           | Refresh and Monitoring Expectation                                                                                                                     |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Personal Workspace       | Suitable only for private drafts and individual exploration. Do not create long-term shared refresh dependencies.                                      |
| Sandbox Workspace        | Refresh should be lightweight and used for learning or experimentation only. Avoid unnecessary scheduled refreshes.                                    |
| Department Workspace     | Refresh should have clear owner, deputy owner, connection ownership, and monitoring responsibility.                                                    |
| BIA Production Workspace | Refresh should be planned, monitored, supported, and managed as part of BIA production operations. Direct workspace access is restricted to BIA users. |

Confirm:

* [ ] The refresh setup matches the workspace purpose
* [ ] The asset is not using a personal workspace for shared or operational refresh
* [ ] Sandbox refresh is not being treated as production refresh
* [ ] Department workspace refresh has both owner and deputy owner awareness
* [ ] BIA Production Workspace access remains restricted to BIA users, where applicable

## 3. Refresh Requirement

* [ ] The asset requires refresh or recurring runs
* [ ] The reason for refresh is clear
* [ ] Users need updated data for a defined purpose
* [ ] The required data currency is understood
* [ ] The refresh frequency is justified
* [ ] The capacity impact has been considered
* [ ] The asset does not refresh more frequently than necessary
* [ ] The refresh requirement matches the asset status and workspace type

## 4. Data Source

| Field                                 | Response                                                                                           |
| ------------------------------------- | -------------------------------------------------------------------------------------------------- |
| Data source name                      |                                                                                                    |
| Data source type                      | File / Database / API / Lakehouse / Warehouse / SharePoint / OneDrive / On-premises source / Other |
| Data source owner                     |                                                                                                    |
| Data steward or subject matter expert |                                                                                                    |
| Source update frequency               |                                                                                                    |
| Source sensitivity                    | Confidential - SUSS / Restricted - SUSS / Unrestricted - SUSS / None / Unsure                      |
| Source approval confirmed?            | Yes / No / Unsure                                                                                  |

## 5. Connection and Credential

* [ ] Connection type is understood
* [ ] Connection owner is identified
* [ ] Credential or identity owner is identified
* [ ] Credential is not dependent on an unsuitable personal account
* [ ] Personal credentials are not used for long-term department or production-facing refresh
* [ ] Permissions to the source are appropriate
* [ ] Credential expiry or access removal risk has been considered
* [ ] Ownership transfer plan exists if the creator leaves or changes role
* [ ] Backup ownership is clear where department or production-facing refresh is involved

## 6. Gateway Requirement

| Question                              | Response          |
| ------------------------------------- | ----------------- |
| Is a gateway required?                | Yes / No / Unsure |
| Gateway name, if known                |                   |
| Gateway owner or support contact      |                   |
| Is the gateway online and available?  | Yes / No / Unsure |
| Is the gateway dependency documented? | Yes / No / Unsure |

## 7. Refresh Schedule

| Field                                                  | Response                                                    |
| ------------------------------------------------------ | ----------------------------------------------------------- |
| Refresh or run type                                    | Manual / Scheduled / Pipeline / Dataflow / Notebook / Other |
| Refresh frequency                                      |                                                             |
| Scheduled time                                         |                                                             |
| Expected duration                                      |                                                             |
| Time zone                                              |                                                             |
| Is the schedule aligned with source data availability? | Yes / No / Unsure                                           |
| Is the schedule aligned with user needs?               | Yes / No / Unsure                                           |

## 8. Monitoring

* [ ] Refresh or run history can be checked
* [ ] Monitoring owner is identified
* [ ] Backup monitoring owner is identified, where applicable
* [ ] Failure alerts or notifications are configured where appropriate
* [ ] Users can tell whether data is stale
* [ ] Refresh duration is monitored where relevant
* [ ] Repeated failures are reviewed
* [ ] Monitoring does not depend only on end users noticing stale data
* [ ] Monitoring responsibility is suitable for the workspace type and asset status

## 9. Failure Handling

| Question                                               | Response                                                                             |
| ------------------------------------------------------ | ------------------------------------------------------------------------------------ |
| Who checks refresh failures?                           |                                                                                      |
| Who fixes connection or credential issues?             |                                                                                      |
| Who checks source system issues?                       |                                                                                      |
| Who checks gateway issues?                             |                                                                                      |
| Who communicates with users if data is stale?          |                                                                                      |
| Who is the backup contact if the owner is unavailable? |                                                                                      |
| Escalation route                                       | BIA / IT / Vendor / Department owner / Deputy workspace owner / Source owner / Other |

## 10. Common Failure Risks

Review whether any of these risks apply.

* [ ] Source file may be moved, renamed, or replaced
* [ ] Source schema may change
* [ ] Columns may be renamed, removed, or added
* [ ] Credentials may expire
* [ ] Gateway may become unavailable
* [ ] Source system permissions may change
* [ ] Pipeline, notebook, or dataflow logic may break
* [ ] Refresh may consume too much capacity
* [ ] Original creator may leave or change role
* [ ] Department workspace owner or deputy owner may change
* [ ] Users may continue using stale data without noticing

## 11. Documentation

* [ ] Data source is documented
* [ ] Connection owner is documented
* [ ] Credential owner is documented
* [ ] Gateway dependency is documented, if applicable
* [ ] Refresh schedule is documented
* [ ] Monitoring owner is documented
* [ ] Backup owner or deputy owner is documented, where applicable
* [ ] Escalation route is documented
* [ ] Known failure risks are documented

## 12. Review Decision

| Decision Area                | Response                    |
| ---------------------------- | --------------------------- |
| Refresh setup is acceptable? | Yes / No / Yes with caveats |
| Main caveats                 |                             |
| Required changes             |                             |
| Reviewer                     |                             |
| Follow-up owner              |                             |
| Target date                  |                             |

## 13. Final Checklist

* [ ] Refresh requirement is justified
* [ ] Workspace type and asset status are clear
* [ ] Data source and owner are known
* [ ] Connection and credential ownership are clear
* [ ] Personal credentials are not used for long-term department or production-facing refresh
* [ ] Gateway requirement is checked
* [ ] Refresh schedule is appropriate
* [ ] Monitoring owner is assigned
* [ ] Backup owner or deputy owner is identified, where applicable
* [ ] Failure handling route is clear
* [ ] Users can identify stale data
* [ ] Documentation is available
* [ ] Review decision is documented
* [ ] BIA Production Workspace access remains restricted to BIA users, where applicable
