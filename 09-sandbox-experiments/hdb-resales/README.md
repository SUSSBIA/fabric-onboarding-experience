# HDB Resales Sandbox Series

The HDB Resales Sandbox Series is the main hands-on learning project for the Fabric Onboarding Experience.

It uses public HDB resale flat data as a safe, relatable, and practical dataset for learning Microsoft Fabric. The same sandbox project supports different learning pathways, from basic report consumption to dashboard design, data analysis, data engineering, semantic modelling, and advanced analytics.

## Why this sandbox series exists

Fabric onboarding should not rely only on product screenshots or abstract examples.

Learners need a safe project where they can practise:

- Opening and interpreting reports
- Building and improving dashboards
- Understanding semantic models and measures
- Exploring data quality and analytical questions
- Loading and preparing data in a Lakehouse
- Running simple notebooks or modelling experiments
- Documenting assumptions, caveats, and limitations
- Thinking about whether an output should remain sandbox or move towards a real use case

The HDB Resales dataset is useful because it is public, non-sensitive, and familiar to many users in Singapore.

## Sandbox-first principle

All activities in this series should be completed in the assigned Fabric Sandbox Workspace.

This series should use only:

- Public data
- Mocked data
- Synthetic data
- Approved non-sensitive data

Do not use:

- Real confidential institutional data
- Real restricted institutional data
- Student personal data
- Staff personal data
- Financial records
- Donor records
- Operational production data
- Any data that has not been approved for sandbox use

Sandbox outputs are for learning and experimentation only. They are not official reports, production semantic models, operational dashboards, or formal decision-support tools.

## Repo versus Fabric Sandbox Workspace

The HDB Resales Sandbox Series uses both this GitHub repo and a Fabric Sandbox Workspace.

The repo explains what to do. The Fabric Sandbox Workspace is where the hands-on work happens.

| Area | Purpose |
|---|---|
| GitHub repo | Stores onboarding instructions, README files, templates, checklists, source references, and learning guidance |
| Fabric Sandbox Workspace | Hosts the working artefacts that learners open, run, edit, copy, and practise with |

Learners should perform hands-on work in the Fabric Sandbox Workspace, not directly inside the GitHub repo.

## Where artefacts are stored

| Artefact | Primary Location | Purpose |
|---|---|---|
| Learning instructions | GitHub repo | Guides learners through each exercise |
| Templates and checklists | GitHub repo | Provides reusable documentation aids |
| Source PBIX reference | GitHub repo, optional | Provides a version-controlled starter reference |
| Published HDB Resales report | Fabric Sandbox Workspace | Used by report consumers and report developers |
| HDB Resales semantic model | Fabric Sandbox Workspace | Used for report development and semantic model review |
| HDB Resales Lakehouse | Fabric Sandbox Workspace | Used for ingestion, cleaning, and data engineering activities |
| HDB Resales source data | Fabric Sandbox Workspace, with optional public copy in repo | Used for data loading, analysis, and modelling |
| Notebooks | Fabric Sandbox Workspace, with optional source copy in repo | Used for data preparation, segmentation, and modelling |
| Dataflows and pipelines | Fabric Sandbox Workspace | Used for orchestration and transformation practice |
| Completed learner outputs | Fabric Sandbox Workspace | Stores sandbox outputs created during exercises |

## Learning map

![HDB Resales sandbox experiment map](../../assets/images/hdb-resales-sandbox-experiment-map.png)

> Image: Map of the HDB Resales Sandbox Series showing how one public dataset supports report consumption, report development, data analysis, data engineering, data science, workspace ownership, department use case framing, and AI-ready data learning.

## Repo structure

The repo structure for this sandbox series is:

