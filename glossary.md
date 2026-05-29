# Glossary

This glossary explains key terms used in the Fabric Onboarding Guide.

The aim is to help learners understand common Microsoft Fabric, Power BI, analytics, governance, and onboarding terms in plain language.

## A

### Access Control

The practice of deciding who can access a workspace, report, semantic model, dataset, Lakehouse, pipeline, notebook, or other Fabric item.

Access control should follow the principle of least privilege.

### AI-Ready Data

Data that is structured, documented, governed, and meaningful enough to support AI-assisted analytics, copilots, agents, or semantic discovery.

AI-ready data is not just data stored in a modern platform. It should have clear definitions, ownership, security controls, and business meaning.

### Analytics Thinking

The ability to ask good questions, understand data meaning, assess assumptions, interpret evidence carefully, and communicate insights responsibly.

Analytics thinking is not only about using tools. It is about knowing what the data can and cannot support.

### Artefact

A file, report, notebook, template, dataset, model, or other output used in the onboarding guide or Fabric Sandbox Workspace.

Examples include a published report, a semantic model, a notebook, a use case canvas, a report review note, or a model card.

## B

### BIA

Business Intelligence and Analytics.

In this onboarding guide, BIA refers to the team responsible for supporting Fabric onboarding, managing the University’s Fabric analytics operating model, and reviewing relevant workspace, access, productionisation, and platform-level requests.

### BIA Production Workspace

A Fabric workspace reserved for BIA-managed production analytics assets.

Assets in BIA Production Workspaces should have stronger control, validation, monitoring, ownership, and release practices.

Direct workspace access to BIA Production Workspaces is restricted to BIA users. Non-BIA users should consume approved production outputs through approved report or app sharing channels.

### Bronze Layer

A commonly used term for raw or near-raw ingested data.

In the onboarding guide, Bronze means data preserved close to its original source form.

## C

### Capacity

The shared compute resource that powers Fabric workloads.

A simple analogy is electricity. Every action in Fabric consumes compute, just as every appliance consumes electricity.

### Capacity Unit

A unit of compute used by Microsoft Fabric capacity.

Users do not need to manage capacity units directly during onboarding, but they should understand that Fabric activity consumes shared resources.

### Checklist

A practical list of items to review before performing an action.

Examples include a sandbox readiness checklist, workspace access checklist, RLS testing checklist, and productionisation readiness checklist.

### Confidential - SUSS

A SUSS sensitivity label for higher-sensitivity institutional information that should be tightly controlled.

Users should follow SUSS guidance on how this label should be handled.

### Connection

A configuration that allows Fabric to connect to a data source.

Connections may involve files, databases, cloud sources, APIs, Lakehouses, Warehouses, or on-premises sources.

### Credential

The account, identity, or authentication method used to access a data source.

Credential ownership matters because refresh can fail if the credential expires, changes, or loses access.

### Curated Data

Data that has been cleaned, structured, and prepared for analysis or reporting.

Curated data is usually more suitable for reuse than raw data.

## D

### Dashboard

A Power BI visual summary that presents key metrics or visuals, often for monitoring.

In Power BI, dashboards and reports are different item types.

### Data Dictionary

A document that explains the meaning of fields, tables, measures, values, and business definitions.

A data dictionary helps users interpret data consistently.

### Dataflow Gen2

A Fabric data preparation capability that allows users to clean, transform, and load data using a low-code Power Query-style experience.

### Data Lakehouse

A Fabric item used for storing and analysing structured and semi-structured data.

A Lakehouse can support data engineering, analytics, notebooks, and reporting.

### Data Pipeline

A Fabric item used to move, orchestrate, and schedule data workflows.

Pipelines can be used to coordinate ingestion, transformation, refresh, and other activities.

### Data Source

The original system, file, database, API, or location from which data comes.

Data source ownership should be clear before data is used for reporting or analytics.

### Data Steward

A person or team that understands the meaning, quality, and appropriate use of a dataset.

A data steward may not own the system, but they help explain the data.

### Department Workspace

A Fabric workspace used for approved department-level exploration, prototyping, development, and capability building.

Department workspace outputs are not automatically production assets.

Department workspace requests should identify both a workspace owner and deputy workspace owner so that ownership does not depend on one person.

### Deployment Pipeline

A Fabric lifecycle management feature that can help move content between development, test, and production stages.

