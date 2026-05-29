# Start Here

Welcome to the Fabric Onboarding Guide.

This repo helps learners understand how to start using Microsoft Fabric safely, progressively, and responsibly.

It provides a structured self-service pathway for users who need to learn Fabric through practical, role-based guidance and sandbox activities.

## Why this repo exists

Microsoft Fabric is a powerful analytics platform, but successful adoption depends on more than tool access.

Users need to understand:

* What they are allowed to access
* Which workspace they should use
* What data they can use safely
* How shared capacity is consumed
* How to practise without using sensitive data
* When outputs should remain experimental
* When a report, model, Lakehouse, pipeline, notebook, or dashboard needs review before wider use
* Who owns the asset after it is created
* Who monitors refresh, connections, and operational issues

This repo helps learners build those foundations before moving into hands-on work.

## Why onboarding is layered

Microsoft Fabric is not just a reporting tool.

It is a shared analytics platform that may involve reports, semantic models, Lakehouses, pipelines, notebooks, dataflows, warehouses, connections, refresh schedules, and institutional data.

Because of this, learners should not jump straight into creating Fabric items without first understanding the foundations.

The onboarding is layered so that learners move progressively from awareness to safe hands-on use.

![Layered Fabric onboarding journey](../assets/images/layered-fabric-onboarding-journey.png)

## Repo versus Fabric Sandbox Workspace

The GitHub repo and the Fabric Sandbox Workspace serve different purposes.

| Area                     | Purpose                                                                                                       |
| ------------------------ | ------------------------------------------------------------------------------------------------------------- |
| GitHub repo              | Stores onboarding instructions, README files, templates, checklists, source references, and learning guidance |
| Fabric Sandbox Workspace | Hosts the working artefacts that learners open, run, edit, copy, and practise with                            |

The repo explains what to do.

The Fabric Sandbox Workspace is where the hands-on work happens.

## Who this repo is for

This repo is intended for several learner groups.

| User Group                 | How this repo helps                                                                                        |
| -------------------------- | ---------------------------------------------------------------------------------------------------------- |
| New Fabric users           | Understand the basics before using Fabric                                                                  |
| Report consumers           | Learn how to access, filter, and interpret reports responsibly                                             |
| Report developers          | Learn how to build or improve Power BI reports and dashboards                                              |
| Department representatives | Understand how department use cases, ownership, and workspace boundaries fit into the operating model      |
| Fabric enthusiasts         | Practise safely in sandbox workspaces using safe data                                                      |
| Data analysts              | Build analytical confidence through guided activities and reusable patterns                                |
| Data engineers             | Learn common Fabric data patterns such as Lakehouse, pipeline, notebook, connection, and refresh workflows |
| Data scientists            | Explore advanced analytics experiments using public, mocked, synthetic, or approved non-sensitive data     |
| Workspace owners           | Understand ownership, access, refresh, review, and operational responsibilities                            |
| BIA colleagues             | Use the guide to support consistent Fabric onboarding and safe adoption                                    |

## How to use this repo

Start with the foundation sections.

Then choose the persona pathway that best matches your role or learning need.

After that, complete the relevant sandbox experiments in the assigned Fabric Sandbox Workspace.

Recommended sequence:

1. Start Here
2. Security, Access and Governance
3. Licensing, Capacity and Compute Awareness
4. Workspace Operating Model
5. Start Using Fabric
6. Persona Pathways
7. Sandbox Experiments
8. Templates and Checklists
9. Department Use Case Exploration, where applicable
10. Review or Productionisation, where applicable

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
Sandbox Experiments
   ↓
Templates and Checklists
   ↓
Department Use Case Exploration, where applicable
   ↓
