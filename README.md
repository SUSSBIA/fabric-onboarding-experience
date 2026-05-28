# Fabric Onboarding Experience

This repository provides a structured self-service onboarding experience for Microsoft Fabric users in the University context.

It is designed to help BIA scale Fabric onboarding beyond one-to-one support by giving staff, department representatives, workspace owners, and Fabric enthusiasts a clear pathway to learn, practise, and apply Fabric safely.

## Why this repo exists

As interest in Microsoft Fabric grows across the University, BIA cannot provide high-touch onboarding support to every potential learner or department representative.

This repo therefore acts as an onboarding-at-scale resource.

It helps users understand the foundations before entering Fabric, practise safely in sandbox environments, and follow learning pathways appropriate to their role and maturity level.

The goal is not only to teach users how to use Fabric features, but also to build responsible analytics thinking.

Users should understand:

- What they are allowed to access
- Which workspace they should use
- What data they can use safely
- How shared Fabric capacity is consumed
- When outputs are experimental
- When assets may need review before productionisation
- Who owns the asset after it is created
- Who monitors refresh, connections, and operational issues

## Onboarding philosophy

Fabric onboarding should be layered.

Users should not jump straight into creating reports, Lakehouses, pipelines, notebooks, semantic models, or dataflows without first understanding access, security, licensing, capacity, workspace boundaries, and responsible use.

The recommended onboarding flow is:

```text
Start Here
   ↓
Security, Access and Governance
   ↓
Licensing, Capacity and Compute Awareness
   ↓
Workspace Operating Model
   ↓
Start Using Fabric
   ↓
Persona Pathways
   ↓
Deployment Lifecycle Management
   ↓
Connections, Refresh and Monitoring
   ↓
Data and Semantic Modelling
   ↓
Sandbox Experiments
   ↓
Department Use Case Exploration
   ↓
Review / Productionisation, where applicable
```

## Sandbox-first principle

All learners start in sandbox.

Sandbox workspaces are used for learning, experimentation, and practice using safe data.

Sandbox exercises should use:

- Public data
- Mocked data
- Synthetic data
- Approved non-sensitive data

Sandbox exercises should not use:

- Real confidential institutional data
- Real restricted institutional data
- Student personal data
- Staff personal data
- Financial records
- Donor records
- Operational data from production systems
- Any data that has not been approved for sandbox use

Sandbox outputs are not production assets. They should not be treated as official reports, validated analytics products, operational dashboards, or formal decision-support tools.

## Current Fabric operating model

The current operating model is based on three workspace patterns.

| Workspace Type | Purpose |
|---|---|
| Sandbox Workspace | Learning, experimentation, and practice using safe data |
| Department Workspace | Department-level exploration, prototyping, development, and capability building |
| BIA Production Workspace | BIA-managed production analytics assets |

At this stage, there is no formal shared or central workspace model for cross-department analytics assets. This may evolve as analytics maturity across the University develops.

## Local licensing and capacity context

All staff experience on Fabric is currently powered by the University’s Microsoft Office 365 Education A5 plan, which includes Power BI Pro capabilities.

BIA has provisioned an F64 Fabric capacity for the University’s analytics workloads.

A simple way to understand Fabric capacity is to think of it as buying a fixed amount of electricity for a household. Every action or activity in Fabric consumes compute, just as every appliance consumes electricity.

This means Fabric users should treat capacity as a shared institutional resource.

External collaborators may require:

- Microsoft Entra B2B guest access
- Power BI Pro or Premium Per User licensing review
- Workspace access review
- Sensitivity and sharing review
- Time-bound access planning
- BIA review where needed

## BIA role

BIA acts as the platform steward for the University’s Fabric analytics environment.

In this onboarding context, BIA may be involved in:

- Fabric onboarding design
- Sandbox workspace enablement
- Department workspace guidance
- Tenant-level settings review
- Capacity and workload considerations
- Security and access escalation
- Productionisation review
- BIA production workspace management
- Guidance on semantic models, deployment, refresh, and operational ownership

Requests involving tenant-level settings, capacity-level settings, preview features, external collaboration, elevated permissions, or productionisation should be escalated to BIA for review.

## Repo structure

| Section | Purpose |
|---|---|
| [00 Start Here](./00-start-here/) | Entry point for the onboarding experience |
| [01 Security, Access and Governance](./01-security-access-governance/) | Security, access, sensitivity labels, RLS awareness, and escalation |
| [02 Licensing, Capacity and Compute Awareness](./02-licensing-capacity/) | Staff licensing, Power BI Pro, F64 capacity, and responsible compute use |
| [03 Fabric Workspace Operating Model](./03-workspace-operating-model/) | Sandbox, department, and BIA production workspace patterns |
| [04 Start Using Fabric](./04-start-using-fabric/) | First safe hands-on activities in the sandbox workspace |
| [05 Persona Pathways](./05-persona-pathways/) | Role-based learning tracks for different user groups |
| [06 Deployment Lifecycle Management](./06-deployment-lifecycle-management/) | Movement from sandbox to department workspace to production review |
| [07 Connections, Refresh and Monitoring](./07-connections-refresh-monitoring/) | Connections, credentials, gateways, refresh, monitoring, and failure handling |
| [08 Data and Semantic Modelling](./08-data-and-semantic-modelling/) | Grain, measures, semantic models, RLS, reuse, and AI-ready data |
| [09 Sandbox Experiments](./09-sandbox-experiments/) | Hands-on HDB Resales sandbox experiments |
| [10 Curated Learning Resources](./10-curated-learning-resources/) | Microsoft documentation, Microsoft Learn, and curated video resources |
| [11 Templates and Checklists](./11-templates-checklists/) | Reusable templates and checklists for onboarding and review |
| [Glossary](./glossary.md) | Plain-language definitions of key terms |
| [Roadmap](./roadmap.md) | Current status and planned evolution of the repo |

