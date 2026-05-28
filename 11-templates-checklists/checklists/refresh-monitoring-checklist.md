# Refresh and Monitoring Checklist

Use this checklist before setting up, relying on, or reviewing recurring refreshes, pipeline runs, notebook runs, Dataflow Gen2 refreshes, or semantic model refreshes.

This checklist helps ensure that data remains current, refresh failures are noticed, and ownership is clear.

## 1. Basic Information

| Field | Response |
|---|---|
| Asset name |  |
| Workspace |  |
| Item type | Report / Semantic Model / Dataflow Gen2 / Pipeline / Notebook / Lakehouse / Warehouse / Other |
| Owner |  |
| Reviewer |  |
| Review date |  |
| Asset status | Sandbox / Draft / Prototype / UAT / Department / Production |

## 2. Refresh Requirement

- [ ] The asset requires refresh or recurring runs
- [ ] The reason for refresh is clear
- [ ] Users need updated data for a defined purpose
- [ ] The required data currency is understood
- [ ] The refresh frequency is justified
- [ ] The capacity impact has been considered
- [ ] The asset does not refresh more frequently than necessary

## 3. Data Source

| Field | Response |
|---|---|
| Data source name |  |
| Data source type | File / Database / API / Lakehouse / Warehouse / SharePoint / OneDrive / On-premises source / Other |
| Data source owner |  |
| Data steward or subject matter expert |  |
| Source update frequency |  |
| Source sensitivity | Confidential - SUSS / Restricted - SUSS / Unrestricted - SUSS / None / Unsure |
| Source approval confirmed? | Yes / No / Unsure |

## 4. Connection and Credential

- [ ] Connection type is understood
- [ ] Connection owner is identified
- [ ] Credential or identity owner is identified
- [ ] Credential is not dependent on an unsuitable personal account
- [ ] Permissions to the source are appropriate
- [ ] Credential expiry or access removal risk has been considered
- [ ] Ownership transfer plan exists if the creator leaves or changes role

## 5. Gateway Requirement

| Question | Response |
|---|---|
| Is a gateway required? | Yes / No / Unsure |
| Gateway name, if known |  |
| Gateway owner or support contact |  |
| Is the gateway online and available? | Yes / No / Unsure |
| Is the gateway dependency documented? | Yes / No / Unsure |

## 6. Refresh Schedule

| Field | Response |
|---|---|
| Refresh or run type | Manual / Scheduled / Pipeline / Dataflow / Notebook / Other |
| Refresh frequency |  |
| Scheduled time |  |
| Expected duration |  |
| Time zone |  |
| Is the schedule aligned with source data availability? | Yes / No / Unsure |
| Is the schedule aligned with user needs? | Yes / No / Unsure |

## 7. Monitoring

- [ ] Refresh or run history can be checked
- [ ] Monitoring owner is identified
- [ ] Failure alerts or notifications are configured where appropriate
- [ ] Users can tell whether data is stale
- [ ] Refresh duration is monitored where relevant
- [ ] Repeated failures are reviewed
- [ ] Monitoring does not depend only on end users noticing stale data

## 8. Failure Handling

| Question | Response |
|---|---|
| Who checks refresh failures? |  |
| Who fixes connection or credential issues? |  |
| Who checks source system issues? |  |
| Who checks gateway issues? |  |
| Who communicates with users if data is stale? |  |
| Escalation route | BIA / IT / Vendor / Department owner / Source owner / Other |

## 9. Common Failure Risks

Review whether any of these risks apply.

- [ ] Source file may be moved, renamed, or replaced
- [ ] Source schema may change
- [ ] Columns may be renamed, removed, or added
- [ ] Credentials may expire
- [ ] Gateway may become unavailable
- [ ] Source system permissions may change
- [ ] Pipeline, notebook, or dataflow logic may break
- [ ] Refresh may consume too much capacity
- [ ] Original creator may leave or change role
- [ ] Users may continue using stale data without noticing

## 10. Documentation

- [ ] Data source is documented
- [ ] Connection owner is documented
- [ ] Credential owner is documented
- [ ] Gateway dependency is documented, if applicable
- [ ] Refresh schedule is documented
- [ ] Monitoring owner is documented
- [ ] Escalation route is documented
- [ ] Known failure risks are documented

## 11. Review Decision

| Decision Area | Response |
|---|---|
| Refresh setup is acceptable? | Yes / No / Yes with caveats |
| Main caveats |  |
| Required changes |  |
| Reviewer |  |
| Follow-up owner |  |
| Target date |  |

## 12. Final Checklist

- [ ] Refresh requirement is justified
- [ ] Data source and owner are known
- [ ] Connection and credential ownership are clear
- [ ] Gateway requirement is checked
- [ ] Refresh schedule is appropriate
- [ ] Monitoring owner is assigned
- [ ] Failure handling route is clear
- [ ] Users can identify stale data
- [ ] Documentation is available
- [ ] Review decision is documented