Review / Productionisation, where applicable
```

## Two connected learning tracks

This repo supports two connected learning tracks.

### Track 1: Fabric Onboarding

This track helps learners understand how to access, navigate, and use Fabric safely.

It covers:

* Security and access expectations
* Licensing and capacity awareness
* Workspace operating model
* First safe activities in Fabric
* Persona-based pathways
* Deployment and lifecycle expectations
* Connections, credentials, refresh, and monitoring responsibilities
* Data and semantic modelling basics

### Track 2: Analytics Thinking Sandbox

This track helps learners go beyond basic tool familiarity.

It provides guided sandbox experiments that help learners practise analytics, BI, semantic modelling, data engineering, data science, and AI-ready data thinking using safe datasets.

The aim is not only to teach Fabric features, but also to develop better analytics judgement.

## Sandbox as a safe learning entry point

Sandbox workspaces provide a safe entry point for learners who may not yet have a formal department use case.

Sandbox experiments should use only:

* Public data
* Mocked data
* Synthetic data
* Approved non-sensitive data

Sandbox outputs should not be treated as official reports, validated analytics products, production dashboards, or formal decision-support tools.

## Workspace operating model in brief

Fabric work should happen in the correct workspace.

| Workspace Type           | Purpose                                                                                      |
| ------------------------ | -------------------------------------------------------------------------------------------- |
| Personal Workspace       | Individual exploration and private drafts                                                    |
| Sandbox Workspace        | Guided onboarding and safe experimentation                                                   |
| Department Workspace     | Department-level exploration, prototyping, and working assets                                |
| BIA Production Workspace | BIA-managed production analytics assets with direct workspace access restricted to BIA users |

Simple rule:

```text
Personal workspace = private draft
Sandbox workspace = safe learning
Department workspace = department-owned working asset
BIA production workspace = governed production asset restricted to BIA workspace users
```

Non-BIA users should not be granted direct BIA Production Workspace membership.

Where approved production outputs need to be shared with non-BIA users, sharing should happen through approved report or app sharing channels.

## Before you start

Before doing hands-on work in Fabric, make sure you can answer these questions:

* Do I know which workspace I should use?
* Do I know whether I am in a personal, sandbox, department, or BIA production workspace?
* Do I understand my workspace role?
* Do I know what data I am allowed to use?
* Do I understand the sensitivity expectations for the data or asset?
* Do I know whether my output is experimental, department-facing, or production-facing?
* Do I know who owns the asset after it is created?
* Do I know whether there is a deputy owner for department workspace work?
* Do I know who will maintain the connection or refresh?
* Do I know who to contact if I need help?

## Important reminders

* Hands-on onboarding work should happen in the assigned Fabric Sandbox Workspace
* Sandbox outputs are learning artefacts
* Sandbox outputs are not official reports
* Sandbox outputs should not be copied into department or production workspaces without review
* Department workspace requests should identify both a workspace owner and deputy workspace owner
* BIA Production Workspaces are restricted to BIA users
* Non-BIA users should consume approved production outputs through approved report or app sharing channels
* Workspace access does not automatically mean permission to export, reuse, or redistribute data
* Confidential or restricted institutional data should not be used in sandbox unless explicitly approved

## References and further learning

| Resource                                                                                                                   | Purpose                                                                                    |
| -------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ |
| [Microsoft Fabric documentation](https://learn.microsoft.com/en-us/fabric/)                                                | Official Microsoft documentation for Fabric concepts, workloads, and platform capabilities |
| [What is Microsoft Fabric?](https://learn.microsoft.com/en-us/fabric/fundamentals/microsoft-fabric-overview)               | Introduction to Fabric as an end-to-end analytics platform                                 |
| [Power BI service basic concepts](https://learn.microsoft.com/en-us/power-bi/fundamentals/service-basic-concepts)          | Helpful for users new to workspaces, reports, dashboards, and semantic models              |
| [Microsoft Learn: Get started with Microsoft Fabric](https://learn.microsoft.com/en-us/training/paths/get-started-fabric/) | Structured Microsoft Learn pathway for users beginning with Fabric                         |

## Next section

Proceed to:

[Security, Access and Governance](../01-security-access-governance/)
