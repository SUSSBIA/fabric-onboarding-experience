# Semantic Model Review Checklist

Use this checklist when reviewing a semantic model before reuse, wider sharing, or productionisation.

This checklist helps report developers, data analysts, data modellers, workspace owners, and BIA reviewers check whether a semantic model is understandable, reusable, and safe to rely on.

## 1. Basic Information

| Field | Response |
|---|---|
| Semantic model name |  |
| Workspace |  |
| Model owner |  |
| Reviewer |  |
| Review date |  |
| Model status | Sandbox / Draft / Prototype / UAT / Department / Production |
| Intended users |  |
| Related reports |  |
| Sensitivity label | Confidential - SUSS / Restricted - SUSS / Unrestricted - SUSS / None / Unsure |

## 2. Purpose and Scope

- [ ] The purpose of the semantic model is clear
- [ ] The intended audience is clear
- [ ] The model supports a known report, analysis, or use case
- [ ] The model status is clear: sandbox, draft, prototype, UAT, department, or production
- [ ] The model does not imply production readiness if it is only a sandbox or prototype artefact
- [ ] The scope of the model is documented

## 3. Data Source and Ownership

- [ ] Data sources are identified
- [ ] Data owners are identified
- [ ] Data stewards or subject matter experts are identified, if applicable
- [ ] Source refresh or update frequency is understood
- [ ] Source data limitations are documented
- [ ] Use of the data is approved for the intended purpose
- [ ] Source system dependencies are understood

## 4. Grain and Tables

- [ ] The grain of each important table is documented
- [ ] Users can understand what one row represents
- [ ] Fact-like and dimension-like tables are identifiable
- [ ] Table names are clear and meaningful
- [ ] Duplicate or unnecessary tables are avoided
- [ ] Tables not intended for users are hidden where appropriate
- [ ] Raw, cleaned, and curated data are not confused

## 5. Relationships

- [ ] Relationships between tables are reviewed
- [ ] Relationship cardinality is appropriate
- [ ] Cross-filter direction is intentional
- [ ] Inactive relationships are documented, if used
- [ ] Ambiguous relationships are avoided
- [ ] Relationship design supports the intended report logic
- [ ] Relationship behaviour has been tested with sample visuals

## 6. Measures and Calculations

- [ ] Key measures are clearly named
- [ ] Key measures are documented
- [ ] Measures use business-friendly names
- [ ] Ambiguous measure names such as `Total`, `Amount`, or `Value` are avoided
- [ ] Measures produce expected results under different filter contexts
- [ ] Important calculations have been validated
- [ ] Duplicated or conflicting measures are avoided
- [ ] Measures that are experimental are clearly marked

## 7. Field Naming and Usability

- [ ] Field names are understandable to report developers
- [ ] Display names are business-friendly where possible
- [ ] Technical fields are hidden where not needed
- [ ] Columns are categorised or formatted where useful
- [ ] Date fields are handled consistently
- [ ] Numeric fields have appropriate formatting
- [ ] Fields that require explanation are documented

## 8. Definitions and Documentation

- [ ] Data dictionary exists or is planned
- [ ] Key fields are defined
- [ ] Key measures are defined
- [ ] Business rules are documented
- [ ] Caveats and limitations are documented
- [ ] Ownership of definitions is clear
- [ ] Documentation is stored in an accessible location

## 9. Reuse and Duplication

- [ ] Existing approved semantic models were checked before creating this one
- [ ] The model does not duplicate an existing trusted model unnecessarily
- [ ] Reuse opportunities have been considered
- [ ] If duplication exists, the reason is documented
- [ ] The model is suitable for reuse only if definitions are stable and reviewed
- [ ] Users know whether the model is sandbox-only or reusable

## 10. Security and Row-Level Security

- [ ] Sensitivity label is appropriate
- [ ] Intended audience is authorised
- [ ] Row-Level Security requirement has been assessed
- [ ] RLS roles are documented, if applicable
- [ ] RLS has been tested, if applicable
- [ ] Users with no mapping behave as expected, if applicable
- [ ] External collaborator access has been reviewed, if applicable
- [ ] Workspace role access does not expose more data than intended

## 11. Refresh and Performance

- [ ] Refresh or Direct Lake behaviour is understood
- [ ] Refresh frequency is justified
- [ ] Refresh owner is identified
- [ ] Connection or credential owner is identified
- [ ] Gateway dependency is known, if applicable
- [ ] Model size and performance are acceptable for intended use
- [ ] Slow visuals or queries have been investigated
- [ ] Capacity impact has been considered for recurring or heavy use

## 12. Validation

- [ ] Key measures have been checked against source data or expected values
- [ ] Sample report visuals behave as expected
- [ ] Filters and slicers produce expected results
- [ ] Totals and subtotals behave as expected
- [ ] Business owner or subject matter expert has reviewed important outputs
- [ ] Known issues are documented
- [ ] The model is not promoted if validation is incomplete

## 13. Review Decision

| Decision Area | Response |
|---|---|
| Review outcome | Approved / Approved with caveats / Needs revision / Sandbox only / Not suitable for reuse |
| Main issues found |  |
| Required changes |  |
| Reviewer |  |
| Follow-up owner |  |
| Target date |  |

## 14. Final Checklist

- [ ] Model purpose is clear
- [ ] Data sources and owners are identified
- [ ] Grain is documented
- [ ] Relationships are reviewed
- [ ] Measures are clearly named and defined
- [ ] Key outputs are validated
- [ ] Reuse and duplication have been considered
- [ ] Security and RLS requirements are reviewed
- [ ] Refresh and ownership are clear
- [ ] Review decision is documented