```text
09-sandbox-experiments/
└── hdb-resales/
    ├── README.md
    ├── assets/
    │   └── HDB_Resales.pbix
    ├── data/
    │   ├── hdb_resales_sample.csv
    │   ├── hdb_resales_data_dictionary.md
    │   └── hdb_resales_modelling_sample.csv
    ├── notebooks/
    │   ├── hdb_resales_data_preparation.ipynb
    │   ├── hdb_resales_market_segmentation.ipynb
    │   └── hdb_resales_price_band_prediction.ipynb
    ├── templates/
    │   ├── report-context-note.md
    │   ├── insight-summary-template.md
    │   ├── use-case-canvas.md
    │   ├── workspace-inventory-template.md
    │   ├── workspace-health-note.md
    │   └── model-card-template.md
    ├── model-output/
    ├── 01-report-consumer-walkthrough/
    │   └── README.md
    ├── 02-dashboard-design-and-storytelling/
    │   └── README.md
    ├── 03-semantic-model-and-kpi-definitions/
    │   └── README.md
    ├── 04-lakehouse-ingestion-and-cleaning/
    │   └── README.md
    ├── 05-market-segmentation/
    │   └── README.md
    ├── 06-price-trend-and-affordability-analysis/
    │   └── README.md
    ├── 07-town-and-flat-type-comparison/
    │   └── README.md
    ├── 08-geospatial-location-analysis/
    │   └── README.md
    └── 09-ai-ready-data-and-semantic-layer/
        └── README.md
```

Some artefacts may be added progressively as the sandbox series develops.

## Fabric Sandbox Workspace structure

The Fabric Sandbox Workspace should contain the working artefacts used by learners.

Suggested workspace items:

| Fabric Item | Suggested Name | Purpose |
|---|---|---|
| Report | `sandbox_hdb_resales_report` | Published report used for report consumer and report developer activities |
| Semantic model | `sandbox_hdb_resales_semantic_model` | Model used for reporting, measure review, and semantic model exercises |
| Lakehouse | `sandbox_hdb_resales_lakehouse` | Stores HDB resale source data, cleaned tables, and curated tables |
| Notebook | `sandbox_hdb_resales_data_preparation_notebook` | Prepares and cleans HDB resale data |
| Notebook | `sandbox_hdb_resales_market_segmentation_notebook` | Supports clustering or segmentation exercises |
| Notebook | `sandbox_hdb_resales_price_band_prediction_notebook` | Supports simple modelling or prediction exercises |
| Dataflow Gen2 | `sandbox_hdb_resales_dataflow` | Optional low-code transformation exercise |
| Pipeline | `sandbox_hdb_resales_pipeline` | Optional orchestration exercise |
| Output table | `sandbox_hdb_resales_model_output` | Stores sandbox model or segmentation outputs |

The exact workspace item names may vary, but they should clearly indicate that the artefacts are sandbox learning assets.

## Supporting artefacts in the repo

Different users will use different repo artefacts depending on their pathway.

| Artefact Area | Purpose |
|---|---|
| `assets/` | Stores the starting PBIX reference file and other reusable static artefacts |
| `data/` | Stores public HDB resale sample data and data dictionary files, if included |
| `notebooks/` | Stores source copies of Fabric notebook exercises, if included |
| `templates/` | Stores exercise-specific copies of templates used during sandbox activities |
| `model-output/` | Stores sample sandbox model outputs, if included |
| Experiment folders | Store step-by-step README files for each guided activity |

The repo version should be treated as the documentation and source reference. The Fabric Sandbox Workspace version should be treated as the hands-on working environment.

## Starting PBIX artefact

The starting Power BI file may be stored in the repo as a reference copy:

```text
09-sandbox-experiments/hdb-resales/assets/HDB_Resales.pbix
```

This file is mainly used for:

- Publishing the HDB Resales report into the Fabric Sandbox Workspace
- Report consumer walkthrough
- Dashboard design and storytelling
- Report developer practice
- Semantic model review
- Measure and KPI definition review
- Demonstrating how curated data becomes a report

Learners should usually interact with the published report in the Fabric Sandbox Workspace.

Report developers may work on a copy of the PBIX or report where instructed. They should not overwrite the shared starter artefact.

## Source data

Source data should be loaded into the Fabric Sandbox Workspace, usually through a Lakehouse.

