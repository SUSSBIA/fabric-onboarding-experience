# Contributing to the Fabric Onboarding Guide

This document is for contributors and maintainers of the Fabric Onboarding Guide.

The main repo content is learner-facing. This file explains how to maintain the repo safely, consistently, and in a way that supports the onboarding design pattern.

## Purpose of this repo

This repo is a learner-facing onboarding guide for Microsoft Fabric.

It helps users:

* Understand Fabric onboarding expectations
* Choose the right persona pathway
* Complete safe sandbox experiments
* Use templates and checklists
* Understand workspace boundaries
* Avoid treating sandbox outputs as official production assets

The repo should remain readable, practical, and safe for learners.

## Public repo safety checklist

This repo may be publicly visible. Do not commit internal or sensitive information.

Do not place the following in this repo:

* Direct Fabric workspace links
* Direct report links
* Direct semantic model links
* Direct Lakehouse links
* Internal SharePoint or Teams links
* Confidential institutional data
* Restricted institutional data
* Student personal data
* Staff personal data
* Financial records
* Donor records
* Operational production data
* Secrets, tokens, credentials, or connection strings

Use generic Microsoft Fabric access instructions where needed:

```text
https://app.fabric.microsoft.com/
```

Actual workspace and artefact links should be shared through internal BIA onboarding channels, not committed to this repo.

## Learner-facing writing principle

Most README files in this repo should be written for learners, not maintainers.

Use learner-facing wording such as:

```text
Use the assigned Fabric Sandbox Workspace.
Open the HDB Resales report.
Complete the following activity.
Record your observation.
```

Avoid maintainer-facing wording in learner pages, such as:

```text
These files should be made available.
Add this later.
Suggested placeholder.
To be created.
Upload the artefact when ready.
```

If maintainer notes are needed, place them in this `CONTRIBUTING.md` file or a clearly marked maintainer document.

## Repo versus Fabric Sandbox Workspace

The repo and Fabric Sandbox Workspace have different roles.

| Area                     | Purpose                                                                                                       |
| ------------------------ | ------------------------------------------------------------------------------------------------------------- |
| GitHub repo              | Stores onboarding instructions, README files, templates, checklists, source references, and learning guidance |
| Fabric Sandbox Workspace | Hosts the working artefacts that learners open, run, edit, copy, and practise with                            |

The repo explains what to do.

The Fabric Sandbox Workspace is where the hands-on work happens.

Do not make the repo look like the primary working environment for learners.

## Content design pattern

Use this pattern consistently:

```text
Persona pathway README = curriculum map
Sandbox experiment README = hands-on lesson worksheet
```

## Persona pathway README pattern

Persona pathway READMEs should explain what a learner in that role should know.

They should include:

* Who this pathway is for
* Learning objectives
* Prerequisites
* Key responsibilities
* Key principles
* What learners should not do
* Expected completion evidence
* Related templates and checklists
* Recommended hands-on experiments

They should not duplicate detailed step-by-step exercises.

Detailed hands-on steps belong in sandbox experiment READMEs.

## Sandbox experiment README pattern

Sandbox experiment READMEs should act as lesson worksheets.

They should include:

* Experiment purpose
* Learning level
* Main persona
* Supporting personas
* Required artefacts
* Workspace boundary
* Safety reminder
* Step-by-step activities
* Outputs for each activity
* Reflection questions
* Completion evidence
* Related templates and checklists
* Related pathway
* Next experiment

Sandbox experiment pages should be practical and action-oriented.

## Workspace boundary principle

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

## Department workspace owner and deputy rule

Department workspace requests should identify both:

* A workspace owner
* A deputy workspace owner

This is required so that a department workspace does not depend on a single person.

The deputy owner helps ensure continuity if the workspace owner leaves, changes role, or is unavailable.

This rule should be reflected in:

* `03-workspace-operating-model/README.md`
* `11-templates-checklists/checklists/workspace-access-checklist.md`
* `11-templates-checklists/checklists/productionisation-readiness-checklist.md`
* `11-templates-checklists/templates/workspace-inventory-template.md`
* `11-templates-checklists/templates/workspace-health-note.md`

## BIA Production Workspace rule

BIA Production Workspaces are restricted to BIA users.

Non-BIA users should not be granted direct BIA Production Workspace membership.

Where approved production outputs need to be shared with non-BIA users, sharing should happen through approved report or app sharing channels.

This rule should be reflected in:

