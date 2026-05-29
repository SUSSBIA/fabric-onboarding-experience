# Report Consumer Pathway

This pathway is for learners who mainly need to view, filter, interpret, and use Power BI reports or dashboards responsibly.

Report consumers are not expected to build data pipelines, create Lakehouses, write notebooks, or design semantic models. Their main responsibility is to understand how to use reports safely, interpret outputs correctly, and avoid inappropriate sharing or export.

This pathway explains what report consumers should know. The hands-on practice is provided separately through the HDB Resales sandbox experiment.

## Who this pathway is for

Choose this pathway if you mainly need to:

* Open assigned reports or dashboards
* Use filters, slicers, and report navigation
* Interpret visuals and summary metrics
* Understand report refresh dates and ownership
* Know whether a report is sandbox, departmental, or production-facing
* Avoid unauthorised sharing, screenshots, or exports
* Raise questions when numbers look incorrect

## Learning objectives

By the end of this pathway, learners should be able to:

* Explain what a report consumer does
* Access the assigned Fabric Sandbox Workspace
* Open an assigned report in the Fabric or Power BI experience
* Check report title, purpose, owner, refresh date, and sensitivity label, where available
* Use filters, slicers, and basic visual interactions responsibly
* Understand how filters and selections affect interpretation
* Explain one insight from a report with appropriate caveats
* Distinguish between sandbox output and production output
* Know when to ask for clarification or escalate an issue
* Avoid unauthorised export, screenshots, or sharing

## Prerequisites

Before starting this pathway, learners should complete:

1. [Start Here](../../00-start-here/)
2. [Security, Access and Governance](../../01-security-access-governance/)
3. [Licensing, Capacity and Compute Awareness](../../02-licensing-capacity/)
4. [Fabric Workspace Operating Model](../../03-workspace-operating-model/)
5. [Start Using Fabric](../../04-start-using-fabric/)

Learners should also know which Fabric Sandbox Workspace they have been assigned to.

## What report consumers should understand

Report consumers should understand that a report is not just a set of visuals.

Before interpreting a report, learners should check:

| Area        | Question                                                                    |
| ----------- | --------------------------------------------------------------------------- |
| Purpose     | What is this report for?                                                    |
| Audience    | Who is supposed to use this report?                                         |
| Status      | Is this sandbox, draft, prototype, department-facing, or production-facing? |
| Owner       | Who owns or maintains the report?                                           |
| Refresh     | How current is the data?                                                    |
| Sensitivity | Is there a sensitivity label?                                               |
| Filters     | Are filters or slicers affecting what I see?                                |
| Definitions | Are the measures and terms clear?                                           |
| Caveats     | What should I be careful not to overinterpret?                              |

This habit helps reduce misinterpretation and prevents sandbox outputs from being treated as official reports.

## Sandbox-first practice

All hands-on practice for this pathway should be completed in the assigned Fabric Sandbox Workspace.

The HDB Resales sandbox report is used because it is based on public and relatable data. It allows learners to practise report consumption and interpretation without using confidential institutional data.

Learners should not upload real confidential or restricted data for this pathway.

![Report consumer sandbox learning path](../../assets/images/report-consumer-sandbox-learning-path.png)

> Image: Report consumer sandbox learning path showing how learners access the sandbox workspace, open a report, check report context, use filters, interact with visuals, interpret one insight responsibly, and identify what not to do.

## Recommended hands-on experiment

Start with:

[HDB Resales: Report Consumer Walkthrough](../../09-sandbox-experiments/hdb-resales/01-report-consumer-walkthrough/)

This experiment gives step-by-step practice in:

* Opening the HDB Resales report in the assigned Fabric Sandbox Workspace
* Checking report context
* Using filters and slicers
* Interacting with visuals
* Writing one responsible interpretation
* Identifying caveats and follow-up questions

The pathway explains what report consumers should learn. The sandbox experiment explains what learners should do.

## Responsible report consumption principles

Report consumers should follow these principles.

### 1. Check context before interpreting

Do not interpret visuals immediately without checking the report purpose, audience, refresh date, and caveats.

### 2. Watch for active filters

Filters, slicers, and visual selections can change the meaning of what is shown.