Suggested repo reference location:

```text
09-sandbox-experiments/hdb-resales/data/
```

Suggested files:

```text
hdb_resales_sample.csv
hdb_resales_data_dictionary.md
hdb_resales_modelling_sample.csv
```

Suggested Fabric Sandbox Workspace location:

```text
sandbox_hdb_resales_lakehouse
```

Possible Lakehouse structure:

```text
Files/
└── hdb-resales/
    └── raw/

Tables/
├── hdb_resales_raw
├── hdb_resales_cleaned
├── hdb_resales_curated
└── hdb_resales_modelling
```

The source data supports:

- Data analyst activities
- Data engineer activities
- Data scientist activities
- Semantic modelling activities
- AI-ready data activities

The source data should be treated as public sandbox data. If any derived dataset is created, it should be clearly marked as sandbox or experimental.

## Notebooks

Notebooks should primarily live in the Fabric Sandbox Workspace so learners can run them.

Suggested repo reference location:

```text
09-sandbox-experiments/hdb-resales/notebooks/
```

Suggested notebooks:

```text
hdb_resales_data_preparation.ipynb
hdb_resales_market_segmentation.ipynb
hdb_resales_price_band_prediction.ipynb
```

Suggested Fabric Sandbox Workspace items:

```text
sandbox_hdb_resales_data_preparation_notebook
sandbox_hdb_resales_market_segmentation_notebook
sandbox_hdb_resales_price_band_prediction_notebook
```

Notebooks should be used only in sandbox unless reviewed and approved for a department or production use case.

## Templates

Exercise-specific templates may be stored under:

```text
09-sandbox-experiments/hdb-resales/templates/
```

Suggested templates:

```text
report-context-note.md
insight-summary-template.md
use-case-canvas.md
workspace-inventory-template.md
workspace-health-note.md
model-card-template.md
```

The general reusable versions are stored in:

```text
11-templates-checklists/
```

The HDB Resales versions may be copied or adapted for specific sandbox exercises.

## Experiment catalogue

| No. | Experiment | Main Persona | Purpose | Status |
|---|---|---|---|---|
| 01 | [Report Consumer Walkthrough](./01-report-consumer-walkthrough/) | Report Consumer | Practise opening, filtering, and interpreting the HDB Resales report | Drafted |
| 02 | [Dashboard Design and Storytelling](./02-dashboard-design-and-storytelling/) | Report Developer | Improve dashboard clarity, layout, and visual storytelling | Planned |
| 03 | [Semantic Model and KPI Definitions](./03-semantic-model-and-kpi-definitions/) | Report Developer / Data Analyst | Practise measure definitions, semantic modelling, and reuse | Planned |
| 04 | [Lakehouse Ingestion and Cleaning](./04-lakehouse-ingestion-and-cleaning/) | Data Engineer | Load, clean, and prepare HDB resale data in a Lakehouse | Planned |
| 05 | [Market Segmentation](./05-market-segmentation/) | Data Scientist | Explore clustering or segmentation of resale market patterns | Planned |
| 06 | [Price Trend and Affordability Analysis](./06-price-trend-and-affordability-analysis/) | Data Analyst / Data Scientist | Analyse resale price trends and interpret them cautiously | Planned |
| 07 | [Town and Flat Type Comparison](./07-town-and-flat-type-comparison/) | Data Analyst | Compare resale patterns across towns and flat types | Planned |
| 08 | [Geospatial and Location Analysis](./08-geospatial-location-analysis/) | Advanced Analyst | Explore location-related patterns where suitable data is available | Planned |
| 09 | [AI-Ready Data and Semantic Layer](./09-ai-ready-data-and-semantic-layer/) | Advanced User / Fabric Enthusiast | Explore how clean data, definitions, and semantic meaning support AI-ready analytics | Planned |

## Relationship with persona pathways

The persona pathways explain what users should learn.

The HDB Resales experiments provide the hands-on practice.

