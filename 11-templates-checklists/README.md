# Templates and Checklists

This section provides reusable templates and checklists for Fabric onboarding, sandbox learning, workspace management, deployment review, and productionisation readiness.

Templates help users document their thinking clearly. Checklists help users avoid missing important security, access, ownership, refresh, and governance considerations.

## Why templates matter

Fabric onboarding is not only about learning where to click.

Users also need to learn how to:

- Frame use cases clearly
- Document assumptions
- Check sensitivity and access
- Review report context
- Validate measures and outputs
- Track ownership
- Plan refresh and monitoring
- Decide whether an asset should remain sandbox or move beyond sandbox

Templates make these practices easier to repeat.

![Templates and checklists overview](../assets/images/templates-checklists-overview.png)

> Image placeholder: Overview showing templates and checklists for report context, insight summaries, use case canvas, workspace health, production readiness, refresh ownership, RLS testing, and sandbox experiment review.

## Template catalogue

| Template | Purpose | Suggested Location |
|---|---|---|
| Report Context Note | Helps users check report title, owner, refresh date, sensitivity label, caveats, and questions | `report-context-note.md` |
| Insight Summary Template | Helps analysts write observations with caveats and follow-up questions | `insight-summary-template.md` |
| Use Case Canvas | Helps department representatives frame analytics use cases clearly | `use-case-canvas.md` |
| Workspace Inventory Template | Helps workspace owners review items, owners, status, and actions | `workspace-inventory-template.md` |
| Workspace Health Note | Helps workspace owners summarise access, naming, sensitivity, refresh, and escalation concerns | `workspace-health-note.md` |
| Model Card Template | Helps data scientists document model purpose, inputs, outputs, metrics, limitations, and risks | `model-card-template.md` |
| Release Note Template | Helps teams document what changed before wider release | `release-note-template.md` |
| Refresh Failure Note | Helps users report refresh, connection, gateway, or pipeline failures clearly | `refresh-failure-note.md` |

## Checklist catalogue

| Checklist | Purpose | Suggested Location |
|---|---|---|
| Sandbox Readiness Checklist | Confirms users are working safely in sandbox | `sandbox-readiness-checklist.md` |
| Workspace Access Checklist | Supports least privilege and purpose-based access decisions | `workspace-access-checklist.md` |
| Report Review Checklist | Supports review of report clarity, definitions, filters, and caveats | `report-review-checklist.md` |
| Semantic Model Review Checklist | Supports review of grain, relationships, measures, definitions, reuse, and ownership | `semantic-model-review-checklist.md` |
| RLS Testing Checklist | Supports validation of Row-Level Security behaviour | `rls-testing-checklist.md` |
| Refresh and Monitoring Checklist | Supports ownership of connections, credentials, refresh, and failure monitoring | `refresh-monitoring-checklist.md` |
| Productionisation Readiness Checklist | Supports review before moving assets beyond sandbox or department use | `productionisation-readiness-checklist.md` |
| External Collaborator Checklist | Supports review of guest account, licensing, access, sensitivity, and removal planning | `external-collaborator-checklist.md` |

## Suggested folder structure

Use this structure:

```text
11-templates-checklists/
├── README.md
├── templates/
│   ├── report-context-note.md
│   ├── insight-summary-template.md
│   ├── use-case-canvas.md
│   ├── workspace-inventory-template.md
│   ├── workspace-health-note.md
│   ├── model-card-template.md
│   ├── release-note-template.md
│   └── refresh-failure-note.md
│
└── checklists/
    ├── sandbox-readiness-checklist.md
    ├── workspace-access-checklist.md
    ├── report-review-checklist.md
    ├── semantic-model-review-checklist.md
    ├── rls-testing-checklist.md
    ├── refresh-monitoring-checklist.md
    ├── productionisation-readiness-checklist.md
    └── external-collaborator-checklist.md
```

Some templates may also be copied into the HDB Resales sandbox folder when they are used for specific exercises:

```text
09-sandbox-experiments/hdb-resales/templates/
```

The version in `11-templates-checklists/` should be treated as the general reusable version.

## Report Context Note

Use this when reviewing a report.

```markdown
# Report Context Note

## Basic Information

| Field | Response |
|---|---|
| Report name |  |
| Workspace |  |
| Report owner or contact |  |
| Report purpose |  |
| Intended audience |  |
| Report status | Sandbox / Draft / Prototype / UAT / Department / Production |
| Refresh date or data currency |  |
| Sensitivity label |  |

## Context Check

| Question | Response |
|---|---|
| Is the report clearly labelled? |  |
| Is the purpose clear? |  |
| Are the main measures defined? |  |
| Are filters and slicers easy to understand? |  |
| Are caveats visible? |  |
| Is the report safe to share with the intended audience? |  |

## Notes

```text
Important caveats:

Questions to clarify:

Potential issues:
```
```

## Insight Summary Template

Use this when writing an analytical finding.