Not every onboarding or department use case requires a deployment pipeline.

### Deputy Workspace Owner

A backup accountable person for a department workspace.

The deputy workspace owner helps support continuity if the workspace owner leaves, changes role, or is unavailable.

### Direct Lake

A Fabric semantic model storage mode that allows Power BI to work with data in OneLake in certain Fabric scenarios.

Users do not need to master Direct Lake during basic onboarding, but they should be aware that semantic models can connect to data in different ways.

## E

### External Collaborator

A person outside the University who may need access to Fabric or Power BI content.

External collaborators may require Microsoft Entra B2B guest access, licensing review, and additional governance checks.

External collaborators should not be granted direct access to BIA Production Workspaces.

## F

### F64 Capacity

A Microsoft Fabric capacity SKU.

In the local onboarding context, BIA has provisioned F64 capacity to support the University’s analytics workloads.

### Fabric

Microsoft Fabric.

An end-to-end analytics platform that brings together data integration, data engineering, data warehousing, data science, real-time analytics, and business intelligence.

### Fabric Enthusiast

A user who wants to explore Microsoft Fabric before having a formal department use case.

Fabric enthusiasts should start in sandbox using safe data.

### Fabric Item

An object created or managed in Fabric.

Examples include reports, semantic models, Lakehouses, Warehouses, notebooks, pipelines, dataflows, and dashboards.

### Fabric Sandbox Workspace

A Fabric workspace assigned for onboarding, learning, and safe experimentation.

Hands-on onboarding activities should normally happen in the assigned Fabric Sandbox Workspace using public, mocked, synthetic, or approved non-sensitive data.

## G

### Gateway

A component that allows cloud services such as Fabric or Power BI to connect to data sources that are on-premises or behind private networks.

Gateway issues may require coordination with BIA, IT, system owners, or vendors.

### Git Integration

A Fabric lifecycle management feature that connects a workspace to a Git repository for version control and collaboration.

Git integration is a maturity option and should be introduced carefully.

### Gold Layer

A commonly used term for curated, reporting-ready or analysis-ready data.

In the onboarding guide, Gold means data that is prepared for reuse in reports, semantic models, or analytics.

### Grain

The level of detail represented by one row in a dataset.

Examples:

| Dataset                      | Grain                                |
| ---------------------------- | ------------------------------------ |
| HDB resale transaction table | One row per resale transaction       |
| Course feedback table        | One row per survey response          |
| Enrolment table              | One row per student-course enrolment |

Understanding grain is essential for correct analysis.

## H

### HDB Resales Sandbox Series

The main sandbox learning project used in this repo.

It uses public HDB resale flat data to support safe onboarding activities across report consumption, report development, data analysis, data engineering, semantic modelling, and advanced analytics.

## I

### Insight Summary

A short analytical write-up that explains an observation, why it matters, caveats, and follow-up questions.

### Item Permission

Permissions applied to a specific Fabric item, such as a report or semantic model.

Item permissions are different from workspace roles, although they may interact.

## K

### KPI

Key Performance Indicator.

A measure with business meaning, often used to monitor progress, performance, or outcomes.

A KPI should have a clear definition and interpretation.

## L

### Lakehouse

A Fabric data item that combines data lake storage with structured table capabilities for analytics.

### Least Privilege

The principle that users should receive only the minimum access needed for their role or task.

### Lifecycle Management

The practice of managing an asset from experimentation to development, review, deployment, monitoring, update, and retirement.

### Live Connection

A reporting pattern where a Power BI report connects to an existing semantic model or analytical source rather than importing its own data.

## M

### Measure

A calculated value used in reports and analysis.

Examples include transaction count, average resale price, median resale price, and completion rate.

### Microsoft Entra B2B Guest User

An external user invited into an organisation’s Microsoft Entra tenant for controlled collaboration.

External Fabric or Power BI collaboration may require Microsoft Entra B2B guest access.

### Microsoft Learn

Microsoft’s official learning platform for self-paced training modules and learning paths.

### Model Card

A document that explains a model’s purpose, input data, method, outputs, evaluation, limitations, and responsible use considerations.

## N

### Notebook

A Fabric item used for code-based data preparation, transformation, analytics, data science, or machine learning.

Notebooks may use Python, Spark, SQL, or other supported approaches depending on the Fabric experience.

## O

### OneLake

