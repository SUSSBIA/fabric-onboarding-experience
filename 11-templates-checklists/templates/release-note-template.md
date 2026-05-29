# Release Note Template

Use this template when documenting a change, update, release, or retirement of a Fabric asset.

This is especially useful when an asset is shared more widely, moved beyond sandbox, updated for department use, or considered for BIA production.

## 1. Release Summary

| Field                                 | Response                                                                                                  |
| ------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| Asset name                            |                                                                                                           |
| Workspace                             |                                                                                                           |
| Workspace type                        | Personal / Sandbox / Department / BIA Production                                                          |
| Asset type                            | Report / Semantic Model / Lakehouse / Warehouse / Notebook / Pipeline / Dataflow Gen2 / Dashboard / Other |
| Asset status                          | Sandbox / Draft / Prototype / UAT / Department / Production                                               |
| Release type                          | New / Update / Fix / Retirement                                                                           |
| Version or release date               |                                                                                                           |
| Owner                                 |                                                                                                           |
| Workspace owner                       |                                                                                                           |
| Deputy workspace owner, if applicable |                                                                                                           |
| Reviewer or approver                  |                                                                                                           |
| Intended audience                     |                                                                                                           |
| Sensitivity label                     | Confidential - SUSS / Restricted - SUSS / Unrestricted - SUSS / None / Unsure                             |

## 2. Purpose of Release

| Question                                                           | Response          |
| ------------------------------------------------------------------ | ----------------- |
| Why is this release needed?                                        |                   |
| What business question, process, or learning need does it support? |                   |
| Who will use the asset?                                            |                   |
| Is this sandbox, department-facing, or production-facing?          |                   |
| Is the release intended for wider sharing?                         | Yes / No / Unsure |
| Is BIA review required?                                            | Yes / No / Unsure |

## 3. Workspace and Sharing Boundary

| Workspace Type           | Release Expectation                                                                                                                          |
| ------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------- |
| Personal Workspace       | Suitable only for private drafts and individual exploration. Personal workspace assets should not be released as shared or official outputs. |
| Sandbox Workspace        | Suitable for learning and experimentation. Sandbox outputs should not be released as official reports or production assets.                  |
| Department Workspace     | Suitable for department-level working assets, prototypes, UAT, or approved department use cases. Owner and deputy owner should be known.     |
| BIA Production Workspace | Suitable for BIA-managed production assets. Direct workspace access is restricted to BIA users.                                              |

Confirm:

* [ ] The asset is in the correct workspace for the release purpose
* [ ] Personal workspace content is not being released as a shared department or production asset
* [ ] Sandbox output is not being presented as official or production-ready
* [ ] Department workspace release has a clear workspace owner and deputy owner
* [ ] BIA Production Workspace access remains restricted to BIA users, where applicable
* [ ] Non-BIA users consume approved production outputs through approved report or app sharing channels, where applicable

## 4. What Changed

| Change Area                              | Description |
| ---------------------------------------- | ----------- |
| Report layout or visuals                 |             |
| Measures or KPIs                         |             |
| Semantic model                           |             |
| Data source                              |             |
| Refresh or connection                    |             |
| Access or sharing                        |             |
| RLS or security                          |             |
| Documentation                            |             |
| Retirement or replacement, if applicable |             |
| Other                                    |             |

## 5. Impact Assessment

| Question                                                 | Response          |
| -------------------------------------------------------- | ----------------- |
| Which users are affected?                                |                   |
| Which reports or downstream assets are affected?         |                   |
| Are existing definitions or measures changed?            | Yes / No / Unsure |
| Could users see different numbers after this release?    | Yes / No / Unsure |
| Is communication to users needed?                        | Yes / No / Unsure |
| Is training or guidance needed?                          | Yes / No / Unsure |
| Could users misinterpret the change without explanation? | Yes / No / Unsure |
| Are any old assets being replaced or retired?            | Yes / No / Unsure |

## 6. Validation

| Validation Area                               | Response                  |
| --------------------------------------------- | ------------------------- |
| Output validated against source data?         | Yes / No / Not applicable |
| Measures checked?                             | Yes / No / Not applicable |
| Filters and slicers checked?                  | Yes / No / Not applicable |
| RLS tested, if applicable?                    | Yes / No / Not applicable |
| Refresh tested?                               | Yes / No / Not applicable |
| Business owner reviewed?                      | Yes / No / Not applicable |
| Data owner or subject matter expert reviewed? | Yes / No / Not applicable |
| Known issues                                  |                           |

## 7. Access and Governance

| Question                                  | Response                                                                 |
| ----------------------------------------- | ------------------------------------------------------------------------ |
| Is the sensitivity label appropriate?     | Yes / No / Unsure                                                        |
| Is the intended audience clearly defined? | Yes / No / Unsure                                                        |
| Are workspace roles appropriate?          | Yes / No / Unsure                                                        |
| Are sharing permissions appropriate?      | Yes / No / Unsure                                                        |
| Is export allowed?                        | Yes / No / Unsure                                                        |
| Is external collaborator access involved? | Yes / No / Unsure                                                        |
| Is BIA review required?                   | Yes / No / Unsure                                                        |
| Approved sharing channel, if applicable   | Workspace access / Report sharing / App sharing / Other / Not applicable |

## 8. Refresh and Operations

| Question                               | Response                                                                             |
| -------------------------------------- | ------------------------------------------------------------------------------------ |
| Does the asset require refresh?        | Yes / No / Unsure                                                                    |
| Refresh frequency                      |                                                                                      |
| Connection owner                       |                                                                                      |
| Credential owner                       |                                                                                      |
| Monitoring owner                       |                                                                                      |
| Support contact                        |                                                                                      |
| Escalation route                       | BIA / IT / Vendor / Department owner / Deputy workspace owner / Source owner / Other |
| Are users able to identify stale data? | Yes / No / Unsure                                                                    |

## 9. Retirement or Replacement

Complete this section if the release retires or replaces an existing asset.

| Question                              | Response                  |
| ------------------------------------- | ------------------------- |
| Is an old asset being retired?        | Yes / No / Not applicable |
| Asset being replaced                  |                           |
| Reason for retirement or replacement  |                           |
| Has usage or dependency been checked? | Yes / No / Unsure         |
| Are users informed?                   | Yes / No / Unsure         |
| Is an archive needed before deletion? | Yes / No / Unsure         |
| Retirement date                       |                           |
| Owner of retirement action            |                           |

## 10. Release Decision

| Option                                           | Select One |
| ------------------------------------------------ | ---------- |
| Release approved                                 |            |
| Release approved with caveats                    |            |
| Hold release pending validation                  |            |
| Hold release pending access or governance review |            |
| Return for revision                              |            |
| Retire asset                                     |            |
| Keep as sandbox or department working asset only |            |

## 11. Release Notes for Users

| Area                          | Message |
| ----------------------------- | ------- |
| Summary of change             |         |
| What users should know        |         |
| Any caveats                   |         |
| Any action users need to take |         |
| Who to contact for questions  |         |

## 12. Follow-Up Actions

| Action | Owner | Target Date | Status                           |
| ------ | ----- | ----------- | -------------------------------- |
|        |       |             | Not started / In progress / Done |
|        |       |             | Not started / In progress / Done |
|        |       |             | Not started / In progress / Done |