* `03-workspace-operating-model/README.md`
* `11-templates-checklists/checklists/workspace-access-checklist.md`
* `11-templates-checklists/checklists/productionisation-readiness-checklist.md`
* `11-templates-checklists/templates/workspace-inventory-template.md`
* `11-templates-checklists/templates/workspace-health-note.md`
* Root `README.md` governance reminders

## File and folder naming

Use clear folder and file names.

Recommended:

```text
report-consumer/
report-developer/
workspace-access-checklist.md
productionisation-readiness-checklist.md
hdb-resales/
01-report-consumer-walkthrough/
```

Avoid vague names such as:

```text
misc/
new/
latest/
final/
copy/
test/
```

## Image asset naming

Store images in:

```text
assets/images/
```

Use descriptive names such as:

```text
fabric-workspace-operating-model.png
report-consumer-sandbox-learning-path.png
hdb-resales-sandbox-experiment-map.png
```

Avoid generic image names such as:

```text
image1.png
diagram.png
new-image.png
final.png
```

## Image use

Images should support learner understanding.

Use images for:

* Workspace boundary models
* Persona learning paths
* Sandbox experiment maps
* Process overviews
* Conceptual diagrams

Each image should have:

* Descriptive alt text
* A short caption
* A stable file name
* A clear placement in the relevant README

## Public data and sample files

Public sample datasets may be referenced or included where appropriate.

Before adding data files, check that:

* The data is public, mocked, synthetic, or approved non-sensitive data
* The data does not contain personal, confidential, restricted, or operational production information
* The file size is reasonable for the repo
* The data supports a clear learning purpose
* The README explains how learners should use it

Do not add real institutional data to this repo.

## Fabric links

Do not commit direct internal Fabric links.

Use generic instructions instead:

```text
Go to https://app.fabric.microsoft.com/
Sign in using your University account.
Open the assigned Fabric Sandbox Workspace.
```

Specific workspace and artefact links should be distributed internally.

## Power BI and PBIX files

Avoid storing PBIX files in this public learner-facing repo unless there is a clear reason and approval.

PBIX files are binary, harder to review, and may contain model details, data, connection information, or metadata that should not be exposed.

For learner-facing guidance, prefer:

* Published reports in Fabric Sandbox Workspace
* Instructions in README files
* Public CSV sample data where suitable
* Power Query steps documented as learning activities
* Templates and checklists

## Markdown style

Use clear, plain Markdown.

Recommended:

* Short paragraphs
* Clear headings
* Tables for structured comparison
* Checklists for learner confirmation
* Code fences for file paths, formulas, and examples
* Relative links within the repo

Avoid:

* Overly long paragraphs
* Internal project notes in learner pages
* Unexplained acronyms
* Placeholder text that looks unfinished
* Raw internal URLs

## Status labels

Use consistent status labels.

Recommended labels:

```text
Planned
Drafted
In development
Ready for review
Published
Retired
```

Avoid unclear labels such as:

```text
Done?
Maybe
TBC
Final final
```

## Review checklist before committing

Before committing changes, check:

* [ ] The content is learner-facing unless it belongs in `CONTRIBUTING.md`
* [ ] No internal Fabric workspace, report, semantic model, or Lakehouse links are included
* [ ] No confidential, restricted, personal, financial, donor, or production data is included
* [ ] No secrets, tokens, credentials, or connection strings are included
* [ ] Workspace boundary rules are consistent
* [ ] Department workspace owner and deputy owner requirement is reflected where relevant
* [ ] BIA Production Workspace access is described as restricted to BIA users
* [ ] Non-BIA production consumption is described as approved report/app sharing, not direct workspace membership
* [ ] Links are relative and working
* [ ] Image paths are correct
* [ ] The content does not duplicate detailed hands-on steps in persona pathway pages
* [ ] Sandbox experiment pages include completion evidence and reflection questions

## Recommended update workflow

When adding or changing an onboarding section:

1. Decide whether the content is learner-facing or maintainer-facing.
2. If learner-facing, place it in the relevant README.
3. If maintainer-facing, place it in this file or a maintainer note.
4. Check whether the change affects workspace boundary rules.
5. Check whether templates or checklists need updates.
6. Check whether persona pathways and sandbox experiments remain clearly separated.
7. Review the page as if you are a new learner.

## Questions

If a contributor is unsure whether something should be added, ask:

* Is this useful to a learner?
* Is this safe for a public repo?
* Does this belong in the repo or in the Fabric Sandbox Workspace?
* Is this a curriculum map or a hands-on worksheet?
* Does this expose internal information?
* Does this create confusion about workspace boundaries?

When in doubt, keep learner pages simple and move maintainer guidance to this file.
