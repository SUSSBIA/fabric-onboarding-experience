# Roadmap

This roadmap explains how the Fabric Onboarding Guide is expected to evolve.

The repo is designed as a living onboarding resource. It starts with foundational guidance, then grows into persona pathways, sandbox experiments, reusable templates, checklists, curated learning resources, and more advanced operating practices as Fabric adoption matures.

## Roadmap principles

The roadmap follows these principles:

* Start with safety, access, and governance before hands-on use
* Use sandbox-first onboarding for learners
* Use public, mocked, synthetic, or approved non-sensitive data for learning
* Build pathways for different learner personas
* Use HDB Resales as the initial common sandbox learning project
* Keep personal, sandbox, department, and BIA production workspace boundaries clear
* Keep BIA Production Workspaces restricted to BIA users
* Avoid creating unmanaged self-service sprawl
* Grow towards reusable semantic models, trusted data assets, and AI-ready analytics over time

## Current operating assumptions

The current Fabric operating model is based on:

| Area                           | Current Assumption                                                                                                             |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ |
| Staff licensing                | Staff access is supported through Office 365 Education A5, which includes Power BI Pro capabilities                            |
| Capacity                       | BIA has provisioned F64 capacity for University analytics workloads                                                            |
| Personal workspace             | Personal workspaces are for individual exploration and private drafts, not shared department or production work                |
| Sandbox onboarding             | Learners begin hands-on practice in the assigned Fabric Sandbox Workspace                                                      |
| Department workspaces          | Department workspaces support approved exploration, prototyping, and department-level working assets                           |
| Department ownership           | Department workspace requests should identify both a workspace owner and deputy workspace owner                                |
| BIA Production Workspaces      | BIA Production Workspaces are reserved for BIA-managed production assets, with direct workspace access restricted to BIA users |
| Non-BIA production consumption | Non-BIA users should consume approved production outputs through approved report or app sharing channels                       |
| Shared central workspace       | No formal shared or central workspace model currently exists                                                                   |
| Tenant-level settings          | Relevant Fabric tenant-level settings are controlled by BIA and should be escalated to BIA for review                          |
| External collaborators         | External collaborators may require Microsoft Entra B2B guest access and licensing review                                       |

## Phase 1: Foundation onboarding

Status: Drafted

This phase establishes the common foundation that learners should understand before using Fabric hands-on.

| Section                          | Purpose                                                                       | Status  |
| -------------------------------- | ----------------------------------------------------------------------------- | ------- |
| `README.md`                      | Front door and navigation map for the repo                                    | Drafted |
| `00-start-here/`                 | Explain the onboarding journey and sandbox-first approach                     | Drafted |
| `01-security-access-governance/` | Explain security, access, sensitivity labels, RLS awareness, and escalation   | Drafted |
| `02-licensing-capacity/`         | Explain A5 licensing, Power BI Pro, F64 capacity, and responsible compute use | Drafted |
| `03-workspace-operating-model/`  | Explain personal, sandbox, department, and BIA production workspace patterns  | Drafted |
| `04-start-using-fabric/`         | Guide learners into their first safe Fabric activities in sandbox             | Drafted |
| `glossary.md`                    | Explain common terms used in the onboarding guide                             | Drafted |

## Phase 2: Persona pathways

Status: In progress

This phase provides role-based learning pathways so learners do not need to learn every Fabric capability at once.

| Pathway                         | Purpose                                                                                      | Status  |
| ------------------------------- | -------------------------------------------------------------------------------------------- | ------- |
| `05-persona-pathways/README.md` | Gateway page for choosing a pathway                                                          | Drafted |
| `report-consumer/`              | Learn to open, filter, and interpret reports responsibly                                     | Drafted |
| `report-developer/`             | Learn report design, semantic model awareness, measures, validation, and caveats             | Drafted |
| `data-analyst/`                 | Learn data exploration, analytical questions, comparisons, trends, and insight summaries     | Drafted |
| `data-engineer/`                | Learn Lakehouse ingestion, cleaning, layering, transformation, and refresh thinking          | Drafted |
| `data-scientist/`               | Learn modelling, clustering, evaluation, responsible interpretation, and model documentation | Drafted |
| `department-representative/`    | Learn use case framing, ownership, access, sensitivity, and BIA engagement                   | Drafted |
| `workspace-owner/`              | Learn workspace health, access, naming, ownership, and escalation practices                  | Drafted |
| `fabric-enthusiast/`            | Learn safe exploration across Fabric capabilities                                            | Drafted |

## Phase 3: Responsible-use modules

Status: Drafted

These sections support more sustainable Fabric use beyond basic onboarding.

