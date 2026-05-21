# Start Using Fabric

This section begins the hands-on part of the onboarding experience.

Users should only start this section after reading the foundation sections:

1. [Security, Access and Governance](../01-security-access-governance/)
2. [Licensing, Capacity and Compute Awareness](../02-licensing-capacity/)
3. [Fabric Workspace Operating Model](../03-workspace-operating-model/)

The aim is to help users enter Fabric safely, understand what they are looking at, and complete their first safe activity without accidentally treating exploratory work as production-ready output.

## Before you create anything

When users first enter Fabric, they should not immediately create a report, Lakehouse, pipeline, notebook, or semantic model.

They should first confirm:

- Am I in the correct workspace?
- Is this a sandbox, department, or BIA production workspace?
- What is my workspace role?
- What items already exist?
- Is there an existing report, semantic model, Lakehouse, or dataset I should reuse?
- What data am I allowed to use?
- Is this activity for learning, department exploration, or production work?

![Placeholder: First safe steps in Fabric](../assets/images/first-safe-steps-in-fabric.png)

> Image placeholder: A simple checklist-style diagram showing the first safe steps: sign in, open correct workspace, check workspace type, review existing items, confirm data use, then begin a safe activity.

## Basic user journey

A typical first-use journey should look like this:

```text
Sign in to Fabric
   ↓
Open the correct workspace
   ↓
Confirm workspace type and role
   ↓
Review existing items
   ↓
Check data and sensitivity expectations
   ↓
Create or open the relevant Fabric item
   ↓
Save work with clear naming
   ↓
Share or escalate only when appropriate
```

## Common Fabric items

Users may see different types of items in a Fabric workspace.

| Fabric Item | Used For | Typical Users |
|---|---|---|
| Power BI Report | Visual reporting, dashboards, and interactive analysis | Report consumers, analysts, report developers |
| Semantic Model | A reusable business layer for Power BI reporting, including relationships and measures | Report developers, analysts, data modellers |
| Lakehouse | Storing and analysing structured and semi-structured data | Data engineers, analysts, data scientists |
| Warehouse | SQL-based analytics and data warehousing | Data engineers, SQL users, analysts |
| Data Pipeline | Moving, orchestrating, and scheduling data workflows | Data engineers, advanced analysts |
| Dataflow Gen2 | Low-code data preparation and transformation | Analysts, data engineers |
| Notebook | Code-based data preparation, transformation, analytics, and machine learning | Data engineers, data scientists |
| Dashboard | A Power BI visual summary, usually for monitoring selected metrics | Report consumers, analysts |

Users do not need to learn every Fabric item at once. The relevant item depends on their persona and use case.

## Start from the correct workspace

The first practical step is to identify the correct workspace.

| Workspace Type | What users should do |
|---|---|
| Sandbox Workspace | Practise using safe data and guided exercises |
| Department Workspace | Work on approved department-level exploration or development |
| BIA Production Workspace | Access or support BIA-managed production assets only where authorised |

If users are unsure which workspace to use, they should ask the workspace owner or BIA before creating new items.

## First safe activity for all users

A safe first activity should help users become familiar with Fabric without creating unnecessary risk.

Recommended first activity:

1. Sign in to Fabric.
2. Open the assigned workspace.
3. Confirm whether the workspace is sandbox, department, or BIA production.
4. Review the list of existing items.
5. Open an existing report or sample item.
6. Check the report title, owner, refresh date, and sensitivity label.
7. Apply basic filters or slicers.
8. Do not export, share, or forward screenshots unless permitted.

This activity is suitable for most new users because it focuses on navigation, interpretation, and responsible use.

## First safe activity for Fabric enthusiasts

Fabric enthusiasts who are using a sandbox workspace may continue with a simple hands-on activity using safe data.

Example sandbox activity:

1. Open the sandbox workspace.
2. Locate the approved sample dataset.
3. Create or open a simple Power BI report.
4. Build one or two simple visuals.
5. Save the report using the recommended naming convention.
6. Add a short note explaining the purpose of the report.
7. Treat the output as learning material only.

