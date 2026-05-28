# Sandbox Experiments

Sandbox experiments provide guided practice activities for Microsoft Fabric onboarding.

All onboarding learners start in sandbox. The sandbox is the safe space for learning, experimenting, making mistakes, asking questions, and building confidence before moving into department-level or production-facing work.

The initial sandbox series is built around **HDB Resales**, a public-data learning project based on HDB resale flat transactions.

## Why HDB Resales

HDB resale data is useful for onboarding because it is:

- Public and non-sensitive
- Relatable to users in Singapore
- Rich enough for dashboarding, analytics, semantic modelling, and data engineering
- Safe for experimentation at scale
- Suitable for beginner, practitioner, and advanced learning
- Easy to connect to real-world analytical questions without using institutional data

Using one common project across multiple pathways helps learners build progressively.

A report consumer may start by interpreting an HDB resale dashboard. A report developer may improve the dashboard design. A data analyst may examine price trends. A data engineer may ingest and clean the data in a Lakehouse. A data scientist may attempt segmentation or modelling. A workspace owner may review access, naming, ownership, and refresh responsibilities.

![Placeholder: HDB Resales sandbox experiment map](../assets/images/hdb-resales-sandbox-experiment-map.png)

> Image placeholder: A map showing the HDB Resales sandbox series branching into report consumer, report developer, data analyst, data engineer, data scientist, department representative, workspace owner, and Fabric enthusiast activities.

## Sandbox-first principle

Sandbox experiments should use only safe data.

Approved sandbox data includes:

- Public data
- Mocked data
- Synthetic data
- Approved non-sensitive data

Sandbox experiments should not use:

- Real confidential institutional data
- Real restricted institutional data
- Student personal data
- Staff personal data
- Financial records
- Donor records
- Operational data from production systems
- Any data that has not been approved for sandbox use

## Sandbox outputs are not production assets

Sandbox outputs are for learning and experimentation only.

They should not be treated as:

- Official reports
- Validated analytics products
- Production semantic models
- Operational dashboards
- Authoritative data products
- Formal decision-support tools

A sandbox output may inspire a real use case, but it should go through review before moving into department workspace or BIA production consideration.

## HDB Resales sandbox structure

The HDB Resales sandbox series is organised as follows:

```text
09-sandbox-experiments/
└── hdb-resales/
    ├── README.md
    ├── assets/
    │   └── HDB_Resales.pbix
    ├── data/
    │   ├── hdb_resales_sample.csv
    │   └── hdb_resales_data_dictionary.md
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
    └── model-output/
```

Some files may be added progressively as the sandbox series develops.

## Sandbox experiment catalogue

| No. | Experiment | Main Persona | Purpose |
|---|---|---|---|
| 01 | [HDB Resales: Report Consumer Walkthrough](./hdb-resales/01-report-consumer-walkthrough/) | Report Consumer | Practise opening, filtering, and interpreting the HDB Resales report |
| 02 | [HDB Resales: Dashboard Design and Storytelling](./hdb-resales/02-dashboard-design-and-storytelling/) | Report Developer | Improve dashboard clarity, layout, and visual storytelling |
| 03 | [HDB Resales: Semantic Model and KPI Definitions](./hdb-resales/03-semantic-model-and-kpi-definitions/) | Report Developer / Data Analyst | Practise measure definitions, semantic modelling, and reuse |
| 04 | [HDB Resales: Lakehouse Ingestion and Cleaning](./hdb-resales/04-lakehouse-ingestion-and-cleaning/) | Data Engineer | Load, clean, and prepare HDB resale data in a Lakehouse |
| 05 | [HDB Resales: Market Segmentation](./hdb-resales/05-market-segmentation/) | Data Scientist | Explore clustering or segmentation of resale market patterns |
| 06 | [HDB Resales: Price Trend and Affordability Analysis](./hdb-resales/06-price-trend-and-affordability-analysis/) | Data Analyst / Data Scientist | Analyse resale price trends and interpret them cautiously |
| 07 | [HDB Resales: Town and Flat Type Comparison](./hdb-resales/07-town-and-flat-type-comparison/) | Data Analyst | Compare resale patterns across towns and flat types |
| 08 | [HDB Resales: Geospatial and Location Analysis](./hdb-resales/08-geospatial-location-analysis/) | Advanced Analyst | Explore location-related patterns where suitable data is available |
| 09 | [HDB Resales: AI-Ready Data and Semantic Layer](./hdb-resales/09-ai-ready-data-and-semantic-layer/) | Advanced User / Fabric Enthusiast | Explore how clean data, definitions, and semantic meaning support AI-ready analytics |

