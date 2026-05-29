# Row-Level Security Testing Checklist

Use this checklist before relying on Row-Level Security, also known as RLS, in a Power BI or Fabric semantic model.

RLS should be tested carefully because workspace access alone does not guarantee that users only see the rows they are supposed to see.

RLS is one layer of access control. It should be used together with appropriate workspace roles, item permissions, sharing settings, sensitivity labels, and review.

## 1. Basic Information

| Field                                 | Response                                         |
| ------------------------------------- | ------------------------------------------------ |
| Semantic model name                   |                                                  |
| Report name, if applicable            |                                                  |
| Workspace                             |                                                  |
| Workspace type                        | Personal / Sandbox / Department / BIA Production |
| Model owner                           |                                                  |
| Workspace owner                       |                                                  |
| Deputy workspace owner, if applicable |                                                  |
| RLS designer                          |                                                  |
| Tester                                |                                                  |
| Test date                             |                                                  |
| RLS status                            | Sandbox / Draft / UAT / Department / Production  |

## 2. RLS Requirement

* [ ] The need for RLS is confirmed
* [ ] The intended user groups are identified
* [ ] The data each group should see is clearly defined
* [ ] The data each group should not see is clearly defined
* [ ] The business owner or data owner agrees that RLS is required
* [ ] The RLS design is documented before testing
* [ ] RLS is not being used as a substitute for appropriate workspace or item access control

## 3. Workspace and Access Context

| Workspace Type           | RLS Expectation                                                                                    |
| ------------------------ | -------------------------------------------------------------------------------------------------- |
| Personal Workspace       | Not suitable for shared or production RLS testing. Use only for private learning or drafts.        |
| Sandbox Workspace        | Suitable for learning or testing RLS concepts using safe data. Not production-ready.               |
| Department Workspace     | Suitable for department-level UAT or controlled access testing, with clear owner and deputy owner. |
| BIA Production Workspace | Suitable for BIA-managed production RLS, with direct workspace access restricted to BIA users.     |

Confirm:

* [ ] The semantic model is in the correct workspace for its purpose
* [ ] The workspace owner is known
* [ ] The deputy workspace owner is known, if this is a department workspace asset
* [ ] Workspace role access is appropriate
* [ ] Item permissions are appropriate
* [ ] Report or app sharing permissions are appropriate
* [ ] BIA Production Workspace access remains restricted to BIA users, where applicable
* [ ] Non-BIA users consume approved production outputs through approved report or app sharing channels, where applicable

## 4. Access Logic

| User Group or Role | Expected Data Access | Should Not See | Notes |
| ------------------ | -------------------- | -------------- | ----- |
|                    |                      |                |       |
|                    |                      |                |       |
|                    |                      |                |       |

Examples:

| User Group or Role       | Expected Data Access  | Should Not See                            | Notes |
| ------------------------ | --------------------- | ----------------------------------------- | ----- |
| School A users           | School A records only | School B records                          |       |
| School B users           | School B records only | School A records                          |       |
| Central authorised users | All approved records  | Restricted fields not approved for access |       |

## 5. User Mapping

* [ ] User-to-role mapping is available
* [ ] User-to-department, school, or group mapping is available, if required
* [ ] Test users are identified
* [ ] Users with multiple roles are identified
* [ ] Users with no mapping are identified
* [ ] Mapping source is documented
* [ ] Mapping owner is identified
* [ ] Mapping update process is understood
* [ ] Mapping ownership will not depend only on the original model creator

## 6. Test Accounts or Test Users

| Test User | Expected Role | Expected Access | Test Result              | Notes |
| --------- | ------------- | --------------- | ------------------------ | ----- |
|           |               |                 | Pass / Fail / Not tested |       |
|           |               |                 | Pass / Fail / Not tested |       |
|           |               |                 | Pass / Fail / Not tested |       |

## 7. Positive Testing

Positive testing checks that users can see what they are supposed to see.

* [ ] User can open the report
* [ ] User can see the expected rows
* [ ] User can see the expected totals
* [ ] User can use filters and slicers within their allowed data
* [ ] User can see expected drill-down or detail records, if applicable
* [ ] Central authorised users can see approved broader access, if applicable
* [ ] Expected report pages remain usable under RLS

