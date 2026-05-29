# Fabric Onboarding Guide

This repo provides a learner-facing onboarding guide for Microsoft Fabric.

It is designed to help users understand how to start safely, choose the right learning pathway, practise in a Fabric Sandbox Workspace, and recognise when an artefact should remain sandbox or move towards department or production review.

The guide is especially useful for users who need to learn Fabric through practical, role-based activities rather than product documentation alone.

## Purpose

The purpose of this repo is to support structured Fabric onboarding.

It helps learners understand:

* How Fabric fits into the analytics operating model
* How workspace boundaries work
* Which pathway to follow based on their role
* How to practise safely using sandbox experiments
* How to use public or approved non-sensitive data for learning
* How to document assumptions, caveats, and limitations
* How to avoid treating sandbox outputs as official reports
* When BIA review is needed

This repo is a guide and learning resource. It is not the place where learners perform the hands-on work.

Hands-on work should happen in the assigned Fabric Sandbox Workspace.

## Repo versus Fabric Sandbox Workspace

The GitHub repo and the Fabric Sandbox Workspace serve different purposes.

| Area                     | Purpose                                                                                                       |
| ------------------------ | ------------------------------------------------------------------------------------------------------------- |
| GitHub repo              | Stores onboarding instructions, README files, templates, checklists, source references, and learning guidance |
| Fabric Sandbox Workspace | Hosts the working artefacts that learners open, run, edit, copy, and practise with                            |

The repo explains what to do.

The Fabric Sandbox Workspace is where the hands-on work happens.

## Accessing Fabric artefacts

This repo does not contain direct links to internal Fabric workspaces, reports, semantic models, Lakehouses, or other internal artefacts.

To access Microsoft Fabric:

```text
https://app.fabric.microsoft.com/
```

Sign in using your University account and follow the instructions in the relevant onboarding section or sandbox experiment.

For hands-on activities, learners will use the assigned Fabric Sandbox Workspace. The specific workspace and artefact access details will be provided through internal BIA onboarding channels.

If you cannot find the assigned workspace or artefact, check with the workspace owner or BIA contact.

## Workspace operating principle

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

## Who this guide is for

This guide supports several learner groups.

| Learner Group             | Typical Need                                                          |
| ------------------------- | --------------------------------------------------------------------- |
| Report Consumer           | View, filter, and interpret reports responsibly                       |
| Report Developer          | Build or improve Power BI reports and dashboards                      |
| Data Analyst              | Explore data, develop insights, and support analytical interpretation |
| Data Engineer             | Load, prepare, transform, and manage data assets                      |
| Data Scientist            | Build models, experiments, and analytical outputs responsibly         |
| Department Representative | Frame use cases, clarify needs, and coordinate department ownership   |
| Workspace Owner           | Manage workspace purpose, access, ownership, and continuity           |
| Fabric Enthusiast         | Explore Fabric capabilities safely and progressively                  |

## How to use this repo

Start with the foundation sections, then choose a persona pathway, then complete the relevant sandbox experiments.

Recommended sequence:

1. Start with the foundation sections
2. Read the workspace operating model
3. Choose a persona pathway
4. Complete the relevant HDB Resales sandbox experiment
5. Use templates and checklists to document your work
6. Ask BIA if the work may move beyond sandbox

## Repo structure

```text
fabric-onboarding-guide/
├── README.md
├── 00-start-here/
├── 01-security-access-governance/
├── 02-licensing-capacity/
├── 03-workspace-operating-model/
├── 04-start-using-fabric/
├── 05-persona-pathways/
│   ├── report-consumer/
│   ├── report-developer/
│   ├── data-analyst/
│   ├── data-engineer/
│   ├── data-scientist/
│   ├── department-representative/
│   ├── workspace-owner/
│   └── fabric-enthusiast/
├── 06-deployment-lifecycle-management/
├── 07-connections-refresh-monitoring/
├── 08-data-and-semantic-modelling/
├── 09-sandbox-experiments/
│   └── hdb-resales/
├── 10-curated-learning-resources/
├── 11-templates-checklists/
├── CONTRIBUTING.md
└── assets/
    └── images/
```

## Foundation sections

