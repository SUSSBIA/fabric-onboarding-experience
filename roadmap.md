# Roadmap

This roadmap explains how the Fabric Onboarding Experience is expected to evolve.

The repo is designed as a living onboarding resource. It starts with foundational guidance, then grows into persona pathways, sandbox experiments, reusable templates, and more advanced operating practices as Fabric adoption matures.

## Roadmap principles

The roadmap follows these principles:

- Start with safety, access, and governance before hands-on use
- Use sandbox-first onboarding for all learners
- Use public, mocked, synthetic, or approved non-sensitive data for learning
- Build pathways for different user personas
- Use HDB Resales as the initial common sandbox learning project
- Keep BIA production workspaces controlled
- Avoid creating unmanaged self-service sprawl
- Grow towards reusable semantic models, trusted data assets, and AI-ready analytics over time

## Current operating assumptions

The current Fabric operating model is based on:

| Area | Current Assumption |
|---|---|
| Staff licensing | Staff access is supported through Office 365 Education A5, which includes Power BI Pro capabilities |
| Capacity | BIA has provisioned F64 capacity for University analytics workloads |
| Sandbox onboarding | All learners begin in sandbox workspaces |
| Department workspaces | Department workspaces support approved exploration and development |
| Production workspaces | BIA production workspaces are reserved for BIA-managed production assets |
| Shared central workspace | No formal shared or central workspace model currently exists |
| Tenant-level settings | Relevant Fabric tenant-level settings are controlled by BIA and should be escalated to BIA for review |
| External collaborators | External collaborators may require Microsoft Entra B2B guest access and licensing review |

## Phase 1: Foundation onboarding

Status: In progress

This phase establishes the common foundation that all users should understand before using Fabric hands-on.

| Section | Purpose | Status |
|---|---|---|
| `00-start-here/` | Explain the onboarding journey and sandbox-first approach | Drafted |
| `01-security-access-governance/` | Explain security, access, sensitivity labels, RLS awareness, and escalation | Drafted |
| `02-licensing-capacity/` | Explain A5 licensing, Power BI Pro, F64 capacity, and responsible compute use | Drafted |
| `03-workspace-operating-model/` | Explain sandbox, department, and BIA production workspace patterns | Drafted |
| `04-start-using-fabric/` | Guide users into their first safe Fabric activities in sandbox | Drafted |

## Phase 2: Persona pathways

Status: In progress

This phase provides role-based learning pathways so users do not need to learn every Fabric capability at once.

| Pathway | Purpose | Status |
|---|---|---|
| `05-persona-pathways/README.md` | Gateway page for choosing a pathway | Drafted |
| `report-consumer/` | Learn to open, filter, and interpret reports responsibly | Drafted |
| `report-developer/` | Learn report design, semantic model awareness, measures, validation, and caveats | Drafted |
| `data-analyst/` | Learn data exploration, analytical questions, comparisons, trends, and insight summaries | Drafted |
| `data-engineer/` | Learn Lakehouse ingestion, cleaning, layering, transformation, and refresh thinking | Drafted |
| `data-scientist/` | Learn modelling, clustering, evaluation, responsible interpretation, and model documentation | Drafted |
| `department-representative/` | Learn use case framing, ownership, access, sensitivity, and BIA engagement | Drafted |
| `workspace-owner/` | Learn workspace health, access, naming, ownership, and escalation practices | Drafted |
| `fabric-enthusiast/` | Learn safe exploration across Fabric capabilities | Drafted |

## Phase 3: Responsible-use modules

Status: Drafted

These sections support more sustainable Fabric use beyond basic onboarding.

| Section | Purpose | Status |
|---|---|---|
| `06-deployment-lifecycle-management/` | Explain movement from sandbox to department workspace to BIA production where applicable | Drafted |
| `07-connections-refresh-monitoring/` | Explain connections, credentials, gateways, refresh, monitoring, and failure handling | Drafted |
| `08-data-and-semantic-modelling/` | Explain grain, measures, semantic models, RLS, reuse, and AI-ready data | Drafted |