| Persona Pathway | Recommended Starting Point |
|---|---|
| [Report Consumer](../../05-persona-pathways/report-consumer/) | [01 Report Consumer Walkthrough](./01-report-consumer-walkthrough/) |
| [Report Developer](../../05-persona-pathways/report-developer/) | [02 Dashboard Design and Storytelling](./02-dashboard-design-and-storytelling/) |
| [Data Analyst](../../05-persona-pathways/data-analyst/) | [06 Price Trend and Affordability Analysis](./06-price-trend-and-affordability-analysis/) |
| [Data Engineer](../../05-persona-pathways/data-engineer/) | [04 Lakehouse Ingestion and Cleaning](./04-lakehouse-ingestion-and-cleaning/) |
| [Data Scientist](../../05-persona-pathways/data-scientist/) | [05 Market Segmentation](./05-market-segmentation/) |
| [Department Representative](../../05-persona-pathways/department-representative/) | [01 Report Consumer Walkthrough](./01-report-consumer-walkthrough/) and use case canvas |
| [Workspace Owner](../../05-persona-pathways/workspace-owner/) | Workspace inventory and workspace health activities |
| [Fabric Enthusiast](../../05-persona-pathways/fabric-enthusiast/) | Any beginner experiment based on interest |

## Learning levels

| Level | Suitable Experiments | Focus |
|---|---|---|
| Beginner | 01, 02 | Report consumption, navigation, dashboard interpretation, dashboard design |
| Practitioner | 03, 04, 06, 07 | Semantic modelling, data preparation, analytical comparison, trend interpretation |
| Advanced | 05, 08, 09 | Segmentation, location analysis, AI-ready semantic layer, advanced analytics thinking |

Users should not rush into advanced experiments before understanding safe data use, workspace context, and responsible interpretation.

## Suggested naming convention

Use names that clearly show the work is sandbox or experimental.

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

## Before starting an experiment

Before starting any HDB Resales sandbox experiment, confirm:

- [ ] I am working in the assigned Fabric Sandbox Workspace
- [ ] I am using only public, mocked, synthetic, or approved non-sensitive data
- [ ] I understand the purpose of the experiment
- [ ] I know which Fabric artefact I should use
- [ ] I will not overwrite shared starter artefacts
- [ ] I will name my work clearly
- [ ] I understand that sandbox outputs are not production assets
- [ ] I will document assumptions, caveats, and limitations
- [ ] I know when to ask for help

## When a sandbox idea becomes a real use case

A sandbox experiment may inspire a real department use case.

Before moving beyond sandbox, confirm:

- There is a real business question
- There is a department owner
- The intended users are known
- The data source is approved
- Sensitivity and access expectations are understood
- Refresh and ownership responsibilities are considered
- BIA is involved if productionisation may be required

Sandbox work should not be copied into department or production workspaces without review.

## References and further learning

| Resource | Purpose |
|---|---|
| [Microsoft Fabric documentation](https://learn.microsoft.com/en-us/fabric/) | Official Microsoft documentation for Fabric concepts, workloads, and platform capabilities |
| [Microsoft Learn: Get started with Microsoft Fabric](https://learn.microsoft.com/en-us/training/paths/get-started-fabric/) | Beginner learning pathway for users starting with Fabric |
| [Create a lakehouse, ingest sample data, and build a report](https://learn.microsoft.com/en-us/fabric/data-engineering/tutorial-build-lakehouse) | Useful end-to-end tutorial for Lakehouse, ingestion, transformation, semantic model, and reporting concepts |
| [Prepare and visualize data with Microsoft Power BI](https://learn.microsoft.com/en-us/training/paths/prepare-visualize-data-power-bi/) | Useful for report development, dashboard design, and visual analysis |
| [Implement a data science and machine learning solution with Microsoft Fabric](https://learn.microsoft.com/en-us/training/paths/implement-data-science-machine-learning-fabric/) | Useful for advanced learners exploring data science and machine learning in Fabric |

## Next experiment

Proceed to:

[HDB Resales: Report Consumer Walkthrough](./01-report-consumer-walkthrough/)
