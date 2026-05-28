# Productionisation Readiness Checklist

Use this checklist before moving a Fabric asset beyond sandbox or department experimentation.

Productionisation means preparing an asset for formal, wider-facing, monitored, or BIA-managed production use. A report, semantic model, Lakehouse, pipeline, notebook, or dashboard that works once in sandbox is not automatically production-ready.

## 1. Basic Information

| Field | Response |
|---|---|
| Asset name |  |
| Workspace |  |
| Asset type | Report / Semantic Model / Lakehouse / Warehouse / Notebook / Pipeline / Dataflow Gen2 / Dashboard / Other |
| Current status | Sandbox / Draft / Prototype / UAT / Department / Production candidate |
| Proposed status | Department working asset / BIA production asset / Other |
| Business owner |  |
| Technical owner |  |
| Reviewer |  |
| Review date |  |

## 2. Business Purpose

- [ ] The business purpose is clearly documented
- [ ] The intended audience is known
- [ ] The decision, process, or monitoring need is clear
- [ ] The asset is needed beyond learning or experimentation
- [ ] The expected output is clear
- [ ] The asset does not duplicate an existing approved asset unnecessarily

## 3. Ownership

- [ ] Business owner is identified
- [ ] Technical owner is identified
- [ ] Data owner is identified
- [ ] Data steward or subject matter expert is identified, if applicable
- [ ] Support contact is identified
- [ ] Escalation route is identified
- [ ] Ownership will not depend only on the original creator

## 4. Data Source and Approval

- [ ] Data source is identified
- [ ] Data source owner is known
- [ ] Data use is approved for the intended purpose
- [ ] Data quality has been reviewed
- [ ] Data limitations are documented
- [ ] Source update frequency is understood
- [ ] Source system dependencies are understood

## 5. Sensitivity, Access and Sharing

- [ ] Sensitivity label is applied where needed
- [ ] Intended audience is documented
- [ ] Users who should not have access are considered
- [ ] Workspace roles are appropriate
- [ ] Item permissions are appropriate
- [ ] Sharing permissions are appropriate
- [ ] Export expectations are clear
- [ ] Screenshot or onward-sharing risks are considered
- [ ] External collaborator access is reviewed, if applicable

## 6. Row-Level Security

- [ ] RLS requirement has been assessed
- [ ] RLS logic is documented, if required
- [ ] User mapping is available, if required
- [ ] Positive testing is completed, if required
- [ ] Negative testing is completed, if required
- [ ] Data owner or business owner has reviewed RLS behaviour, if required
- [ ] RLS caveats are documented, if applicable

## 7. Semantic Model and Definitions

- [ ] Semantic model purpose is clear, if applicable
- [ ] Table grain is documented
- [ ] Key fields are defined
- [ ] Key measures are clearly named
- [ ] Key measures are defined
- [ ] KPI definitions are documented
- [ ] Relationships are reviewed
- [ ] Reuse opportunities are considered
- [ ] Duplicated or conflicting definitions are avoided

## 8. Report or Output Validation

- [ ] Key outputs have been validated against source or expected values
- [ ] Totals, counts, averages, percentages, or model outputs behave as expected
- [ ] Filters and slicers have been tested
- [ ] Visual interactions have been tested
- [ ] Caveats are visible
- [ ] Business owner or subject matter expert has reviewed the output
- [ ] Known issues are documented
- [ ] Users are warned where interpretation requires caution

## 9. Refresh and Operations

- [ ] Refresh requirement is confirmed
- [ ] Refresh frequency is justified
- [ ] Connection owner is identified
- [ ] Credential owner is identified
- [ ] Gateway dependency is known, if applicable
- [ ] Monitoring owner is assigned
- [ ] Failure escalation route is documented
- [ ] Users can identify stale data
- [ ] Capacity impact has been considered
- [ ] Operational support expectations are clear

## 10. Lifecycle and Release

- [ ] Asset status is clear
- [ ] Release notes are prepared, if needed
- [ ] Change history is documented, if needed
- [ ] Deployment approach is agreed
- [ ] Git integration or deployment pipeline need is assessed
- [ ] User communication is prepared, if needed
- [ ] Retirement or replacement of older assets is considered

## 11. BIA Review

- [ ] BIA review is required if the asset is production-facing
- [ ] BIA review is required if the asset enters BIA production workspace
- [ ] BIA review is required if tenant-level settings are involved
- [ ] BIA review is required if capacity-heavy workloads are involved
- [ ] BIA review is required if external collaborators are involved
- [ ] BIA review is required if access, sensitivity, or RLS risks are unclear

## 12. Readiness Decision

| Decision Area | Response |
|---|---|
| Productionisation readiness | Ready / Ready with caveats / Not ready / Keep as department asset / Keep as sandbox |
| Main reasons |  |
| Required fixes |  |
| Approval or reviewer |  |
| Follow-up owner |  |
| Target date |  |

## 13. Final Checklist

- [ ] Business purpose is documented
- [ ] Business owner is identified
- [ ] Data owner or subject matter expert is identified
- [ ] Data source is approved
- [ ] Sensitivity label is applied where needed
- [ ] Access model is agreed
- [ ] RLS is designed and tested, if required
- [ ] Measures and definitions are documented
- [ ] Output has been validated
- [ ] Refresh approach is confirmed
- [ ] Connection and credential ownership is clear
- [ ] Monitoring and support responsibilities are assigned
- [ ] BIA review is completed, where applicable
