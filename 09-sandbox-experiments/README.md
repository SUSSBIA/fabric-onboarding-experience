# Sandbox Experiments

Sandbox experiments provide guided hands-on practice activities for Microsoft Fabric onboarding.

This section helps learners find practical activities that can be completed safely in the assigned Fabric Sandbox Workspace.

Each sandbox series uses a safe dataset, a clear learning purpose, and guided activities that help learners practise Fabric skills without using confidential institutional data.

The first sandbox series is the **HDB Resales Sandbox Series**.

## Purpose of sandbox experiments

Sandbox experiments help learners practise Fabric skills in a safe environment before moving into department or production-facing work.

Through sandbox experiments, learners can practise:

* Opening and interpreting reports
* Building or improving dashboards
* Exploring data
* Preparing data for analysis
* Understanding semantic models and measures
* Loading and transforming data
* Running notebooks or basic modelling activities
* Documenting assumptions, caveats, and limitations
* Deciding whether an idea should remain sandbox or move towards a real use case

Sandbox experiments are learning activities. They are not production projects.

## Sandbox-first principle

All hands-on onboarding activities should start in the assigned Fabric Sandbox Workspace.

Sandbox experiments should use only:

* Public data
* Mocked data
* Synthetic data
* Approved non-sensitive data

Sandbox experiments should not use:

* Real confidential institutional data
* Real restricted institutional data
* Student personal data
* Staff personal data
* Financial records
* Donor records
* Operational data from production systems
* Any data that has not been approved for sandbox use

Sandbox outputs are for learning and experimentation only. They should not be treated as official reports, validated analytics products, operational dashboards, production semantic models, or formal decision-support tools.

## Workspace boundary for sandbox experiments

Sandbox experiments should be completed in the assigned Fabric Sandbox Workspace.

They should not be completed in a personal workspace, department workspace, or BIA production workspace unless the experiment explicitly says so.

| Workspace Type           | Use for Sandbox Experiments? | Reason                                                                                                           |
| ------------------------ | ---------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| Personal Workspace       | No, unless instructed        | Personal workspaces are for private drafts and individual exploration, not shared onboarding exercises           |
| Sandbox Workspace        | Yes                          | This is the correct place for guided onboarding and safe experimentation                                         |
| Department Workspace     | No, unless approved          | Department workspaces are for department-owned use cases and working assets                                      |
| BIA Production Workspace | No                           | Production workspaces are restricted to BIA users and are for governed, validated, BIA-managed production assets |

## Repo versus Fabric Sandbox Workspace

The GitHub repo and the Fabric Sandbox Workspace serve different purposes.

| Area                     | Purpose                                                                                                       |
| ------------------------ | ------------------------------------------------------------------------------------------------------------- |
| GitHub repo              | Stores learning instructions, README files, templates, checklists, source references, and onboarding guidance |
| Fabric Sandbox Workspace | Hosts the working artefacts that learners open, run, edit, copy, and practise with                            |

The repo explains what to do.

The Fabric Sandbox Workspace is where the hands-on work happens.

## Accessing sandbox artefacts

Hands-on artefacts are accessed through the assigned Fabric Sandbox Workspace.

The actual workspace and artefact links are shared through internal BIA onboarding channels and are not published in this public repo.

Each sandbox series or experiment page provides the specific instructions for the report, Lakehouse, notebook, semantic model, or other artefact used in that activity.

## How to find a sandbox experiment

Use this section to find the sandbox series and activity that matches your pathway or learning need.

```text
09-sandbox-experiments/
├── README.md
└── hdb-resales/
    ├── README.md
    ├── data/
    ├── notebooks/
    ├── templates/
    ├── model-output/
    ├── 01-report-consumer-walkthrough/
    ├── 02-dashboard-design-and-storytelling/
    ├── 03-semantic-model-and-kpi-definitions/
    ├── 04-lakehouse-ingestion-and-cleaning/
    ├── 05-market-segmentation/
    ├── 06-price-trend-and-affordability-analysis/
    ├── 07-town-and-flat-type-comparison/
    ├── 08-geospatial-location-analysis/
    └── 09-ai-ready-data-and-semantic-layer/
```

Each series folder contains the guidance and supporting files for a specific sandbox learning project.

## Available sandbox series

| Series                                       | Purpose                                                                                                                                            | Status         |
| -------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------- |
| [HDB Resales Sandbox Series](./hdb-resales/) | Public-data learning project for report consumption, dashboard design, data analysis, data engineering, semantic modelling, and advanced analytics | In development |