## Persona pathways

Users should choose the pathway closest to their immediate need.

| Persona | Pathway |
|---|---|
| Report Consumer | [Report Consumer Pathway](./05-persona-pathways/report-consumer/) |
| Report Developer | [Report Developer Pathway](./05-persona-pathways/report-developer/) |
| Data Analyst | [Data Analyst Pathway](./05-persona-pathways/data-analyst/) |
| Data Engineer | [Data Engineer Pathway](./05-persona-pathways/data-engineer/) |
| Data Scientist | [Data Scientist Pathway](./05-persona-pathways/data-scientist/) |
| Department Representative | [Department Representative Pathway](./05-persona-pathways/department-representative/) |
| Workspace Owner | [Workspace Owner Pathway](./05-persona-pathways/workspace-owner/) |
| Fabric Enthusiast | [Fabric Enthusiast Pathway](./05-persona-pathways/fabric-enthusiast/) |

Users may eventually follow more than one pathway, but they should start with the one closest to their role, responsibility, or learning interest.

## HDB Resales Sandbox Series

The first sandbox learning project is the **HDB Resales Sandbox Series**.

It uses public HDB resale flat data as a safe and relatable dataset for onboarding.

The HDB Resales Sandbox Series supports:

- Report consumption
- Dashboard design
- Data analysis
- Semantic modelling
- Lakehouse ingestion and cleaning
- Market segmentation
- Price trend analysis
- Town and flat type comparison
- AI-ready data and semantic layer thinking

The starting Power BI artefact is:

```text
09-sandbox-experiments/hdb-resales/assets/HDB_Resales.pbix
```

This file should be treated as a sandbox learning artefact.

## HDB Resales sandbox experiment catalogue

| No. | Experiment | Main Persona |
|---|---|---|
| 01 | [Report Consumer Walkthrough](./09-sandbox-experiments/hdb-resales/01-report-consumer-walkthrough/) | Report Consumer |
| 02 | [Dashboard Design and Storytelling](./09-sandbox-experiments/hdb-resales/02-dashboard-design-and-storytelling/) | Report Developer |
| 03 | [Semantic Model and KPI Definitions](./09-sandbox-experiments/hdb-resales/03-semantic-model-and-kpi-definitions/) | Report Developer / Data Analyst |
| 04 | [Lakehouse Ingestion and Cleaning](./09-sandbox-experiments/hdb-resales/04-lakehouse-ingestion-and-cleaning/) | Data Engineer |
| 05 | [Market Segmentation](./09-sandbox-experiments/hdb-resales/05-market-segmentation/) | Data Scientist |
| 06 | [Price Trend and Affordability Analysis](./09-sandbox-experiments/hdb-resales/06-price-trend-and-affordability-analysis/) | Data Analyst / Data Scientist |
| 07 | [Town and Flat Type Comparison](./09-sandbox-experiments/hdb-resales/07-town-and-flat-type-comparison/) | Data Analyst |
| 08 | [Geospatial and Location Analysis](./09-sandbox-experiments/hdb-resales/08-geospatial-location-analysis/) | Advanced Analyst |
| 09 | [AI-Ready Data and Semantic Layer](./09-sandbox-experiments/hdb-resales/09-ai-ready-data-and-semantic-layer/) | Advanced User / Fabric Enthusiast |

Some experiment pages may be developed progressively. Check the [roadmap](./roadmap.md) for current status.

## Important cautions

### Sandbox outputs are not official

Sandbox reports, models, notebooks, and datasets are for learning and experimentation.

They should not be used for formal reporting, operational decision-making, or wider sharing unless reviewed and approved.

### Workspace access does not equal data approval

Having access to a workspace does not mean a user is approved to use all data, export all outputs, or share content freely.

Users should still follow sensitivity label guidance, access expectations, and sharing rules.

### Licensing does not override governance

Having Power BI Pro or Fabric access does not override workspace roles, item permissions, data sensitivity, RLS, or production review.

### Getting something to work once is not productionisation

A report, pipeline, notebook, semantic model, or dashboard that works once in sandbox is not automatically ready for department or production use.

Productionisation requires review, validation, ownership, refresh planning, access control, and support arrangements.

## Suggested first steps

New users should start here:

1. Read [Start Here](./00-start-here/)
2. Read [Security, Access and Governance](./01-security-access-governance/)
3. Read [Licensing, Capacity and Compute Awareness](./02-licensing-capacity/)
4. Read [Fabric Workspace Operating Model](./03-workspace-operating-model/)
5. Complete [Start Using Fabric](./04-start-using-fabric/)
6. Choose a pathway from [Persona Pathways](./05-persona-pathways/)
7. Practise using the [HDB Resales Sandbox Series](./09-sandbox-experiments/)

## Status

This repository is evolving.

Current focus:

- Establish foundation onboarding materials
- Build persona pathways
- Develop the HDB Resales Sandbox Series
- Add reusable templates and checklists
- Curate Microsoft documentation, Microsoft Learn, and video resources
- Prepare the repo for internal sharing and onboarding at scale

See the [roadmap](./roadmap.md) for the current build status and planned next steps.