## Phase 4: HDB Resales Sandbox Series

Status: Planned

This phase builds the hands-on practice layer of the onboarding experience.

The initial sandbox project is based on public HDB resale flat data. It is safe, relatable, and rich enough to support multiple learning pathways.

| Experiment | Purpose | Status |
|---|---|---|
| `09-sandbox-experiments/README.md` | Catalogue of all sandbox experiments | Drafted |
| `hdb-resales/README.md` | Overview of the HDB Resales Sandbox Series | Planned |
| `01-report-consumer-walkthrough/` | Practise report navigation, filters, slicers, and responsible interpretation | Planned |
| `02-dashboard-design-and-storytelling/` | Practise dashboard design and report storytelling | Planned |
| `03-semantic-model-and-kpi-definitions/` | Practise measures, definitions, semantic modelling, and reuse | Planned |
| `04-lakehouse-ingestion-and-cleaning/` | Practise loading and cleaning HDB resale data in a Lakehouse | Planned |
| `05-market-segmentation/` | Practise clustering or segmentation of resale market patterns | Planned |
| `06-price-trend-and-affordability-analysis/` | Practise trend analysis and cautious interpretation | Planned |
| `07-town-and-flat-type-comparison/` | Practise group comparison across towns and flat types | Planned |
| `08-geospatial-location-analysis/` | Explore location-related analysis where suitable data is available | Planned |
| `09-ai-ready-data-and-semantic-layer/` | Explore semantic meaning, documentation, and AI-ready data concepts | Planned |

## Phase 5: Supporting artefacts

Status: Partially drafted

This phase creates supporting files used by the HDB Resales sandbox series and the persona pathways.

| Artefact Area | Examples | Status |
|---|---|---|
| PBIX | `HDB_Resales.pbix` | Available |
| Data | `hdb_resales_sample.csv`, `hdb_resales_data_dictionary.md` | Planned |
| Notebooks | Data preparation, market segmentation, price band prediction | Planned |
| Templates | Report context note, insight summary, use case canvas, model card | Partially drafted |
| Model outputs | Sandbox model output tables or files | Planned |
| Workspace review artefacts | Workspace inventory, workspace health note | Planned |

## Phase 6: Templates and checklists

Status: Catalogue drafted, individual files pending

The templates and checklists section should remain a clean catalogue. Individual templates and checklists should be created as separate files.

| Resource | Status |
|---|---|
| `11-templates-checklists/README.md` | Drafted |
| `templates/report-context-note.md` | Drafted |
| `templates/insight-summary-template.md` | Drafted |
| `templates/use-case-canvas.md` | Drafted |
| Other templates | Planned |
| Checklists | Planned |

Planned template files:

```text
11-templates-checklists/templates/
├── workspace-inventory-template.md
├── workspace-health-note.md
├── model-card-template.md
├── release-note-template.md
└── refresh-failure-note.md
```

Planned checklist files:

```text
11-templates-checklists/checklists/
├── sandbox-readiness-checklist.md
├── workspace-access-checklist.md
├── report-review-checklist.md
├── semantic-model-review-checklist.md
├── rls-testing-checklist.md
├── refresh-monitoring-checklist.md
├── productionisation-readiness-checklist.md
└── external-collaborator-checklist.md
```

## Phase 7: Curated learning resources

Status: Drafted

This section gathers official Microsoft documentation, Microsoft Learn resources, and curated video learning references.

| Area | Status |
|---|---|
| Microsoft Fabric overview | Drafted |
| Security, access, and governance | Drafted |
| Licensing and capacity | Drafted |
| Workspaces and operating model | Drafted |
| Power BI report consumers | Drafted |
| Report development and dashboard design | Drafted |
| Data analytics and modelling | Drafted |
| Data engineering | Drafted |
| Data Factory, pipelines, and Dataflow Gen2 | Drafted |
| Connections, gateways, refresh, and monitoring | Drafted |
| Data science and machine learning | Drafted |
| Deployment lifecycle management | Drafted |
| Adoption and governance | Drafted |
| Curated video inventory | Placeholder drafted |