## Current sandbox experiment catalogue

| Series      | Experiment                                                                                            | Main Persona                      | Status  |
| ----------- | ----------------------------------------------------------------------------------------------------- | --------------------------------- | ------- |
| HDB Resales | [01 Report Consumer Walkthrough](./hdb-resales/01-report-consumer-walkthrough/)                       | Report Consumer                   | Drafted |
| HDB Resales | [02 Dashboard Design and Storytelling](./hdb-resales/02-dashboard-design-and-storytelling/)           | Report Developer                  | Drafted |
| HDB Resales | [03 Semantic Model and KPI Definitions](./hdb-resales/03-semantic-model-and-kpi-definitions/)         | Report Developer / Data Analyst   | Planned |
| HDB Resales | [04 Lakehouse Ingestion and Cleaning](./hdb-resales/04-lakehouse-ingestion-and-cleaning/)             | Data Engineer                     | Planned |
| HDB Resales | [05 Market Segmentation](./hdb-resales/05-market-segmentation/)                                       | Data Scientist                    | Planned |
| HDB Resales | [06 Price Trend and Affordability Analysis](./hdb-resales/06-price-trend-and-affordability-analysis/) | Data Analyst / Data Scientist     | Planned |
| HDB Resales | [07 Town and Flat Type Comparison](./hdb-resales/07-town-and-flat-type-comparison/)                   | Data Analyst                      | Planned |
| HDB Resales | [08 Geospatial and Location Analysis](./hdb-resales/08-geospatial-location-analysis/)                 | Advanced Analyst                  | Planned |
| HDB Resales | [09 AI-Ready Data and Semantic Layer](./hdb-resales/09-ai-ready-data-and-semantic-layer/)             | Advanced User / Fabric Enthusiast | Planned |

## How sandbox experiments connect to persona pathways

Persona pathways explain what learners should understand for their role.

Sandbox experiments provide the hands-on practice.

| Persona Pathway                                                                | Recommended Starting Point                                                                                      |
| ------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------- |
| [Report Consumer](../05-persona-pathways/report-consumer/)                     | [HDB Resales: Report Consumer Walkthrough](./hdb-resales/01-report-consumer-walkthrough/)                       |
| [Report Developer](../05-persona-pathways/report-developer/)                   | [HDB Resales: Dashboard Design and Storytelling](./hdb-resales/02-dashboard-design-and-storytelling/)           |
| [Data Analyst](../05-persona-pathways/data-analyst/)                           | [HDB Resales: Price Trend and Affordability Analysis](./hdb-resales/06-price-trend-and-affordability-analysis/) |
| [Data Engineer](../05-persona-pathways/data-engineer/)                         | [HDB Resales: Lakehouse Ingestion and Cleaning](./hdb-resales/04-lakehouse-ingestion-and-cleaning/)             |
| [Data Scientist](../05-persona-pathways/data-scientist/)                       | [HDB Resales: Market Segmentation](./hdb-resales/05-market-segmentation/)                                       |
| [Department Representative](../05-persona-pathways/department-representative/) | [HDB Resales: Report Consumer Walkthrough](./hdb-resales/01-report-consumer-walkthrough/) and Use Case Canvas   |
| [Workspace Owner](../05-persona-pathways/workspace-owner/)                     | Workspace inventory and workspace health activities                                                             |
| [Fabric Enthusiast](../05-persona-pathways/fabric-enthusiast/)                 | Any beginner experiment based on interest                                                                       |

## Learning levels

Sandbox experiments can support different levels of learning.

| Level        | Focus                                                                                   | Example Activities                                                                |
| ------------ | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| Beginner     | Safe navigation, report interpretation, basic dashboard use                             | Open a report, use slicers, interpret one insight                                 |
| Practitioner | Data preparation, semantic modelling, dashboard design, analytical comparison           | Build visuals, define measures, load data, compare trends                         |
| Advanced     | Modelling, segmentation, geospatial analysis, AI-ready data and semantic layer thinking | Run notebooks, profile clusters, prepare model outputs, document semantic meaning |

Learners should not rush into advanced activities before understanding safe data use, workspace context, and responsible interpretation.

## What each sandbox experiment includes

Each sandbox experiment page guides learners through a practical activity.

Most experiment pages include:

