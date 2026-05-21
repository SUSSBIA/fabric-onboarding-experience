# Persona Pathways

This section helps users choose the Fabric learning pathway that best matches their role, responsibility, or learning interest.

Not every user needs to learn every Fabric capability. A report consumer does not need to start with pipelines and notebooks. A data engineering learner does not need to start with dashboard design. A department representative may need a broad understanding without becoming a technical expert.

The persona pathways help users focus on what they need first.

## Sandbox-first principle

All persona pathways begin in the sandbox workspace.

For onboarding purposes, users should practise using:

- Mocked data
- Synthetic data
- Public data
- Approved non-sensitive data

Department workspaces and BIA production workspaces are introduced conceptually, but hands-on onboarding activities should happen in sandbox unless BIA explicitly instructs otherwise.

![Placeholder: Persona pathways in Fabric onboarding](../assets/images/persona-pathways-fabric-onboarding.png)

> Image placeholder: A pathway diagram showing different user personas starting from the sandbox workspace, then branching into report consumer, report developer, data analyst, data engineer, data scientist, department representative, workspace owner, and Fabric enthusiast pathways.

## How to choose your pathway

Start by identifying the closest description of your role.

| Persona | Choose this pathway if you mainly need to... |
|---|---|
| Report Consumer | View and interpret approved reports or dashboards |
| Report Developer | Build Power BI reports and work with semantic models |
| Data Analyst | Explore data, prepare analysis, and create insights |
| Data Engineer | Work with Lakehouses, pipelines, notebooks, and data movement |
| Data Scientist | Explore modelling, machine learning, segmentation, or advanced analytics |
| Department Representative | Coordinate department-level Fabric exploration and use cases |
| Workspace Owner | Help manage access, ownership, organisation, and responsible use |
| Fabric Enthusiast | Learn and experiment with Fabric before having a formal use case |

Users may eventually follow more than one pathway, but they should start with the one closest to their immediate need.

## Pathway 1: Report Consumer

Report consumers mainly view, filter, and interpret reports.

They should learn how to:

- Access assigned reports
- Navigate report pages
- Use filters and slicers
- Check report title, owner, refresh date, and sensitivity label
- Understand whether a report is official, draft, or sandbox-only
- Avoid unauthorised sharing, screenshots, or exports
- Raise questions when numbers appear incorrect

Recommended sandbox activities:

1. Open a sample report in the sandbox workspace.
2. Use filters and slicers.
3. Check the refresh date and sensitivity label.
4. Identify the report owner or support contact.
5. Write down one interpretation and one question about the report.

Report consumers should not need to create Lakehouses, pipelines, notebooks, or semantic models at the start.

## Pathway 2: Report Developer

Report developers build reports and may work with semantic models.

They should learn how to:

- Build Power BI reports using approved or sample data
- Understand the difference between a report and a semantic model
- Reuse existing semantic models where appropriate
- Create clear visual layouts
- Define and use measures carefully
- Apply naming conventions
- Understand when Row-Level Security may be needed
- Validate report numbers before sharing
- Avoid creating duplicate or conflicting definitions

Recommended sandbox activities:

1. Open a sample semantic model.
2. Create a simple report using the sample model.
3. Add basic visuals and filters.
4. Create or inspect simple measures.
5. Compare report outputs against expected values.
6. Save the report using a sandbox naming convention.

Report developers should treat semantic models as reusable business layers, not just technical datasets.

## Pathway 3: Data Analyst

Data analysts explore data and turn it into useful insights.

They may work across reports, data preparation, semantic models, and analytical interpretation.

They should learn how to:

- Understand the meaning and structure of a dataset
- Check data quality
- Prepare data for analysis
- Use simple transformations
- Build exploratory reports
- Interpret patterns carefully
- Document assumptions and limitations
- Avoid overclaiming from incomplete data

Recommended sandbox activities:

1. Load or open a sample dataset.
2. Inspect fields, missing values, and data types.
3. Create simple derived fields.
4. Build an exploratory report.
5. Write a short insight summary.
6. List assumptions, caveats, and follow-up questions.

Data analysts should focus not only on producing charts, but also on explaining what the data can and cannot support.

## Pathway 4: Data Engineer

Data engineers work with data ingestion, storage, transformation, and workflow orchestration.

They should learn how to:

- Understand Lakehouse concepts
- Load safe sample data into a Lakehouse
- Distinguish between files and tables
- Use pipelines or Dataflows Gen2 for ingestion
- Use notebooks for transformation
- Understand Bronze, Silver, and Gold layering
- Document source, transformation, and output tables
- Understand refresh, connections, credentials, and monitoring responsibilities

Recommended sandbox activities:

1. Create or open a sandbox Lakehouse.
2. Load mocked or synthetic data.
3. Create a table.
4. Transform the data using a notebook, Dataflow Gen2, or pipeline.
5. Write the output to a curated table.
6. Query the table and verify the result.
7. Document the source-to-output flow.

Data engineering learners should understand that getting data to load once is not the same as operating a reliable data pipeline.

## Pathway 5: Data Scientist

Data scientists and advanced analytics users work with modelling, experimentation, prediction, segmentation, or machine learning.

They should learn how to:

- Use safe and appropriate datasets for modelling
- Understand target variables and features
- Prepare data for modelling
- Apply exploratory analysis
- Build simple models or clustering outputs
- Evaluate model performance
- Interpret results responsibly
- Document limitations and intended use
- Avoid treating model outputs as final truth

Recommended sandbox activities:

1. Open a synthetic dataset.
2. Explore the dataset and define the analytical question.
3. Prepare features.
4. Run a basic model or clustering technique.
5. Evaluate or profile the output.
6. Create a simple dashboard or summary table.
7. Write a short note on limitations and responsible use.

Data science outputs should be treated as decision-support signals, not automated decisions.

## Pathway 6: Department Representative

Department representatives support department-level exploration and coordination.

They may not need to become deep technical experts, but they should understand how Fabric fits into department use cases.

They should learn how to:

- Understand the sandbox-first onboarding model
- Understand department workspace purpose
- Identify potential department use cases
- Coordinate with BIA where needed
- Understand data sensitivity and access boundaries
- Avoid treating prototypes as production assets
- Help validate whether outputs make business sense
- Escalate productionisation needs to BIA

Recommended sandbox activities:

1. Complete a basic report consumer activity.
2. Complete one sandbox experiment relevant to the department.
3. Identify a possible department use case.
4. Describe what data may be needed.
5. Identify the likely owner, audience, and sensitivity level.
6. Discuss whether the use case is exploratory or production-facing.

Department representatives play an important role in translating department needs into responsible analytics use cases.

## Pathway 7: Workspace Owner

Workspace owners or responsible representatives help manage workspace use.

They should learn how to:

- Understand workspace purpose
- Coordinate access requests
- Assign roles appropriately
- Keep workspace content organised
- Ensure sandbox, department, and production boundaries are respected
- Understand who owns reports, semantic models, connections, and refreshes
- Review whether assets are obsolete or duplicated
- Escalate tenant setting, capacity, or productionisation requests to BIA

Recommended sandbox activities:

1. Review the contents of a sample workspace.
2. Identify item owners and item types.
3. Check whether naming is clear.
4. Identify which items are experimental.
5. Review a sample access request scenario.
6. Decide whether a request should be approved, rejected, or escalated.

Workspace ownership is not only technical. It includes accountability for safe and sustainable use.

## Pathway 8: Fabric Enthusiast

Fabric enthusiasts are users who want to explore Fabric before they have a formal department use case.

They should learn how to:

- Use sandbox safely
- Practise with mocked, synthetic, public, or approved non-sensitive data
- Try reports, Lakehouses, semantic models, pipelines, notebooks, and Dataflows Gen2
- Follow guided sandbox experiments
- Reflect on data meaning and responsible interpretation
- Avoid uploading real restricted or confidential data
- Avoid presenting sandbox outputs as official findings

Recommended sandbox activities:

1. Complete the first safe activity.
2. Try one beginner sandbox experiment.
3. Explore one Fabric item type that is new to you.
4. Document what you created.
5. Write down what would need to change before this could be used for a real department use case.

The enthusiast pathway is useful for building future champions, but it should remain safe and clearly separated from production work.

## Suggested progression by maturity

Users can progress through three broad maturity levels.

| Level | Focus | Example Outcome |
|---|---|---|
| Beginner | Navigate Fabric and understand safe use | Can access sandbox and interpret sample reports |
| Practitioner | Build simple assets in sandbox | Can create reports, load data, or run guided exercises |
| Advanced | Apply analytics thinking to realistic scenarios | Can complete sandbox experiments and explain assumptions, risks, and limitations |

Progression should be based on demonstrated understanding, not just tool usage.

## When to move beyond sandbox

Users should only move beyond sandbox when there is a clear reason.

Before moving into a department workspace, confirm:

- There is an approved department use case
- The workspace owner is known
- The data source is approved
- Sensitivity labels and access expectations are understood
- The intended audience is clear
- The output is exploratory, departmental, or production-facing
- BIA involvement is requested if productionisation may be required

Before moving towards BIA production, confirm:

- The asset has been reviewed and validated
- Ownership is clear
- Refresh and monitoring are planned
- Access and RLS, if applicable, have been tested
- Sensitivity labels are applied appropriately
- The release has been agreed with BIA

## Minimum checklist for choosing a pathway

Before selecting a pathway, users should confirm:

- [ ] I know my main purpose for using Fabric
- [ ] I know whether I am consuming, building, engineering, modelling, coordinating, or experimenting
- [ ] I know that onboarding starts in the sandbox workspace
- [ ] I know what data I am allowed to use in sandbox
- [ ] I understand that sandbox outputs are not production assets
- [ ] I know when to ask BIA before moving beyond sandbox

## References and further learning

| Resource | Purpose |
|---|---|
| [Microsoft Learn: Get started with Microsoft Fabric](https://learn.microsoft.com/en-us/training/paths/get-started-fabric/) | Beginner learning path for users who need a broad introduction to Fabric |
| [Get started with Microsoft data analytics](https://learn.microsoft.com/en-us/training/paths/data-analytics-microsoft/) | Useful for users beginning with data analytics, Power BI, and Fabric concepts |
| [Prepare and visualize data with Microsoft Power BI](https://learn.microsoft.com/en-us/training/paths/prepare-visualize-data-power-bi/) | Useful for report consumers, report developers, and analysts learning Power BI reporting |
| [Ingest data with Microsoft Fabric](https://learn.microsoft.com/en-us/training/paths/ingest-data-with-microsoft-fabric/) | Useful for data engineering learners working with ingestion, orchestration, Dataflows Gen2, notebooks, and pipelines |
| [Work with semantic models in Microsoft Fabric](https://learn.microsoft.com/en-us/training/paths/work-semantic-models-microsoft-fabric/) | Useful for users learning semantic model concepts and reusable reporting layers |
| [Implement a data science and machine learning solution with Microsoft Fabric](https://learn.microsoft.com/en-us/training/paths/implement-data-science-machine-learning-fabric/) | Useful for advanced analytics users and data scientists exploring modelling in Fabric |
| [Administer and Govern Microsoft Fabric](https://learn.microsoft.com/en-us/training/paths/microsoft-fabric-admin-governance/) | Useful for workspace owners, administrators, and governance-focused users |

## Next section

Proceed to:

[Deployment Lifecycle Management](../06-deployment-lifecycle-management/)
