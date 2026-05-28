# HDB Resales: Report Consumer Walkthrough

This hands-on experiment helps learners practise opening, filtering, and interpreting a Power BI report responsibly in the Fabric Sandbox Workspace.

It supports the [Report Consumer Pathway](../../../05-persona-pathways/report-consumer/) and uses the HDB Resales sandbox report as the practice artefact.

## Experiment purpose

The purpose of this experiment is to help learners become comfortable with report consumption in Microsoft Fabric.

In this experiment, learners will practise how to:

* Open the HDB Resales report in the Fabric Sandbox Workspace
* Check report context before interpreting visuals
* Use filters and slicers carefully
* Interact with visuals
* Write one responsible interpretation
* Identify caveats and follow-up questions
* Recognise what not to do with sandbox reports

## Learning level

| Area                | Details                                                       |
| ------------------- | ------------------------------------------------------------- |
| Level               | Beginner                                                      |
| Main persona        | Report Consumer                                               |
| Supporting personas | Department Representative, Fabric Enthusiast, Workspace Owner |
| Estimated time      | 30 to 45 minutes                                              |
| Main artefact       | HDB Resales sandbox report                                    |
| Workspace           | Fabric Sandbox Workspace                                      |

## Fabric Sandbox Workspace link

Use the link below to access the Fabric Sandbox Workspace or the published HDB Resales report.

```text
Fabric Sandbox Workspace URL:
[insert Fabric Sandbox Workspace URL here]

HDB Resales Report URL:
[insert published HDB Resales report URL here]
```

If you cannot access the workspace or report, check with the workspace owner or BIA contact.

## Before you start

Complete the following foundation sections first:

* [Start Here](../../../00-start-here/)
* [Security, Access and Governance](../../../01-security-access-governance/)
* [Licensing, Capacity and Compute Awareness](../../../02-licensing-capacity/)
* [Fabric Workspace Operating Model](../../../03-workspace-operating-model/)
* [Start Using Fabric](../../../04-start-using-fabric/)

You should also understand the role expectations in:

* [Report Consumer Pathway](../../../05-persona-pathways/report-consumer/)

## Required artefacts

For this walkthrough, use the published HDB Resales report in the Fabric Sandbox Workspace.

The source PBIX reference file is stored in the repo at:

```text
09-sandbox-experiments/hdb-resales/assets/HDB_Resales.pbix
```

Report consumers should usually interact with the published report in the Fabric Sandbox Workspace. They are not expected to edit the PBIX file.

## Safety reminder

This is a sandbox learning activity.

Use only:

* Public data
* Mocked data
* Synthetic data
* Approved non-sensitive data

Do not upload or use:

* Confidential institutional data
* Restricted institutional data
* Student personal data
* Staff personal data
* Financial records
* Donor records
* Operational production data

The HDB Resales report is a learning artefact. It should not be treated as an official report, valuation tool, production dashboard, or formal decision-support tool.

## Walkthrough overview

![Report consumer walkthrough](../../../assets/images/report-consumer-sandbox-learning-path.png)

## Activity 1: Open the HDB Resales report

### Goal

Find and open the HDB Resales report in the Fabric Sandbox Workspace.

### Steps

1. Sign in to Microsoft Fabric.
2. Open the Fabric Sandbox Workspace using the provided link.
3. Locate the HDB Resales report.
4. Open the report in reading mode.
5. Identify the report title.
6. Identify the purpose of the report.
7. Confirm that the report is a sandbox learning artefact.

### Output

Complete the following:

```text
Report name:
Workspace:
Report purpose:
Report status:
```

### Reflection questions

* Is the report clearly labelled?
* Is the report purpose easy to understand?
* Is it clear that this is a sandbox artefact?

## Activity 2: Check report context

### Goal

Understand the report context before interpreting the visuals.

### Steps

1. Check the report title.
2. Check the report owner or contact point, if available.
3. Check the refresh date or data currency indicator, if available.
4. Check whether a sensitivity label is applied.
5. Check whether the report provides notes, definitions, or caveats.
6. Identify whether the source or semantic model is visible to you.

### Output

Complete the following:

```text
Report name:
Workspace:
Report purpose:
Report owner or contact:
Refresh date:
Sensitivity label:
Important caveats:
Questions to clarify:
```

You may also use:

[Report Context Note](../../../11-templates-checklists/templates/report-context-note.md)

### Reflection questions

* Is the report recent enough for its intended purpose?
* Are the main terms or measures clearly explained?
* Who would you ask if the numbers appear incorrect?

## Activity 3: Use filters and slicers

### Goal

Understand how filters and slicers affect report interpretation.

### Steps