| Section                               | Purpose                                                                                  | Status  |
| ------------------------------------- | ---------------------------------------------------------------------------------------- | ------- |
| `06-deployment-lifecycle-management/` | Explain movement from sandbox to department workspace to BIA production where applicable | Drafted |
| `07-connections-refresh-monitoring/`  | Explain connections, credentials, gateways, refresh, monitoring, and failure handling    | Drafted |
| `08-data-and-semantic-modelling/`     | Explain grain, measures, semantic models, RLS, reuse, and AI-ready data                  | Drafted |

## Phase 4: HDB Resales Sandbox Series

Status: In progress

This phase builds the hands-on practice layer of the onboarding experience.

The initial sandbox project is based on public HDB resale flat data. It is safe, relatable, and rich enough to support multiple learning pathways.

| Experiment                                   | Purpose                                                                      | Status  |
| -------------------------------------------- | ---------------------------------------------------------------------------- | ------- |
| `09-sandbox-experiments/README.md`           | Catalogue of all sandbox experiments                                         | Drafted |
| `hdb-resales/README.md`                      | Overview of the HDB Resales Sandbox Series                                   | Drafted |
| `01-report-consumer-walkthrough/`            | Practise report navigation, filters, slicers, and responsible interpretation | Drafted |
| `02-dashboard-design-and-storytelling/`      | Practise dashboard design and report storytelling                            | Drafted |
| `03-semantic-model-and-kpi-definitions/`     | Practise measures, definitions, semantic modelling, and reuse                | Planned |
| `04-lakehouse-ingestion-and-cleaning/`       | Practise loading and cleaning HDB resale data in a Lakehouse                 | Planned |
| `05-market-segmentation/`                    | Practise clustering or segmentation of resale market patterns                | Planned |
| `06-price-trend-and-affordability-analysis/` | Practise trend analysis and cautious interpretation                          | Planned |
| `07-town-and-flat-type-comparison/`          | Practise group comparison across towns and flat types                        | Planned |
| `08-geospatial-location-analysis/`           | Explore location-related analysis where suitable data is available           | Planned |
| `09-ai-ready-data-and-semantic-layer/`       | Explore semantic meaning, documentation, and AI-ready data concepts          | Planned |

## Phase 5: Supporting artefacts

Status: In progress

This phase creates supporting materials used by the HDB Resales sandbox series and the persona pathways.

| Artefact Area              | Examples                                                          | Status                               |
| -------------------------- | ----------------------------------------------------------------- | ------------------------------------ |
| Published report           | HDB Resales report in the assigned Fabric Sandbox Workspace       | Prepared in Fabric Sandbox Workspace |
| PBIX                       | Source PBIX is not stored in this public repo                     | Not included                         |
| Data                       | Public HDB resale sample data and data dictionary                 | Planned                              |
| Notebooks                  | Data preparation, market segmentation, price band prediction      | Planned                              |
| Templates                  | Report context note, insight summary, use case canvas, model card | Drafted                              |
| Model outputs              | Sandbox model output tables or files                              | Planned                              |
| Workspace review artefacts | Workspace inventory, workspace health note                        | Drafted                              |

The repo should store learning instructions, templates, checklists, public sample data, and source references.

Hands-on artefacts should be accessed through the assigned Fabric Sandbox Workspace.

## Phase 6: Templates and checklists

Status: In progress

The templates and checklists section provides reusable resources for onboarding, sandbox learning, workspace management, deployment review, and productionisation readiness.

| Resource                                              | Status  |
| ----------------------------------------------------- | ------- |
| `11-templates-checklists/README.md`                   | Drafted |
| `templates/report-context-note.md`                    | Drafted |
| `templates/insight-summary-template.md`               | Drafted |
| `templates/use-case-canvas.md`                        | Drafted |
| `templates/workspace-inventory-template.md`           | Drafted |
| `templates/workspace-health-note.md`                  | Drafted |
| `templates/model-card-template.md`                    | Drafted |
| `templates/release-note-template.md`                  | Drafted |
| `templates/refresh-failure-note.md`                   | Drafted |
| `checklists/sandbox-readiness-checklist.md`           | Drafted |
| `checklists/workspace-access-checklist.md`            | Drafted |
| `checklists/report-review-checklist.md`               | Drafted |
| `checklists/semantic-model-review-checklist.md`       | Drafted |
| `checklists/rls-testing-checklist.md`                 | Drafted |
| `checklists/refresh-monitoring-checklist.md`          | Drafted |
| `checklists/productionisation-readiness-checklist.md` | Drafted |
| `checklists/external-collaborator-checklist.md`       | Drafted |

## Phase 7: Curated learning resources

Status: Drafted