| Section                          | Purpose                                                         |
| -------------------------------- | --------------------------------------------------------------- |
| Experiment purpose               | Explains why the experiment exists                              |
| Learning level                   | Indicates beginner, practitioner, or advanced level             |
| Main persona                     | Identifies the primary learner group                            |
| Required artefacts               | Lists the report, data, notebook, Lakehouse, or template needed |
| Safety reminder                  | Reinforces safe data and sandbox-only expectations              |
| Activities                       | Provides step-by-step learning tasks                            |
| Completion evidence              | States what the learner should produce                          |
| Related templates and checklists | Links to reusable documentation aids                            |
| Next experiment                  | Points the learner forward                                      |

## Naming convention for sandbox work

Use clear names that show the work is exploratory.

Recommended examples:

```text
sandbox_hdb_resales_report
sandbox_hdb_resales_semantic_model
sandbox_hdb_resales_lakehouse
sandbox_hdb_resales_dataflow
sandbox_hdb_resales_pipeline
sandbox_hdb_resales_segmentation_notebook
sandbox_hdb_resales_price_trend_analysis
```

Avoid names such as:

```text
final_report
official_dashboard
prod_hdb_report
latest_version
test123
copy_of_copy_final
```

## Before starting any sandbox experiment

Before starting, confirm:

* [ ] I am working in the assigned Fabric Sandbox Workspace
* [ ] I am using only public, mocked, synthetic, or approved non-sensitive data
* [ ] I understand the purpose of the experiment
* [ ] I know which artefact I should use
* [ ] I will not overwrite shared starter artefacts
* [ ] I will name my work clearly
* [ ] I understand that sandbox outputs are not production assets
* [ ] I will document assumptions, caveats, and limitations
* [ ] I know when to ask for help

## When a sandbox idea becomes a real use case

A sandbox experiment may inspire a real department use case.

Before moving beyond sandbox, confirm:

* There is a real business question
* There is a department owner
* There is a deputy department workspace owner, if a department workspace is needed
* The intended users are known
* The data source is approved
* Sensitivity and access expectations are understood
* Refresh and ownership responsibilities are considered
* BIA is involved if productionisation may be required

Sandbox work should not be copied into department or production workspaces without review.

BIA Production Workspaces are restricted to BIA users. Non-BIA users should consume approved production outputs through approved report or app sharing channels, not direct BIA Production Workspace membership.

## Related sections

| Section                                                                      | Purpose                                                                           |
| ---------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| [Workspace Operating Model](../03-workspace-operating-model/)                | Understand personal, sandbox, department, and BIA production workspace boundaries |
| [Persona Pathways](../05-persona-pathways/)                                  | Choose a role-based learning pathway                                              |
| [Deployment Lifecycle Management](../06-deployment-lifecycle-management/)    | Understand how assets move beyond sandbox                                         |
| [Connections, Refresh and Monitoring](../07-connections-refresh-monitoring/) | Understand operational ownership and refresh responsibilities                     |
| [Data and Semantic Modelling](../08-data-and-semantic-modelling/)            | Understand grain, measures, semantic models, RLS, and AI-ready data               |
| [Templates and Checklists](../11-templates-checklists/)                      | Use reusable templates and checklists for review and documentation                |

## References and further learning

| Resource                                                                                                                                                                         | Purpose                                                                                                     |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| [Microsoft Fabric documentation](https://learn.microsoft.com/en-us/fabric/)                                                                                                      | Official Microsoft documentation for Fabric concepts, workloads, and platform capabilities                  |
| [Microsoft Learn: Get started with Microsoft Fabric](https://learn.microsoft.com/en-us/training/paths/get-started-fabric/)                                                       | Beginner learning pathway for users starting with Fabric                                                    |
| [Create a lakehouse, ingest sample data, and build a report](https://learn.microsoft.com/en-us/fabric/data-engineering/tutorial-build-lakehouse)                                 | Useful end-to-end tutorial for Lakehouse, ingestion, transformation, semantic model, and reporting concepts |
| [Prepare and visualize data with Microsoft Power BI](https://learn.microsoft.com/en-us/training/paths/prepare-visualize-data-power-bi/)                                          | Useful for report development, dashboard design, and visual analysis                                        |
| [Implement a data science and machine learning solution with Microsoft Fabric](https://learn.microsoft.com/en-us/training/paths/implement-data-science-machine-learning-fabric/) | Useful for advanced learners exploring data science and machine learning in Fabric                          |

## Next section

Proceed to:

[HDB Resales Sandbox Series](./hdb-resales/)