## How the experiments connect to persona pathways

The persona pathways explain what users should learn.

The sandbox experiments provide the hands-on practice.

| Persona Pathway | Recommended Starting Experiment |
|---|---|
| [Report Consumer](../05-persona-pathways/report-consumer/) | [01 Report Consumer Walkthrough](./hdb-resales/01-report-consumer-walkthrough/) |
| [Report Developer](../05-persona-pathways/report-developer/) | [02 Dashboard Design and Storytelling](./hdb-resales/02-dashboard-design-and-storytelling/) |
| [Data Analyst](../05-persona-pathways/data-analyst/) | [06 Price Trend and Affordability Analysis](./hdb-resales/06-price-trend-and-affordability-analysis/) |
| [Data Engineer](../05-persona-pathways/data-engineer/) | [04 Lakehouse Ingestion and Cleaning](./hdb-resales/04-lakehouse-ingestion-and-cleaning/) |
| [Data Scientist](../05-persona-pathways/data-scientist/) | [05 Market Segmentation](./hdb-resales/05-market-segmentation/) |
| [Department Representative](../05-persona-pathways/department-representative/) | [01 Report Consumer Walkthrough](./hdb-resales/01-report-consumer-walkthrough/) and use case canvas |
| [Workspace Owner](../05-persona-pathways/workspace-owner/) | Workspace inventory and health checklist activities |
| [Fabric Enthusiast](../05-persona-pathways/fabric-enthusiast/) | Any beginner experiment based on interest |

## Learning levels

The sandbox experiments can be grouped by learning level.

| Level | Suitable Experiments | Focus |
|---|---|---|
| Beginner | 01, 02 | Report consumption, navigation, dashboard interpretation, visual design |
| Practitioner | 03, 04, 06, 07 | Semantic modelling, data preparation, analytical comparison, trend interpretation |
| Advanced | 05, 08, 09 | Segmentation, location analysis, AI-ready semantic layer, advanced analytics thinking |

Users should not rush into advanced experiments before understanding the basics of safe data use, workspace context, and interpretation.

## Working with the HDB Resales PBIX

The starting Power BI file is stored at:

```text
09-sandbox-experiments/hdb-resales/assets/HDB_Resales.pbix
```

This file is mainly used for:

- Report consumer walkthrough
- Report developer practice
- Dashboard design and storytelling
- Semantic model review
- Demonstrating how curated data becomes a report

The PBIX should be treated as a sandbox learning artefact. Learners should work on copies where instructed and should not overwrite the shared starter file.

## Working with source data

Source data should be stored under:

```text
09-sandbox-experiments/hdb-resales/data/
```

Suggested files:

```text
hdb_resales_sample.csv
hdb_resales_data_dictionary.md
hdb_resales_modelling_sample.csv
```

The source data supports:

- Data analyst activities
- Data engineer activities
- Data scientist activities
- Semantic modelling activities
- AI-ready data activities

## Working with notebooks

Notebooks should be stored under:

```text
09-sandbox-experiments/hdb-resales/notebooks/
```

Suggested notebooks:

```text
hdb_resales_data_preparation.ipynb
hdb_resales_market_segmentation.ipynb
hdb_resales_price_band_prediction.ipynb
```

Notebooks should be used only in sandbox unless reviewed and approved for a department or production use case.

## Working with templates

Templates should be stored under:

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

Templates help learners document their thinking, assumptions, limitations, and next steps.

## Naming convention for sandbox work

Use clear names that show the work is exploratory.

Recommended examples:

```text
sandbox_hdb_resales_report
sandbox_hdb_resales_semantic_model
sandbox_hdb_resales_lakehouse
sandbox_hdb_resales_dataflow
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

## Sandbox experiment checklist

Before starting a sandbox experiment, confirm:

- [ ] I am working in the assigned sandbox workspace
- [ ] I am using public, mocked, synthetic, or approved non-sensitive data
- [ ] I understand the purpose of the experiment
- [ ] I know which artefact I should use
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

## Next section

Proceed to:

[Curated Learning Resources](../10-curated-learning-resources/)