## 8. Negative Testing

Negative testing checks that users cannot see what they are not supposed to see.

* [ ] User cannot see other departments, schools, groups, or restricted records
* [ ] User cannot infer hidden data through totals, filters, or slicers
* [ ] User cannot access restricted records through drill-through or detail pages
* [ ] User cannot bypass RLS through another report connected to the same model
* [ ] User cannot bypass RLS through inappropriate build permission
* [ ] Users with no mapping do not see inappropriate data
* [ ] External collaborators, if any, are restricted appropriately

## 9. Filter and Interaction Testing

* [ ] Slicers only show values the user is allowed to see
* [ ] Visual interactions do not reveal hidden groups
* [ ] Totals and subtotals behave as expected under RLS
* [ ] Drill-through pages respect RLS
* [ ] Tooltips respect RLS
* [ ] Export behaviour has been considered
* [ ] Subscriptions or alerts do not expose restricted data
* [ ] Filters do not accidentally reveal restricted values or categories

## 10. Workspace and Sharing Review

* [ ] Workspace role access is appropriate
* [ ] Report sharing permissions are appropriate
* [ ] Semantic model permissions are appropriate
* [ ] Users do not have build permission unless needed
* [ ] External sharing has been reviewed, if applicable
* [ ] RLS is not being used as the only control where stronger access control is needed
* [ ] Approved sharing channel is identified, where applicable
* [ ] If this is a BIA production output, non-BIA users access it through approved report or app sharing channels, not direct BIA Production Workspace membership

## 11. Sensitivity and Governance

* [ ] Sensitivity label is appropriate
* [ ] Intended audience is documented
* [ ] Data owner has reviewed the access logic
* [ ] Business owner has reviewed the expected user access
* [ ] Export, screenshot, and onward-sharing risks are considered
* [ ] BIA review is completed where required
* [ ] RLS documentation is stored with the asset documentation

## 12. Test Results Summary

| Test Area                             | Result                | Notes |
| ------------------------------------- | --------------------- | ----- |
| Access logic documented               | Pass / Fail / Partial |       |
| User mapping reviewed                 | Pass / Fail / Partial |       |
| Positive testing completed            | Pass / Fail / Partial |       |
| Negative testing completed            | Pass / Fail / Partial |       |
| Filters and interactions tested       | Pass / Fail / Partial |       |
| Sharing and permissions reviewed      | Pass / Fail / Partial |       |
| Data owner or business owner reviewed | Pass / Fail / Partial |       |

## 13. Issues Found

| Issue | Impact              | Recommended Action | Owner | Priority            |
| ----- | ------------------- | ------------------ | ----- | ------------------- |
|       | Low / Medium / High |                    |       | Low / Medium / High |
|       | Low / Medium / High |                    |       | Low / Medium / High |
|       | Low / Medium / High |                    |       | Low / Medium / High |

## 14. Review Decision

| Decision Area                           | Response                                                                 |
| --------------------------------------- | ------------------------------------------------------------------------ |
| RLS ready for use?                      | Yes / No / Yes with caveats                                              |
| Main caveats                            |                                                                          |
| Required fixes                          |                                                                          |
| Reviewer                                |                                                                          |
| Follow-up owner                         |                                                                          |
| Approved sharing channel, if applicable | Workspace access / Report sharing / App sharing / Other / Not applicable |
| Target date                             |                                                                          |

## 15. Final Checklist

* [ ] RLS requirement is confirmed
* [ ] Workspace type and RLS status are clear
* [ ] Access logic is documented
* [ ] User mapping is available
* [ ] Test users are identified
* [ ] Positive testing is completed
* [ ] Negative testing is completed
* [ ] Filters, drill-through, tooltips, and interactions are tested
* [ ] Workspace and sharing permissions are reviewed
* [ ] Build permission is reviewed
* [ ] Data owner or business owner has reviewed the result
* [ ] Department workspace owner and deputy owner are identified, where applicable
* [ ] BIA Production Workspace access remains restricted to BIA users, where applicable
* [ ] Approved sharing channel is identified, where applicable
* [ ] Review decision is documented