Microsoft Fabric’s unified data lake foundation.

OneLake is the storage layer behind many Fabric data experiences.

### Operational Ownership

Clear responsibility for maintaining an asset after it is created.

This includes ownership of connections, credentials, refresh, monitoring, support, and escalation.

## P

### PBIX

A Power BI Desktop file.

A PBIX file may contain report pages, model metadata, measures, data connection details, or imported data depending on how it was built.

For the HDB Resales Sandbox Series, learners should use the published report in the Fabric Sandbox Workspace. The PBIX file is not stored in this repo.

### Persona Pathway

A learning pathway designed for a specific type of user, such as report consumer, report developer, data analyst, data engineer, data scientist, department representative, workspace owner, or Fabric enthusiast.

### Personal Workspace

A Fabric workspace intended for individual exploration and private drafts.

A personal workspace should not be used for shared department assets, official reporting, or production work.

### Pipeline

See Data Pipeline.

### Power BI

Microsoft’s business intelligence and reporting platform.

Power BI is part of the broader Microsoft Fabric experience.

### Power BI Pro

A user license that supports creating, sharing, and collaborating on Power BI content, depending on the scenario.

In the local onboarding context, staff access is supported through Office 365 Education A5, which includes Power BI Pro capabilities.

### Productionisation

The process of preparing an asset for formal, wider-facing, monitored, or BIA-managed production use.

Productionisation may involve validation, access review, sensitivity labels, refresh planning, RLS testing, ownership assignment, and BIA review.

## R

### Refresh

The process of updating data in a report, semantic model, dataflow, pipeline, table, or related item.

Refresh may be manual, scheduled, pipeline-driven, or dependent on another upstream process.

### Report

A Power BI artefact containing pages of visuals, slicers, filters, and interactions.

Reports are used for analysis, monitoring, and communication.

### Report Consumer

A user who mainly views, filters, and interprets reports or dashboards.

### Report Developer

A user who builds or improves Power BI reports and may work with semantic models and measures.

### Restricted - SUSS

A SUSS sensitivity label for sensitive institutional information that should not be shared broadly.

Users should follow SUSS guidance on how this label should be handled.

### RLS

Row-Level Security.

A method for controlling which rows of data different users are allowed to see within the same report or semantic model.

### Roadmap

A plan showing how the repo or onboarding experience will evolve over time.

## S

### Sandbox Workspace

A Fabric workspace used for learning, experimentation, and practice.

Sandbox workspaces should use public, mocked, synthetic, or approved non-sensitive data.

### Semantic Model

A reusable business-friendly layer for reporting and analysis.

A semantic model may include tables, relationships, measures, hierarchies, definitions, formatting, and security rules.

### Sensitivity Label

A label applied to content to indicate how it should be handled.

In the local context, labels may include `Confidential - SUSS`, `Restricted - SUSS`, `Unrestricted - SUSS`, or `None`.

### Silver Layer

A commonly used term for cleaned and standardised data.

In the onboarding guide, Silver means data that has been prepared from raw form but may not yet be fully reporting-ready.

### Source Control

The practice of tracking changes to files or code over time, often using Git.

### SQL

Structured Query Language.

SQL is commonly used for querying structured data.

## T

### Template

A reusable document that helps users record information consistently.

Examples include report context notes, use case canvases, workspace health notes, and model cards.

### Tenant Setting

An administrator-controlled setting that affects what users can do in Fabric or Power BI.

In the local operating model, relevant tenant-level settings should be escalated to BIA for review.

## U

### Unrestricted - SUSS

A SUSS sensitivity label for information that is not classified as confidential or restricted, but still belongs to the organisation and should be handled responsibly.

### Use Case Canvas

A template for framing an analytics use case.

It captures the business question, intended users, data needed, ownership, access, sensitivity, expected output, and next steps.

## W

### Warehouse

A Fabric item that supports SQL-based analytics and data warehousing.

### Workspace

A collaboration area in Fabric where users create, manage, and access items such as reports, semantic models, Lakehouses, notebooks, pipelines, and dashboards.

### Workspace Owner

A person or group responsible for helping manage a workspace, coordinate access, keep content organised, and support responsible use.

For department workspaces, there should also be a deputy workspace owner.

### Workspace Role

A role that determines what a user can do in a workspace.

Common roles include Viewer, Contributor, Member, and Admin.