A filtered view should not be mistaken for the full picture.

### 3. Interpret carefully

A report may show a pattern, but that does not always explain why the pattern exists.

Avoid claiming causality when the report only supports descriptive interpretation.

### 4. Respect sensitivity and sharing rules

Do not export, screenshot, forward, or share reports unless permitted.

Workspace access does not automatically mean onward sharing is allowed.

### 5. Treat sandbox outputs as learning artefacts

Sandbox reports are for practice. They should not be treated as official, validated, or production-ready outputs.

### 6. Ask when numbers look wrong

If numbers look incorrect, outdated, or confusing, ask the report owner, workspace owner, or BIA where appropriate.

Do not quietly rely on a report that appears questionable.

## BIA production output reminder

BIA Production Workspaces are restricted to BIA users.

Non-BIA users should not be granted direct BIA Production Workspace membership.

Where approved BIA production reports or outputs need to be shared with non-BIA users, access should be provided through approved report or app sharing channels.

## What report consumers should not do

Report consumers should not:

* Treat sandbox reports as official reports
* Export data unless permitted
* Forward screenshots without context
* Share report links with unauthorised users
* Assume that all numbers are validated for production use
* Ignore filters or slicers that may affect the view
* Use outdated reports for current decisions
* Interpret a visual without understanding the definition behind it
* Use report access as proof that they are allowed to reuse or redistribute the data

## Expected completion evidence

At the end of this pathway, learners should be able to provide:

* The name of the report used for practice
* A completed report context note
* One filter or slicer observation
* One visual interaction observation
* One responsible interpretation with caveat
* One question they would ask before using the report for a real decision

The hands-on evidence is produced through the HDB Resales report consumer walkthrough.

## Related templates and checklists

| Resource                                                                                        | Purpose                                                                                              |
| ----------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| [Report Context Note](../../11-templates-checklists/templates/report-context-note.md)           | Helps learners record report purpose, owner, refresh date, sensitivity label, caveats, and questions |
| [Insight Summary Template](../../11-templates-checklists/templates/insight-summary-template.md) | Helps learners write an observation with caveat and follow-up question                               |
| [Report Review Checklist](../../11-templates-checklists/checklists/report-review-checklist.md)  | Helps learners review whether a report is clear, safe, and fit for use                               |

## Minimum checklist

Before completing this pathway, learners should confirm:

* [ ] I understand the role of a report consumer
* [ ] I can access the assigned Fabric Sandbox Workspace
* [ ] I can open an assigned report
* [ ] I can identify the report purpose
* [ ] I can check report owner, refresh date, and sensitivity label, if available
* [ ] I can use filters and slicers
* [ ] I understand that filters affect interpretation
* [ ] I can write one insight with a caveat
* [ ] I understand that sandbox reports are not official production reports
* [ ] I know not to export, screenshot, or share unless permitted
* [ ] I know that direct BIA Production Workspace access is restricted to BIA users
* [ ] I know who to ask if something looks wrong

## References and further learning

| Resource                                                                                                                                         | Purpose                                                                                        |
| ------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------- |
| [Interact with reports and dashboards in the Power BI service](https://learn.microsoft.com/en-us/power-bi/explore-reports/end-user-reading-view) | Explains how report consumers use Reading view, filters, Q&A, alerts, and subscriptions        |
| [Navigate the Power BI service](https://learn.microsoft.com/en-us/power-bi/explore-reports/end-user-experience)                                  | Helps users understand dashboards, reports, apps, and workspaces in the Power BI service       |
| [Power BI service basic concepts](https://learn.microsoft.com/en-us/power-bi/fundamentals/service-basic-concepts)                                | Explains key Power BI concepts such as workspaces, reports, dashboards, and semantic models    |
| [How visuals cross-filter each other in a Power BI report](https://learn.microsoft.com/en-us/power-bi/explore-reports/end-user-interactions)     | Explains cross-filtering and cross-highlighting when users interact with visuals               |
| [Feature availability for users in the Power BI service](https://learn.microsoft.com/en-us/power-bi/fundamentals/end-user-features)              | Explains that available features depend on licensing, permissions, and where content is stored |

## Next pathway

Proceed to:

[Report Developer Pathway](../report-developer/)
