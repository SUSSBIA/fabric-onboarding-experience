# Fabric Workspace Operating Model

This section explains where users should work in Microsoft Fabric and how the current workspace model is organised.

The workspace model is important because not every Fabric workspace has the same purpose. A sandbox workspace, a department workspace, and a BIA production workspace carry different expectations for access, data use, reliability, sharing, and production readiness.

## Current operating model

The current Fabric operating model is based on three workspace patterns:

1. Sandbox Workspaces
2. Department Workspaces
3. BIA Production Workspaces

At this stage, there is no formal shared or central workspace model for cross-department analytics assets. This may evolve as analytics maturity across the University develops.

![Placeholder: Fabric workspace operating model](../assets/images/fabric-workspace-operating-model.png)

> Image placeholder: A simple three-part diagram showing Sandbox Workspace for learning and experimentation, Department Workspace for department-level exploration and development, and BIA Production Workspace for BIA-managed production analytics assets.

## Why the workspace model matters

Users should not treat all workspaces the same.

A workspace determines:

- Who can access the content
- What type of work should happen there
- Whether the output is experimental, departmental, or production-facing
- Whether sensitive data may be used
- Whether refresh, monitoring, and operational ownership are required
- Whether BIA review is needed before wider sharing or production use

Microsoft Fabric workspaces are collaboration areas where users create and manage collections of items such as Lakehouses, Warehouses, reports, and task flows. Workspace roles control what users can do within a specific workspace. This means the workspace is both a collaboration boundary and an access control boundary.

## Sandbox Workspace

Sandbox workspaces are used for learning, experimentation, and practice.

They provide a safe entry point for Fabric enthusiasts, learners, and department representatives who want to explore Fabric capabilities before applying them to actual department use cases.

Sandbox workspaces are suitable for:

- Guided onboarding activities
- Hands-on practice
- Trying out Fabric features
- Learning with mocked or synthetic data
- Exploring reports, semantic models, Lakehouses, pipelines, notebooks, and dataflows
- Building confidence before working in department workspaces

Sandbox workspaces should generally use:

- Mocked data
- Synthetic data
- Public data
- Approved non-sensitive data

Sandbox outputs should not be treated as official reports, validated analytics products, or production-ready assets.

## Department Workspace

Department workspaces are provided to nominated department representatives as their working area in Fabric.

They support department-level exploration, prototyping, development, and capability building.

Department workspaces may be used for:

- Department-specific exploration
- Prototyping reports or analytics use cases
- Practising with approved department data
- Developing early-stage analytics assets
- Collaborating with BIA where support is required
- Building local Fabric capability over time

Department workspaces should not automatically be treated as production workspaces.

An asset created in a department workspace may still require review before it is used for formal reporting, wider organisational sharing, or operational decision-making.

## BIA Production Workspace

BIA production workspaces are reserved for BIA-managed production assets.

This means:

- BIA owns or manages the production asset
- The asset has gone through appropriate review and validation
- Access is more tightly controlled
- Refreshes and dependencies are monitored
- Changes follow review and release practices
- The output is intended for formal or wider organisational use

Users should not move or publish assets into BIA production workspaces without the appropriate review and approval process.

## Current-state and future-state

The current operating model does not assume a separate shared or central workspace for cross-department analytics assets.

However, as analytics maturity grows, the University may eventually need more formal patterns for:

- Shared semantic models
- Certified data products
- Cross-department analytics assets
- Common KPI definitions
- Reusable curated datasets
- AI-ready data products
- Governed self-service analytics

These are future maturity considerations rather than current onboarding assumptions.

## Workspace journey

A typical user journey may look like this:

```text
Sandbox Workspace
   ↓
Department Workspace
   ↓
Review and validation
   ↓
BIA Production Workspace, only where applicable
```

Not every department workspace asset needs to become a BIA production asset.

Some assets may remain as department-level working assets. Productionisation is only relevant when the asset is intended for formal reporting, wider organisational use, monitored operation, or BIA-managed production deployment.

## Workspace expectations by type

| Workspace Type | Main Purpose | Typical Users | Data Expectation | Output Status |
|---|---|---|---|---|
| Sandbox Workspace | Learning and experimentation | Fabric enthusiasts, learners, department representatives | Mocked, synthetic, public, or approved non-sensitive data | Experimental |
| Department Workspace | Department-level exploration and development | Department representatives and approved collaborators | Approved department data, subject to sensitivity and access rules | Department-level working asset |
| BIA Production Workspace | BIA-managed production analytics assets | BIA and approved users | Validated and governed data | Production asset |

## Workspace ownership

Every workspace should have a clear owner or responsible group.

Workspace ownership matters because someone must be accountable for:

- Access requests
- User role assignment
- Data use expectations
- Workspace organisation
- Asset clean-up
- Connection and refresh ownership
- Escalation when something breaks
- Review before wider sharing or production use

For department workspaces, the department representative or nominated owner should coordinate with BIA when there are questions about access, capacity, sensitivity, or productionisation.

For BIA production workspaces, BIA retains stronger control over access, change, monitoring, and release practices.

## Workspace creation and access

In the current operating model, users should not assume they can freely create or manage workspaces.

Workspace creation and access may be controlled by BIA through tenant-level or administrator-managed settings.

Requests for new workspaces, role changes, elevated permissions, or feature access should be escalated to BIA for review.

BIA will assess requests based on:

- Business or learning purpose
- Workspace type
- Data sensitivity
- User role required
- Capacity impact
- Governance requirements
- Operational ownership

## Minimum checklist before using a workspace

Before working in a Fabric workspace, users should confirm:

- [ ] I know whether this is a sandbox, department, or BIA production workspace
- [ ] I understand the purpose of the workspace
- [ ] I understand my workspace role
- [ ] I know what data I am allowed to use
- [ ] I know whether the data or asset has a sensitivity label
- [ ] I know whether the output is experimental, departmental, or production-facing
- [ ] I know who owns the workspace
- [ ] I know who to contact for access or role changes
- [ ] I know whether BIA review is needed before wider sharing or production use

## References and further learning

| Resource | Purpose |
|---|---|
| [Workspaces in Microsoft Fabric and Power BI](https://learn.microsoft.com/en-us/fabric/fundamentals/workspaces) | Explains how workspaces are used to collaborate and manage Fabric items |
| [Roles in workspaces in Microsoft Fabric](https://learn.microsoft.com/en-us/fabric/fundamentals/roles-workspaces) | Explains workspace roles such as Admin, Member, Contributor, and Viewer |
| [Give users access to workspaces](https://learn.microsoft.com/en-us/fabric/fundamentals/give-access-workspaces) | Explains how users can be granted workspace roles |
| [Workspace admin settings](https://learn.microsoft.com/en-us/fabric/admin/portal-workspace) | Explains admin-controlled settings such as workspace creation and cross-workspace semantic model use |
| [Manage workspaces](https://learn.microsoft.com/en-us/fabric/admin/portal-workspaces) | Provides admin guidance for managing workspaces and assigning workspaces to capacities |

## Next section

Proceed to:

[Start Using Fabric](../04-start-using-fabric/)
