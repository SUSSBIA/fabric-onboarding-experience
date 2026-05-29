# Workspace Access Checklist

Use this checklist when reviewing a Fabric workspace access request.

This checklist helps workspace owners, deputy workspace owners, department representatives, and BIA reviewers apply least privilege, purpose-based access, ownership continuity, workspace boundary rules, and appropriate governance before granting access.

## 1. Request Information

| Field                        | Response                                                                   |
| ---------------------------- | -------------------------------------------------------------------------- |
| Requester name               |                                                                            |
| Requester department or team |                                                                            |
| Request date                 |                                                                            |
| Workspace requested          |                                                                            |
| Workspace type               | Personal / Sandbox / Department / BIA Production                           |
| Access pattern               | Workspace membership / Item sharing / Report sharing / App sharing / Other |
| Requested role               | Viewer / Contributor / Member / Admin / Unsure                             |
| Requested duration           | Temporary / Ongoing / Unsure                                               |
| Workspace owner              |                                                                            |
| Deputy workspace owner       |                                                                            |
| Reviewer                     |                                                                            |

## 2. Purpose Check

* [ ] The purpose of access is clearly stated
* [ ] The requester has a valid learning, project, operational, or business reason
* [ ] The request is linked to an onboarding activity, department use case, or approved work
* [ ] The requester understands the purpose of the workspace
* [ ] The requester understands whether the workspace is personal, sandbox, department, or production-facing
* [ ] The requested access is not broader than the stated purpose
* [ ] The requested access pattern is appropriate for the purpose

## 3. Workspace Boundary Check

| Workspace Type           | Access Review Consideration                                                                                                                                               |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Personal Workspace       | Used for private drafts and individual exploration. Access requests to another user’s personal workspace are usually not appropriate for shared University work.          |
| Sandbox Workspace        | Suitable for onboarding, learning, and experimentation using public, mocked, synthetic, or approved non-sensitive data                                                    |
| Department Workspace     | Access should align with department use case, ownership, data approval, and continuity expectations                                                                       |
| BIA Production Workspace | Restricted to BIA users only. Non-BIA users should not be granted direct workspace access; approved outputs should be shared through approved report/app sharing channels |

Confirm:

* [ ] The requested workspace type is appropriate for the stated purpose
* [ ] The request is not using a personal workspace for shared department work
* [ ] The request is not using a sandbox workspace for official reporting
* [ ] The request is not using a department workspace for unmanaged production use
* [ ] The request does not grant direct BIA Production Workspace access to non-BIA users
* [ ] Approved production outputs for non-BIA users are shared through approved report/app sharing channels instead of direct workspace membership

## 4. Ownership Continuity Check

Complete this section for department workspace requests.

* [ ] A workspace owner is identified
* [ ] A deputy workspace owner is identified
* [ ] The owner and deputy are from the requesting department or business area, where appropriate
* [ ] The owner understands their responsibility for workspace purpose, access, ownership, and continuity
* [ ] The deputy can support or take over if the owner leaves, changes role, or is unavailable
* [ ] The owner and deputy understand who should be contacted for refresh, connection, or access issues
* [ ] The request should not proceed if no owner or deputy workspace owner is identified

## 5. Least Privilege Check

* [ ] Viewer access is sufficient if the user only needs to view reports
* [ ] Contributor access is only considered if the user needs to create or edit content
* [ ] Member access is only considered if the user needs broader collaboration privileges
* [ ] Admin access is only considered for workspace owners, deputy workspace owners, or authorised administrators
* [ ] The requested role is not higher than necessary
* [ ] Elevated access is justified and documented
* [ ] Item, report, or app sharing is considered where workspace membership is not needed

## 6. Data Sensitivity Check

* [ ] The data or assets in the workspace are understood
* [ ] Sensitivity labels have been considered
* [ ] Confidential or restricted data access is justified, if applicable
* [ ] The requester is authorised to access the relevant data
* [ ] Sharing and export risks have been considered
* [ ] The requester understands handling expectations for the data
* [ ] Workspace access is not treated as permission to export, reuse, or redistribute data

## 7. External Collaborator Check

Complete this section if the requester is not University staff.

* [ ] External collaborator status has been identified
* [ ] Microsoft Entra B2B guest account requirement has been considered
* [ ] Licensing requirement has been considered
* [ ] Purpose of external access is documented
* [ ] Data sensitivity risk has been reviewed
* [ ] Time-bound access has been considered
* [ ] Owner for access removal is identified
* [ ] BIA review is requested where required
* [ ] External collaborators are not granted direct access to BIA Production Workspaces
* [ ] Approved production outputs for external collaborators are shared only through approved channels, where applicable

## 8. Production and Escalation Check

* [ ] The request does not involve direct BIA Production Workspace access for non-BIA users
* [ ] The request does not bypass tenant-level or administrator-controlled settings
* [ ] The request does not involve preview, advanced, or capacity-heavy features without review
* [ ] The request does not involve productionisation without BIA review
* [ ] BIA escalation is requested where needed

## 9. Decision

| Decision Area                             | Response                                                                   |
| ----------------------------------------- | -------------------------------------------------------------------------- |
| Recommended access pattern                | Workspace membership / Item sharing / Report sharing / App sharing / Other |
| Recommended role                          | Viewer / Contributor / Member / Admin / Reject / Escalate                  |
| Approved sharing channel, if applicable   | Workspace access / Report sharing / App sharing / Other / Not applicable   |
| Access duration                           | Temporary / Ongoing / Time-bound until:                                    |
| Conditions or caveats                     |                                                                            |
| Reviewer decision                         | Approved / Rejected / Escalated                                            |
| Reason                                    |                                                                            |
| Follow-up required                        | Yes / No                                                                   |
| Access removal review date, if applicable |                                                                            |

## 10. Post-Approval Reminder

* [ ] User understands workspace purpose
* [ ] User understands workspace boundary
* [ ] User understands data sensitivity expectations
* [ ] User understands sharing and export expectations
* [ ] User knows who to contact for questions
* [ ] Workspace owner and deputy owner are recorded, where applicable
* [ ] Access review or removal date is noted, if applicable
* [ ] Non-BIA users are not granted direct BIA Production Workspace access