| Section                                                               | Purpose                                                                         |
| --------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| [Start Here](./00-start-here/)                                        | Introduces the onboarding guide and how to begin                                |
| [Security, Access and Governance](./01-security-access-governance/)   | Covers safe access, sharing, sensitivity, and governance expectations           |
| [Licensing, Capacity and Compute Awareness](./02-licensing-capacity/) | Explains licensing, capacity, and compute considerations at a learner level     |
| [Workspace Operating Model](./03-workspace-operating-model/)          | Explains personal, sandbox, department, and BIA production workspace boundaries |
| [Start Using Fabric](./04-start-using-fabric/)                        | Helps learners begin navigating and using Fabric safely                         |

## Persona pathways

Persona pathways explain what different learner groups should know.

| Pathway                   | Start Here                                                                            |
| ------------------------- | ------------------------------------------------------------------------------------- |
| Report Consumer           | [Report Consumer Pathway](./05-persona-pathways/report-consumer/)                     |
| Report Developer          | [Report Developer Pathway](./05-persona-pathways/report-developer/)                   |
| Data Analyst              | [Data Analyst Pathway](./05-persona-pathways/data-analyst/)                           |
| Data Engineer             | [Data Engineer Pathway](./05-persona-pathways/data-engineer/)                         |
| Data Scientist            | [Data Scientist Pathway](./05-persona-pathways/data-scientist/)                       |
| Department Representative | [Department Representative Pathway](./05-persona-pathways/department-representative/) |
| Workspace Owner           | [Workspace Owner Pathway](./05-persona-pathways/workspace-owner/)                     |
| Fabric Enthusiast         | [Fabric Enthusiast Pathway](./05-persona-pathways/fabric-enthusiast/)                 |

Persona pathway READMEs act as curriculum maps. They explain role purpose, learning objectives, key principles, expected evidence, and recommended hands-on experiments.

They should not duplicate detailed step-by-step sandbox exercises.

## Sandbox experiments

Sandbox experiments provide hands-on practice.

| Sandbox Series                                                      | Purpose                                                                                                                                            |
| ------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| [HDB Resales Sandbox Series](./09-sandbox-experiments/hdb-resales/) | Public-data learning project for report consumption, dashboard design, data analysis, data engineering, semantic modelling, and advanced analytics |

Sandbox experiment READMEs act as lesson worksheets. They provide step-by-step hands-on activities, outputs, reflection questions, and completion evidence.

## HDB Resales Sandbox Series

The HDB Resales Sandbox Series is the first hands-on learning project in this repo.

It uses public HDB resale flat data as a safe, relatable, and practical dataset for learning Microsoft Fabric.

The series supports:

* Report consumption
* Dashboard design
* Semantic model and KPI review
* Lakehouse ingestion and cleaning
* Market segmentation
* Price trend and affordability analysis
* Town and flat type comparison
* Geospatial and location analysis
* AI-ready data and semantic layer thinking

Start here:

[HDB Resales Sandbox Series](./09-sandbox-experiments/hdb-resales/)

## Templates and checklists

Reusable templates and checklists are stored in:

[Templates and Checklists](./11-templates-checklists/)

These resources help learners and reviewers document:

* Report context
* Insight summaries
* Use case framing
* Workspace inventory
* Workspace health
* Model cards
* Release notes
* Refresh failures
* Sandbox readiness
* Workspace access
* Report review
* Semantic model review
* RLS testing
* Refresh monitoring
* Productionisation readiness
* External collaborator review

## Important governance reminders

* Sandbox outputs are learning artefacts
* Sandbox outputs are not official reports
* Sandbox outputs should not be copied into department or production workspaces without review
* Department workspaces require clear ownership
* Department workspace requests should identify both a workspace owner and deputy workspace owner
* BIA Production Workspaces are restricted to BIA users
* Non-BIA users should consume approved production outputs through approved report/app sharing channels
* Workspace access does not automatically mean permission to export, reuse, or redistribute data
* Confidential or restricted institutional data should not be used in sandbox unless explicitly approved

## When to ask BIA

Ask BIA when:

* You are unsure which workspace should be used
* A sandbox output may become a department use case
* A department workspace request does not have both an owner and deputy owner
* A department asset may become production-facing
* Confidential or restricted data may be involved
* External collaborators need access
* RLS may be required
* A semantic model is intended for reuse
* A report is intended for wider sharing
* A connection, gateway, or refresh setup needs operational support
* A tenant-level or capacity-level setting is involved
* A non-BIA user needs access to an approved BIA production output

## Maintainer and contributor notes

This repo should remain learner-facing and public-safe.

Repo maintenance guidance, including public repo safety rules, should be placed in:

[CONTRIBUTING.md](./CONTRIBUTING.md)

## Getting started

Begin with:

[Start Here](./00-start-here/)