```markdown
# Insight Summary

## Analytical Question

```text
What question are you trying to answer?
```

## Observation

```text
The analysis suggests that...
```

## Why It Matters

```text
This may be useful because...
```

## Caveat

```text
This should be interpreted carefully because...
```

## Follow-Up Question

```text
The next question to explore is...
```

## Additional Data Needed

```text
Additional data that may strengthen the analysis:
```
```

## Use Case Canvas

Use this when framing a department analytics use case.

```markdown
# Use Case Canvas

## Use Case Summary

| Field | Response |
|---|---|
| Use case title |  |
| Department or team |  |
| Business question |  |
| Intended users |  |
| Decision or action supported |  |
| Expected output | Report / Dashboard / Dataset / Semantic Model / Analysis / Model / Other |
| Current maturity | Idea / Sandbox / Department exploration / UAT / Production candidate |

## Data and Ownership

| Field | Response |
|---|---|
| Data needed |  |
| Current source |  |
| Data owner |  |
| Data steward or subject matter expert |  |
| Update frequency |  |
| Known data quality concerns |  |

## Access and Governance

| Field | Response |
|---|---|
| Likely sensitivity label |  |
| Intended audience |  |
| Users who should not have access |  |
| Is RLS likely needed? | Yes / No / Unsure |
| Are external collaborators involved? | Yes / No |
| Workspace type | Sandbox / Department / BIA Production / Unsure |

## Operational Considerations

| Field | Response |
|---|---|
| Refresh required? | Yes / No / Unsure |
| Refresh frequency |  |
| Owner after creation |  |
| Support contact |  |
| BIA support needed? | Yes / No / Unsure |

## Risks and Next Steps

```text
Key risks or caveats:

Questions for BIA:

Recommended next step:
```
```

## Workspace Inventory Template

Use this when reviewing workspace items.

```markdown
# Workspace Inventory

| Item Name | Item Type | Owner | Purpose | Status | Sensitivity Label | Refresh Needed | Action Needed |
|---|---|---|---|---|---|---|---|
|  | Report / Semantic Model / Lakehouse / Notebook / Pipeline / Dataflow / Dashboard / Other |  |  | Sandbox / Draft / Prototype / UAT / Department / Production |  | Yes / No / Unsure |  |
```

## Workspace Health Note

Use this when summarising the health of a workspace.

```markdown
# Workspace Health Note

## Workspace Summary

| Field | Response |
|---|---|
| Workspace name |  |
| Workspace type | Sandbox / Department / BIA Production |
| Main purpose |  |
| Main users |  |
| Workspace owner |  |
| Review date |  |

## Review Areas

| Area | Notes |
|---|---|
| Access and roles |  |
| Naming and organisation |  |
| Item ownership |  |
| Sensitivity labels |  |
| Sharing and export risks |  |
| Connections and credentials |  |
| Refresh and monitoring |  |
| Duplicates or obsolete items |  |
| Escalation needs |  |

## Recommended Actions

```text
Action 1:
Action 2:
Action 3:
```
```

## Model Card Template

Use this when documenting a sandbox model or advanced analytics output.

```markdown
# Model Card

## Model Summary

| Field | Response |
|---|---|
| Model or experiment name |  |
| Owner |  |
| Date |  |
| Purpose |  |
| Intended use |  |
| Not intended for |  |
| Sandbox or production status | Sandbox / Review / Production |

## Data

| Field | Response |
|---|---|
| Input data |  |
| Data source |  |
| Key features |  |
| Target variable, if any |  |
| Data limitations |  |
| Data sensitivity |  |

## Method

| Field | Response |
|---|---|
| Method used | Clustering / Classification / Regression / Other |
| Tool or notebook |  |
| Parameters or settings |  |
| Output produced |  |

## Evaluation

| Field | Response |
|---|---|
| Evaluation metric or profiling method |  |
| Baseline or comparison |  |
| Main result |  |
| Known weaknesses |  |

## Responsible Use

```text
Interpretation:

Caveats:

Risks of misuse:

Validation needed before wider use:

Decision:
Remain sandbox / Improve further / Propose for review
```
```

## Release Note Template

Use this when an asset is shared more widely or moved towards production.

```markdown
# Release Note

| Field | Response |
|---|---|
| Asset name |  |
| Workspace |  |
| Version or release date |  |
| Owner |  |
| Release type | New / Update / Fix / Retirement |
| Intended audience |  |
| Sensitivity label |  |

## What Changed

```text
Summary of changes:
```

## Why It Changed

```text
Reason for change:
```

## Validation

```text
Validation completed:

Known issues:

Approver or reviewer:
```

## Support

```text
Support contact:

Escalation route:
```
```

## Refresh Failure Note

Use this when reporting a refresh, connection, gateway, or pipeline failure.

```markdown
# Refresh Failure Note

| Field | Response |
|---|---|
| Asset name |  |
| Workspace |  |
| Item type | Report / Semantic Model / Dataflow / Pipeline / Notebook / Lakehouse / Other |
| Owner |  |
| Data source |  |
| Refresh or run type | Manual / Scheduled / Pipeline / Other |
| Last successful refresh |  |
| Failure date and time |  |
| Error message |  |
| Recent changes |  |
| Business impact |  |
| Who has already checked |  |
| Escalation needed | BIA / IT / Vendor / Department owner / Unsure |

## Notes

```text
Additional details:
```
```