This section gathers official Microsoft documentation, Microsoft Learn resources, and curated video learning references.

| Area                                           | Status               |
| ---------------------------------------------- | -------------------- |
| Microsoft Fabric overview                      | Drafted              |
| Security, access, and governance               | Drafted              |
| Licensing and capacity                         | Drafted              |
| Workspaces and operating model                 | Drafted              |
| Power BI report consumers                      | Drafted              |
| Report development and dashboard design        | Drafted              |
| Data analytics and modelling                   | Drafted              |
| Data engineering                               | Drafted              |
| Data Factory, pipelines, and Dataflow Gen2     | Drafted              |
| Connections, gateways, refresh, and monitoring | Drafted              |
| Data science and machine learning              | Drafted              |
| Deployment lifecycle management                | Drafted              |
| Adoption and governance                        | Drafted              |
| Curated video inventory                        | Placeholder retained |

## Phase 8: Image and visual polish

Status: In progress

Images are stored in:

```text
assets/images/
```

Generated or planned images include:

| Image                                             | Used In                                                        | Status    |
| ------------------------------------------------- | -------------------------------------------------------------- | --------- |
| `layered-fabric-onboarding-journey.png`           | `00-start-here/`                                               | Generated |
| `fabric-access-and-governance-layers.png`         | `01-security-access-governance/`                               | Generated |
| `fabric-licensing-capacity-model.png`             | `02-licensing-capacity/`                                       | Generated |
| `fabric-workspace-operating-model.png`            | `03-workspace-operating-model/`                                | Generated |
| `first-safe-steps-in-fabric-sandbox.png`          | `04-start-using-fabric/`                                       | Generated |
| `persona-pathways-fabric-onboarding.png`          | `05-persona-pathways/`                                         | Generated |
| `report-consumer-sandbox-learning-path.png`       | `report-consumer/` and HDB Resales report consumer walkthrough | Generated |
| `report-developer-sandbox-learning-path.png`      | `report-developer/`                                            | Generated |
| `data-analyst-hdb-resales-learning-path.png`      | `data-analyst/`                                                | Generated |
| `data-engineer-hdb-resales-learning-path.png`     | `data-engineer/`                                               | Generated |
| `data-scientist-hdb-resales-learning-path.png`    | `data-scientist/`                                              | Generated |
| `department-representative-learning-path.png`     | `department-representative/`                                   | Generated |
| `workspace-owner-learning-path.png`               | `workspace-owner/`                                             | Generated |
| `fabric-enthusiast-learning-path.png`             | `fabric-enthusiast/`                                           | Generated |
| `fabric-deployment-lifecycle.png`                 | `06-deployment-lifecycle-management/`                          | Generated |
| `fabric-connections-refresh-monitoring-model.png` | `07-connections-refresh-monitoring/`                           | Generated |
| `fabric-data-semantic-modelling-layers.png`       | `08-data-and-semantic-modelling/`                              | Generated |
| `hdb-resales-sandbox-experiment-map.png`          | `09-sandbox-experiments/hdb-resales/`                          | Generated |
| `curated-learning-resources-overview.png`         | `10-curated-learning-resources/`                               | Generated |
| `templates-checklists-overview.png`               | `11-templates-checklists/`                                     | Generated |

Image file names should use lower-case kebab-case.

## Future maturity options

The following items may be added later as Fabric adoption matures:

| Future Area            | Possible Addition                                                      |
| ---------------------- | ---------------------------------------------------------------------- |
| Shared semantic models | Guidance on endorsed or certified semantic models                      |
| Central data products  | Guidance on reusable curated datasets                                  |
| AI-ready data          | Deeper semantic layer and ontology-style documentation                 |
| Data concierge         | Link to internal metadata discovery or catalogue work                  |
| CI/CD                  | More detailed deployment pipeline and Git integration patterns         |
| Capacity monitoring    | More detailed guidance on workload monitoring and optimisation         |
| Training delivery      | Facilitator guide, workshop plan, and exercises                        |
| Assessment             | Learner completion checklist or quiz                                   |
| Support model          | Escalation matrix for BIA, IT, vendor, and department owner            |
| Governance maturity    | More formal review process for department assets and productionisation |

## Recommended next build steps

The next build steps are:

1. Review remaining persona pathway pages for learner-facing language and workspace-rule consistency
2. Review remaining HDB Resales experiment pages
3. Complete planned HDB Resales data, notebook, and model-output references where needed
4. Review all image links and filenames
5. Review all internal navigation links
6. Review all Microsoft reference links
7. Check that public repo safety expectations are reflected in `CONTRIBUTING.md`
8. Prepare the repo for first internal sharing
