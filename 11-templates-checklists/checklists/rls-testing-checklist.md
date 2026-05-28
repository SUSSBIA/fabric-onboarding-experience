# Row-Level Security Testing Checklist

Use this checklist before relying on Row-Level Security, also known as RLS, in a Power BI or Fabric semantic model.

RLS should be tested carefully because workspace access alone does not guarantee that users only see the rows they are supposed to see.

## 1. Basic Information

| Field | Response |
|---|---|
| Semantic model name |  |
| Report name, if applicable |  |
| Workspace |  |
| Model owner |  |
| RLS designer |  |
| Tester |  |
| Test date |  |
| RLS status | Sandbox / Draft / UAT / Production |

## 2. RLS Requirement

- [ ] The need for RLS is confirmed
- [ ] The intended user groups are identified
- [ ] The data each group should see is clearly defined
- [ ] The data each group should not see is clearly defined
- [ ] The business owner or data owner agrees that RLS is required
- [ ] The RLS design is documented before testing

## 3. Access Logic

| User Group or Role | Expected Data Access | Should Not See | Notes |
|---|---|---|---|
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |

Examples:

| User Group or Role | Expected Data Access | Should Not See | Notes |
|---|---|---|---|
| School A users | School A records only | School B records |  |
| School B users | School B records only | School A records |  |
| Central authorised users | All approved records | Restricted fields not approved for access |  |

## 4. User Mapping

- [ ] User-to-role mapping is available
- [ ] User-to-department, school, or group mapping is available, if required
- [ ] Test users are identified
- [ ] Users with multiple roles are identified
- [ ] Users with no mapping are identified
- [ ] Mapping source is documented
- [ ] Mapping owner is identified

## 5. Test Accounts or Test Users

| Test User | Expected Role | Expected Access | Test Result | Notes |
|---|---|---|---|---|
|  |  |  | Pass / Fail / Not tested |  |
|  |  |  | Pass / Fail / Not tested |  |
|  |  |  | Pass / Fail / Not tested |  |

## 6. Positive Testing

Positive testing checks that users can see what they are supposed to see.

- [ ] User can open the report
- [ ] User can see the expected rows
- [ ] User can see the expected totals
- [ ] User can use filters and slicers within their allowed data
- [ ] User can see expected drill-down or detail records, if applicable
- [ ] Central authorised users can see approved broader access, if applicable

## 7. Negative Testing

Negative testing checks that users cannot see what they are not supposed to see.

- [ ] User cannot see other departments, schools, groups, or restricted records
- [ ] User cannot infer hidden data through totals, filters, or slicers
- [ ] User cannot access restricted records through drill-through or detail pages
- [ ] User cannot bypass RLS through another report connected to the same model
- [ ] Users with no mapping do not see inappropriate data
- [ ] External collaborators, if any, are restricted appropriately

## 8. Filter and Interaction Testing

- [ ] Slicers only show values the user is allowed to see
- [ ] Visual interactions do not reveal hidden groups
- [ ] Totals and subtotals behave as expected under RLS
- [ ] Drill-through pages respect RLS
- [ ] Tooltips respect RLS
- [ ] Export behaviour has been considered
- [ ] Subscriptions or alerts do not expose restricted data

## 9. Workspace and Sharing Review

- [ ] Workspace role access is appropriate
- [ ] Report sharing permissions are appropriate
- [ ] Semantic model permissions are appropriate
- [ ] Users do not have build permission unless needed
- [ ] External sharing has been reviewed, if applicable
- [ ] RLS is not being used as the only control where stronger access control is needed

## 10. Sensitivity and Governance

- [ ] Sensitivity label is appropriate
- [ ] Intended audience is documented
- [ ] Data owner has reviewed the access logic
- [ ] Business owner has reviewed the expected user access
- [ ] BIA review is completed where required
- [ ] RLS documentation is stored with the asset documentation

## 11. Test Results Summary

| Test Area | Result | Notes |
|---|---|---|
| Access logic documented | Pass / Fail / Partial |  |
| User mapping reviewed | Pass / Fail / Partial |  |
| Positive testing completed | Pass / Fail / Partial |  |
| Negative testing completed | Pass / Fail / Partial |  |
| Filters and interactions tested | Pass / Fail / Partial |  |
| Sharing and permissions reviewed | Pass / Fail / Partial |  |
| Data owner or business owner reviewed | Pass / Fail / Partial |  |

## 12. Issues Found

| Issue | Impact | Recommended Action | Owner | Priority |
|---|---|---|---|---|
|  | Low / Medium / High |  |  | Low / Medium / High |
|  | Low / Medium / High |  |  | Low / Medium / High |
|  | Low / Medium / High |  |  | Low / Medium / High |

## 13. Review Decision

| Decision Area | Response |
|---|---|
| RLS ready for use? | Yes / No / Yes with caveats |
| Main caveats |  |
| Required fixes |  |
| Reviewer |  |
| Follow-up owner |  |
| Target date |  |

## 14. Final Checklist

- [ ] RLS requirement is confirmed
- [ ] Access logic is documented
- [ ] User mapping is available
- [ ] Test users are identified
- [ ] Positive testing is completed
- [ ] Negative testing is completed
- [ ] Filters, drill-through, and interactions are tested
- [ ] Workspace and sharing permissions are reviewed
- [ ] Data owner or business owner has reviewed the result
- [ ] Review decision is documented
