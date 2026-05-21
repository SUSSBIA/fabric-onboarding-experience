# Start Here

Welcome to the Fabric Onboarding Experience.

This repository is designed to support Microsoft Fabric onboarding at scale. As interest in Fabric grows across the University, BIA cannot provide high-touch, one-to-one onboarding for every potential learner, department representative, or Fabric enthusiast.

Instead, this repo provides a structured self-service pathway for users to learn, practise, and apply Fabric safely and progressively.

## Why this repo exists

Microsoft Fabric is a powerful analytics platform, but successful adoption depends on more than tool access.

Users need to understand how Fabric is governed, where they should work, what data they can use, how shared capacity is consumed, and when outputs should remain experimental versus when they require review.

This repo helps users answer:

- What am I allowed to access?
- Which workspace should I use?
- What data can I use safely?
- How do I start using Fabric?
- Which learning pathway should I follow?
- How do I practise without using sensitive data?
- When does a report, model, or pipeline need review before wider use?
- Who owns the asset after it is created?
- Who monitors refresh, connections, and operational issues?

## Why this onboarding is layered

Microsoft Fabric is not just a reporting tool. It is a shared analytics platform that may involve reports, semantic models, Lakehouses, pipelines, notebooks, dataflows, warehouses, connections, refresh schedules, and institutional data.

Because of this, users should not jump straight into creating Fabric items without first understanding the foundations.

The onboarding is layered so that users move progressively from awareness to safe hands-on use.

![Layered Fabric onboarding journey](../assets/images/layered-fabric-onboarding-journey.png)

## Who this repo is for

This repo is intended for several groups of users.

| User Group | How this repo helps |
|---|---|
| New Fabric users | Understand the basics before using Fabric |
| Report consumers | Learn how to access and interpret approved reports responsibly |
| Report developers | Learn how to work with reports, semantic models, access expectations, and deployment considerations |
| Department representatives | Understand how department workspaces fit into the current operating model |
| Fabric enthusiasts | Practise safely in sandbox workspaces using safe data |
| Data analysts | Build analytical confidence through guided activities and reusable patterns |
| Data engineers | Learn common Fabric data patterns such as Lakehouse, pipeline, notebook, connection, and refresh workflows |
| Data scientists | Explore advanced analytics experiments using synthetic or approved data |
| Workspace owners | Understand ownership, access, refresh, review, and operational responsibilities |
| BIA colleagues | Reuse onboarding materials to support Fabric adoption at scale |

## How to use this repo

If you are new to Fabric, start with the foundation sections:

1. Security, Access and Governance
2. Licensing, Capacity and Compute Awareness
3. Fabric Workspace Operating Model

After that, continue to:

4. Start Using Fabric
5. Persona Pathways
6. Deployment Lifecycle Management
7. Connections, Refresh and Monitoring
8. Data and Semantic Modelling
9. Sandbox Experiments

## Recommended onboarding flow

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
Persona Pathway
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

## Two connected learning tracks

This repo supports two connected tracks.

### Track 1: Fabric Onboarding

This track helps users understand how to access, navigate, and use Fabric safely.

It covers:

- Security and access expectations
- Licensing and capacity awareness
- Workspace operating model
- First safe activities in Fabric
- Persona-based pathways
- Deployment and lifecycle expectations
- Connections, credentials, refresh, and monitoring responsibilities
- Data and semantic modelling basics

### Track 2: Analytics Thinking Sandbox

This track is for users who want to go beyond basic tool familiarity.

It provides guided sandbox experiments that help users practise analytics, BI, semantic modelling, data engineering, data science, and AI-ready data thinking using safe datasets.

The aim is not only to teach Fabric features, but also to develop better analytics judgement.

## Sandbox as an entry point for enthusiasts

Sandbox workspaces provide a safe entry point for Fabric enthusiasts and learners who may not yet have a formal department use case.

Sandbox experiments should use:

- Mocked data
- Synthetic data
- Public data
- Approved non-sensitive data

Sandbox outputs should not be treated as official reports, validated analytics products, or production-ready assets.

## Current operating model in brief

The current Fabric operating model is based on three workspace patterns.

| Workspace Type | Purpose |
|---|---|
| Sandbox Workspace | Learning, experimentation, and practice using safe data |
| Department Workspace | Department-level exploration, development, and capability building |
| BIA Production Workspace | BIA-managed production analytics assets |

At this stage, there is no formal shared or central workspace model for cross-department analytics assets. This may evolve as analytics maturity across the University develops.

## Before you start

Before doing hands-on work in Fabric, make sure you can answer these questions:

- Do I know which workspace I should use?
- Do I know whether I am in a sandbox, department, or production workspace?
- Do I understand my workspace role?
- Do I know what data I am allowed to use?
- Do I understand the sensitivity label applied to the data or asset?
- Do I know whether my output is experimental or production-facing?
- Do I know who owns the asset after it is created?
- Do I know who will maintain the connection or refresh?
- Do I know who to contact if I need help?

## References and further learning

| Resource | Purpose |
|---|---|
| [Microsoft Fabric documentation](https://learn.microsoft.com/en-us/fabric/) | Official Microsoft documentation for Fabric concepts, workloads, and platform capabilities |
| [What is Microsoft Fabric?](https://learn.microsoft.com/en-us/fabric/fundamentals/microsoft-fabric-overview) | Introduction to Fabric as an end-to-end analytics platform |
| [Power BI service basic concepts](https://learn.microsoft.com/en-us/power-bi/fundamentals/service-basic-concepts) | Helpful for users new to workspaces, reports, dashboards, and semantic models |
| [Microsoft Learn: Get started with Microsoft Fabric](https://learn.microsoft.com/en-us/training/paths/get-started-fabric/) | Structured Microsoft Learn pathway for users beginning with Fabric |

## Next section

Proceed to:

[Security, Access and Governance](../01-security-access-governance/)