1. Open the HDB Resales report.
2. Select a slicer or filter, such as town, flat type, year, or resale price range.
3. Observe how the visuals change.
4. Clear the filter.
5. Apply a different filter.
6. Compare the before-and-after view.
7. Note whether the filter affects one visual, one page, or the whole report.

### Output

Complete the following:

```text
Filter or slicer used:
What changed:
What did not change:
Possible interpretation:
Possible caveat:
```

### Reflection questions

* Did the filter affect all visuals or only some visuals?
* Could someone misinterpret the report if they forget a filter is applied?
* Does the report make active filters obvious?

## Activity 4: Interact with visuals

### Goal

Understand how selecting one visual can affect other visuals.

### Steps

1. Select a bar, line point, category, map area, or visual element.
2. Observe how the other visuals respond.
3. Identify whether the interaction filters, highlights, or does not affect other visuals.
4. Clear the selection.
5. Repeat with another visual.
6. Note which interaction is helpful and which may be confusing.

### Output

Complete the following:

```text
Visual selected:
Other visuals affected:
Type of effect observed:
Insight gained:
Possible caveat:
```

### Reflection questions

* Did the interaction make the pattern clearer?
* Could the interaction accidentally hide important context?
* Would a new user know that a visual selection is active?

## Activity 5: Interpret one insight responsibly

### Goal

Write one useful observation without overclaiming.

### Steps

1. Choose one chart, KPI, or visual from the report.
2. Apply one appropriate filter, if useful.
3. Write one observation.
4. Add one caveat.
5. Add one follow-up question.

### Output

Use this structure:

```text
Observation:
The report appears to show that...

Caveat:
This should be interpreted carefully because...

Follow-up question:
Before using this for a real decision, I would ask...
```

### Example

```text
Observation:
The report appears to show that resale prices differ across towns and flat types.

Caveat:
This should be interpreted carefully because price differences may also be affected by flat size, remaining lease, storey range, transaction year, and location-specific factors.

Follow-up question:
Before using this for a real decision, I would ask whether the report controls for flat type, floor area, remaining lease, and transaction period.
```

You may also use:

[Insight Summary Template](../../../11-templates-checklists/templates/insight-summary-template.md)

## Activity 6: Identify what not to conclude

### Goal

Recognise the limits of report interpretation.

### Steps

1. Review your observation from Activity 5.
2. Identify one conclusion that would be too strong.
3. Identify one missing context point.
4. Identify one additional data item that would improve interpretation.

### Output

Complete the following:

```text
Observation reviewed:
Conclusion that would be too strong:
Missing context:
Additional data needed:
Why this matters:
```

### Reflection questions

* Does the report support explanation, or only description?
* Could a user mistake correlation for causation?
* Could a filtered view be mistaken for the whole picture?

## Activity 7: Know what not to do

### Goal

Understand responsible behaviour when using sandbox reports.

### Steps

Review the following statements and confirm that you understand them.

Report consumers should not:

* Treat sandbox reports as official reports
* Export data unless permitted
* Forward screenshots without context
* Share report links with unauthorised users
* Assume that all numbers are validated for production use
* Ignore filters or slicers that may affect the view
* Use outdated reports for current decisions
* Interpret a visual without understanding the definition behind it

### Output

Complete the following:

```text
One action I should avoid:
Why this matters:
Who I should ask if unsure:
```

## Completion evidence

At the end of this experiment, learners should have:

* A completed report context note
* One filter or slicer observation
* One visual interaction observation
* One responsible interpretation with caveat
* One note on what not to conclude
* One note on what not to do with sandbox reports

## Checklist

Before completing this experiment, confirm:

* [ ] I opened the HDB Resales report in the Fabric Sandbox Workspace
* [ ] I confirmed the report is a sandbox learning artefact
* [ ] I checked report context
* [ ] I used at least one filter or slicer
* [ ] I interacted with at least one visual
* [ ] I wrote one observation with a caveat
* [ ] I identified one conclusion that would be too strong
* [ ] I identified one action I should avoid
* [ ] I understand that this report is not an official production report

## Related templates and checklists

| Resource                                                                                           | Purpose                                                            |
| -------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------ |
| [Report Context Note](../../../11-templates-checklists/templates/report-context-note.md)           | Record report purpose, owner, refresh date, caveats, and questions |
| [Insight Summary Template](../../../11-templates-checklists/templates/insight-summary-template.md) | Write an observation with caveat and follow-up question            |
| [Report Review Checklist](../../../11-templates-checklists/checklists/report-review-checklist.md)  | Review whether a report is clear, safe, and fit for use            |

## Related pathway

This experiment supports:

[Report Consumer Pathway](../../../05-persona-pathways/report-consumer/)

## Next experiment

Proceed to:

[HDB Resales: Dashboard Design and Storytelling](../02-dashboard-design-and-storytelling/)