## Sandbox Readiness Checklist

Use before starting any sandbox exercise.

```markdown
# Sandbox Readiness Checklist

- [ ] I am working in the assigned sandbox workspace
- [ ] I understand the purpose of the exercise
- [ ] I am using public, mocked, synthetic, or approved non-sensitive data
- [ ] I will not upload confidential or restricted institutional data
- [ ] I know which artefact I should use
- [ ] I will not overwrite shared starter artefacts
- [ ] I will name my work clearly
- [ ] I understand that sandbox outputs are not production assets
- [ ] I will document assumptions, caveats, and limitations
- [ ] I know who to ask if I am unsure
```

## Workspace Access Checklist

Use when reviewing access requests.

```markdown
# Workspace Access Checklist

- [ ] Requester is identified
- [ ] Purpose of access is clear
- [ ] Workspace type is known
- [ ] Minimum required role is identified
- [ ] Least privilege has been considered
- [ ] Data sensitivity has been considered
- [ ] Sharing and export risks have been considered
- [ ] External collaborator status has been checked, if applicable
- [ ] Microsoft Entra B2B guest requirement has been considered, if applicable
- [ ] Licensing requirement has been considered, if applicable
- [ ] Time-bound access has been considered, if applicable
- [ ] BIA escalation is requested where needed
```

## Report Review Checklist

Use before sharing a report more widely.

```markdown
# Report Review Checklist

- [ ] Report purpose is clear
- [ ] Intended audience is known
- [ ] Report owner or contact is identified
- [ ] Data source is understood
- [ ] Refresh date or data currency is visible
- [ ] Sensitivity label is appropriate
- [ ] Key measures are defined
- [ ] Filters and slicers are understandable
- [ ] Visuals support the main question
- [ ] Caveats are visible
- [ ] Outputs have been validated
- [ ] Sharing and export expectations are clear
- [ ] Report status is clear: sandbox, draft, prototype, UAT, department, or production
```

## Semantic Model Review Checklist

Use before reusing or promoting a semantic model.

```markdown
# Semantic Model Review Checklist

- [ ] Model purpose is clear
- [ ] Owner is identified
- [ ] Grain is documented
- [ ] Tables are named clearly
- [ ] Relationships are reviewed
- [ ] Measures are named clearly
- [ ] Key measures are defined
- [ ] Duplicated or conflicting measures are avoided
- [ ] Data types are appropriate
- [ ] Sensitivity label is appropriate
- [ ] RLS requirement has been assessed
- [ ] Reuse opportunities have been considered
- [ ] Refresh or Direct Lake behaviour is understood
- [ ] Model is clearly marked as sandbox, department, or production-facing
```

## RLS Testing Checklist

Use before relying on Row-Level Security.

```markdown
# RLS Testing Checklist

- [ ] RLS requirement is confirmed
- [ ] Access logic is documented
- [ ] User-to-access mapping is available
- [ ] Test users are identified
- [ ] Department or group users see only expected records
- [ ] Central users see expected broader access, if approved
- [ ] Users with no mapping behave as expected
- [ ] Sensitive records are not exposed incorrectly
- [ ] Business owner has validated the access rules
- [ ] BIA review is completed where required
```

## Refresh and Monitoring Checklist

Use before setting up recurring refresh or relying on refreshed data.

```markdown
# Refresh and Monitoring Checklist

- [ ] Data source is identified
- [ ] Data source owner is known
- [ ] Connection type is understood
- [ ] Credential or identity owner is known
- [ ] Gateway requirement is checked
- [ ] Refresh frequency is justified
- [ ] Capacity impact is considered
- [ ] Refresh owner is assigned
- [ ] Monitoring owner is assigned
- [ ] Failure escalation path is known
- [ ] Last successful refresh can be checked
- [ ] Users can identify whether data is stale
```

## Productionisation Readiness Checklist

Use before moving beyond sandbox or department experimentation.

```markdown
# Productionisation Readiness Checklist

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
```

## External Collaborator Checklist

Use before granting access to an external collaborator.

```markdown
# External Collaborator Checklist

- [ ] External collaborator is identified
- [ ] Purpose of access is documented
- [ ] Workspace or item access is identified
- [ ] Microsoft Entra B2B guest account requirement is reviewed
- [ ] Licensing requirement is reviewed
- [ ] Minimum required access role is identified
- [ ] Data sensitivity is assessed
- [ ] External sharing risk is assessed
- [ ] Time-bound access is considered
- [ ] Owner for access removal is identified
- [ ] BIA review is completed where required
```

## How to use these templates

Users should copy the relevant template into the working folder for their exercise or project.

For example:

```text
09-sandbox-experiments/hdb-resales/templates/
```

or into a project-specific documentation folder.

Templates should be kept simple enough for users to complete. If a template becomes too heavy, users may skip it. The goal is to support good thinking, not create unnecessary paperwork.

## Next section

Proceed to:

[Glossary](../glossary.md)