## Phase 8: Image and visual polish

Status: In progress

Images are stored in:

```text
assets/images/
```

Generated or planned images include:

| Image | Used In | Status |
|---|---|---|
| `layered-fabric-onboarding-journey.png` | `00-start-here/` | Generated |
| `fabric-access-and-governance-layers.png` | `01-security-access-governance/` | Generated |
| `fabric-licensing-capacity-model.png` | `02-licensing-capacity/` | Generated |
| `fabric-workspace-operating-model.png` | `03-workspace-operating-model/` | Generated |
| `first-safe-steps-in-fabric-sandbox.png` | `04-start-using-fabric/` | Generated |
| `persona-pathways-fabric-onboarding.png` | `05-persona-pathways/` | Generated |
| `report-consumer-sandbox-learning-path.png` | `report-consumer/` | Generated |
| `report-developer-sandbox-learning-path.png` | `report-developer/` | Generated |
| `data-analyst-hdb-resales-learning-path.png` | `data-analyst/` | Generated |
| `data-engineer-hdb-resales-learning-path.png` | `data-engineer/` | Generated |
| `data-scientist-hdb-resales-learning-path.png` | `data-scientist/` | Generated |
| `department-representative-learning-path.png` | `department-representative/` | Generated |
| `workspace-owner-learning-path.png` | `workspace-owner/` | Generated |
| `fabric-enthusiast-learning-path.png` | `fabric-enthusiast/` | Generated |
| `fabric-deployment-lifecycle.png` | `06-deployment-lifecycle-management/` | Generated |
| `fabric-connections-refresh-monitoring-model.png` | `07-connections-refresh-monitoring/` | Generated |
| `fabric-data-semantic-modelling-layers.png` | `08-data-and-semantic-modelling/` | Generated |
| `hdb-resales-sandbox-experiment-map.png` | `09-sandbox-experiments/` | Generated |
| `curated-learning-resources-overview.png` | `10-curated-learning-resources/` | Generated |
| `templates-checklists-overview.png` | `11-templates-checklists/` | Generated |

Image file names should use lower-case kebab-case.

## Phase 9: Root README finalisation

Status: Next

The root `README.md` should be created after the main sections are stable.

It should act as the front door of the repo and include:

- Short description
- Why the repo exists
- Who it is for
- Recommended onboarding flow
- Repo navigation table
- Sandbox-first principle
- HDB Resales Sandbox Series summary
- Current operating model
- Important cautions
- Links to glossary and roadmap

## Future maturity options

The following items may be added later as Fabric adoption matures:

| Future Area | Possible Addition |
|---|---|
| Shared semantic models | Guidance on endorsed or certified semantic models |
| Central data products | Guidance on reusable curated datasets |
| AI-ready data | Deeper semantic layer and ontology-style documentation |
| Data concierge | Link to internal metadata discovery or catalogue work |
| CI/CD | More detailed deployment pipeline and Git integration patterns |
| Capacity monitoring | More detailed guidance on workload monitoring and optimisation |
| Training delivery | Facilitator guide, workshop plan, and exercises |
| Assessment | Learner completion checklist or quiz |
| Support model | Escalation matrix for BIA, IT, vendor, and department owner |
| Governance maturity | More formal review process for department assets and productionisation |

## Recommended next build steps

The next build steps are:

1. Create the root `README.md`
2. Build `09-sandbox-experiments/hdb-resales/README.md`
3. Build the individual HDB Resales experiment pages
4. Complete remaining templates
5. Complete checklists
6. Review all image links and filenames
7. Review all internal navigation links
8. Review all Microsoft reference links
9. Prepare the repo for first internal sharing