Sandbox outputs should not be treated as official reports or validated analytics products.

## First safe activity for report developers

Report developers should begin by checking whether an approved semantic model or existing report already exists.

Recommended first activity:

1. Open the correct workspace.
2. Review existing reports and semantic models.
3. Check whether the required business definition already exists.
4. Create a draft report only if reuse is not appropriate.
5. Use clear naming to indicate that the report is a draft or prototype.
6. Validate the numbers with the relevant owner before sharing more widely.

Report developers should avoid creating duplicate semantic models or conflicting KPI definitions unless there is a clear reason.

## First safe activity for data engineering learners

Data engineering learners should start in sandbox unless they are working on an approved department use case.

Recommended first activity:

1. Open the sandbox workspace.
2. Create or open a Lakehouse.
3. Load mocked, synthetic, public, or approved non-sensitive data.
4. Inspect the data structure.
5. Create a simple table.
6. Query the table.
7. Document what was created and what the data represents.

This activity helps learners understand how Fabric stores and exposes data before moving into pipelines, notebooks, or production workflows.

## Naming early work clearly

Early work should be named clearly so others understand its purpose and status.

Recommended naming indicators:

| Indicator | Meaning |
|---|---|
| `sandbox` | Learning or experiment only |
| `draft` | Work in progress |
| `prototype` | Early version for feedback |
| `uat` | Under user validation |
| `prod` | Production or production-facing asset, only where approved |

Example names:

```text
sandbox_course_feedback_report
draft_student_engagement_dashboard
prototype_applicant_persona_model
uat_department_reporting_semantic_model
```

Users should avoid names such as:

```text
final_report
latest_dashboard
new_dataset
test123
copy_of_copy_final
```

## What not to do on first use

New users should avoid:

- Uploading real confidential data into sandbox
- Creating duplicate semantic models without checking existing assets
- Sharing unfinished reports as official outputs
- Setting up refresh schedules without ownership
- Using personal credentials for long-term operational assets
- Publishing directly into BIA production workspaces
- Exporting data or screenshots without checking whether it is allowed
- Treating a successful prototype as production-ready

## First-use checklist

Before completing the first hands-on session, users should confirm:

- [ ] I signed in successfully
- [ ] I opened the correct workspace
- [ ] I know whether the workspace is sandbox, department, or BIA production
- [ ] I understand my workspace role
- [ ] I reviewed existing items before creating anything new
- [ ] I checked whether the data or asset has a sensitivity label
- [ ] I avoided uploading restricted or confidential data into sandbox
- [ ] I named any new work clearly
- [ ] I understand whether my output is experimental, departmental, or production-facing
- [ ] I know who to ask before sharing more widely

## References and further learning

| Resource | Purpose |
|---|---|
| [Microsoft Fabric documentation](https://learn.microsoft.com/en-us/fabric/) | Official starting point for Fabric concepts, workloads, and product capabilities |
| [What is Microsoft Fabric?](https://learn.microsoft.com/en-us/fabric/fundamentals/microsoft-fabric-overview) | Introduces Fabric as an end-to-end analytics platform with integrated experiences |
| [Power BI service basic concepts](https://learn.microsoft.com/en-us/power-bi/fundamentals/service-basic-concepts) | Explains basic concepts such as workspaces, reports, dashboards, and semantic models |
| [Navigate the Power BI service](https://learn.microsoft.com/en-us/power-bi/explore-reports/end-user-experience) | Useful for report consumers learning how to find and open reports, dashboards, and apps |
| [Create a lakehouse, ingest sample data, and build a report](https://learn.microsoft.com/en-us/fabric/data-engineering/tutorial-build-lakehouse) | Microsoft tutorial showing a basic end-to-end lakehouse and reporting activity |

## Next section

Proceed to:

[Persona Pathways](../05-persona-pathways/)
