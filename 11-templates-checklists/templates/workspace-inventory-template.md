# Workspace Inventory Template

Use this template to document the contents of a Fabric workspace.

This is useful when reviewing a sandbox workspace, department workspace, or production candidate workspace. It helps clarify what exists, who owns it, what it is used for, and whether any follow-up action is needed.

## 1. Workspace Summary

| Field                         | Response                                                                      |
| ----------------------------- | ----------------------------------------------------------------------------- |
| Workspace name                |                                                                               |
| Workspace type                | Personal / Sandbox / Department / BIA Production                              |
| Business purpose              |                                                                               |
| Requesting department or team |                                                                               |
| Workspace owner               |                                                                               |
| Deputy workspace owner        |                                                                               |
| Reviewer                      |                                                                               |
| Review date                   |                                                                               |
| Sensitivity level, if known   | Confidential - SUSS / Restricted - SUSS / Unrestricted - SUSS / None / Unsure |
| Intended users                |                                                                               |
| Support contact               |                                                                               |
| Escalation route              | BIA / IT / Vendor / Department owner / Other                                  |

## 2. Workspace Boundary Check

| Question                                                                                                                                     | Response                  |
| -------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------- |
| Is the workspace being used for its intended purpose?                                                                                        | Yes / No / Unsure         |
| Is this a personal, sandbox, department, or BIA production workspace?                                                                        |                           |
| If this is a department workspace, is there both an owner and deputy owner?                                                                  | Yes / No / Not applicable |
| If this is a BIA Production Workspace, is direct workspace access restricted to BIA users?                                                   | Yes / No / Not applicable |
| Are non-BIA users consuming approved production outputs through approved report/app sharing channels instead of direct workspace membership? | Yes / No / Not applicable |
| Are any sandbox outputs being treated as official outputs?                                                                                   | Yes / No / Unsure         |
| Are any department assets being treated as production without review?                                                                        | Yes / No / Unsure         |

## 3. Workspace Item Inventory

List the main items in the workspace.

| Item Name | Item Type                                                                                                 | Owner | Purpose | Status                                                      | Sensitivity | Refresh Required? | Notes |
| --------- | --------------------------------------------------------------------------------------------------------- | ----- | ------- | ----------------------------------------------------------- | ----------- | ----------------- | ----- |
|           | Report / Semantic Model / Lakehouse / Warehouse / Notebook / Pipeline / Dataflow Gen2 / Dashboard / Other |       |         | Sandbox / Draft / Prototype / UAT / Department / Production |             | Yes / No / Unsure |       |
|           | Report / Semantic Model / Lakehouse / Warehouse / Notebook / Pipeline / Dataflow Gen2 / Dashboard / Other |       |         | Sandbox / Draft / Prototype / UAT / Department / Production |             | Yes / No / Unsure |       |
|           | Report / Semantic Model / Lakehouse / Warehouse / Notebook / Pipeline / Dataflow Gen2 / Dashboard / Other |       |         | Sandbox / Draft / Prototype / UAT / Department / Production |             | Yes / No / Unsure |       |

## 4. Access and Roles

| User or Group | Role                                  | Purpose of Access | Time-Bound?       | Notes |
| ------------- | ------------------------------------- | ----------------- | ----------------- | ----- |
|               | Viewer / Contributor / Member / Admin |                   | Yes / No / Unsure |       |
|               | Viewer / Contributor / Member / Admin |                   | Yes / No / Unsure |       |
|               | Viewer / Contributor / Member / Admin |                   | Yes / No / Unsure |       |

## 5. Ownership and Continuity

| Question                                                                                  | Response          |
| ----------------------------------------------------------------------------------------- | ----------------- |
| Is the workspace owner still valid?                                                       | Yes / No / Unsure |
| Is the deputy workspace owner still valid?                                                | Yes / No / Unsure |
| Can the deputy support or take over if the owner leaves, changes role, or is unavailable? | Yes / No / Unsure |
| Is item ownership clear?                                                                  | Yes / No / Unsure |
| Are there items owned only by a person who may leave or has left?                         | Yes / No / Unsure |
| Are support and escalation routes clear?                                                  | Yes / No / Unsure |
| Are ownership records up to date?                                                         | Yes / No / Unsure |

## 6. Data and Sensitivity

| Question                                                    | Response          |
| ----------------------------------------------------------- | ----------------- |
| What data sources are used?                                 |                   |
| Are data owners known?                                      | Yes / No / Unsure |
| Is the data approved for this workspace purpose?            | Yes / No / Unsure |
| Are sensitivity labels applied where needed?                | Yes / No / Unsure |
| Does the workspace contain confidential or restricted data? | Yes / No / Unsure |
| Are export and sharing expectations clear?                  | Yes / No / Unsure |
| Are external collaborators involved?                        | Yes / No / Unsure |

## 7. Refresh and Operations

| Question                                            | Response          |
| --------------------------------------------------- | ----------------- |
| Which items require refresh or scheduled runs?      |                   |
| Is refresh ownership clear?                         | Yes / No / Unsure |
| Are credentials or connections owned appropriately? | Yes / No / Unsure |
| Is a gateway required?                              | Yes / No / Unsure |
| Is monitoring assigned?                             | Yes / No / Unsure |
| Are users able to identify stale data?              | Yes / No / Unsure |
| Is there an escalation route for refresh failures?  | Yes / No / Unsure |

## 8. Reuse, Duplication and Clean-Up

| Question                                                       | Response          |
| -------------------------------------------------------------- | ----------------- |
| Are there duplicate reports or semantic models?                | Yes / No / Unsure |
| Are any items obsolete or unused?                              | Yes / No / Unsure |
| Are item names clear?                                          | Yes / No / Unsure |
| Are sandbox, draft, department, and production statuses clear? | Yes / No / Unsure |
| Are there items that should be archived or removed?            | Yes / No / Unsure |
| Are there items that should be reviewed for wider use?         | Yes / No / Unsure |

## 9. Review Notes

| Area                                         | Notes |
| -------------------------------------------- | ----- |
| Key observations                             |       |
| Main risks                                   |       |
| Items requiring follow-up                    |       |
| Recommended clean-up actions                 |       |
| Recommended access changes                   |       |
| Recommended ownership updates                |       |
| Recommended productionisation review, if any |       |

## 10. Follow-Up Actions

| Action | Owner | Target Date | Status                           |
| ------ | ----- | ----------- | -------------------------------- |
|        |       |             | Not started / In progress / Done |
|        |       |             | Not started / In progress / Done |
|        |       |             | Not started / In progress / Done |
