# Model Card Template

Use this template to document a sandbox model, clustering output, predictive model, scoring logic, or advanced analytics experiment.

This is especially useful for data scientists, data analysts, reviewers, and anyone who needs to interpret or explain model outputs responsibly.

A model card should help users understand:

* What the model or experiment is for
* What data was used
* What method was applied
* What the output means
* What the output should not be used for
* What limitations, caveats, and risks are present
* Whether the output should remain sandbox or move towards review

## 1. Model or Experiment Summary

| Field                                                     | Response                                                                              |
| --------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| Model or experiment name                                  |                                                                                       |
| Workspace                                                 |                                                                                       |
| Workspace type                                            | Personal / Sandbox / Department / BIA Production                                      |
| Related sandbox experiment or use case                    |                                                                                       |
| Owner                                                     |                                                                                       |
| Workspace owner                                           |                                                                                       |
| Deputy workspace owner, if applicable                     |                                                                                       |
| Reviewer                                                  |                                                                                       |
| Date created                                              |                                                                                       |
| Date reviewed                                             |                                                                                       |
| Status                                                    | Sandbox / Draft / Prototype / Review / Department / Production candidate / Production |
| Related report, notebook, semantic model, or output table |                                                                                       |

## 2. Purpose and Intended Use

| Question                                               | Response |
| ------------------------------------------------------ | -------- |
| What question does this model or experiment address?   |          |
| Why was this model or experiment created?              |          |
| Who is the intended audience?                          |          |
| What decision, discussion, or analysis may it support? |          |
| What is the intended use?                              |          |
| What is it not intended for?                           |          |

## 3. Workspace and Use Boundary

| Workspace Type           | Model Use Expectation                                                                                      |
| ------------------------ | ---------------------------------------------------------------------------------------------------------- |
| Personal Workspace       | Suitable only for private exploration and drafts using safe data                                           |
| Sandbox Workspace        | Suitable for learning and experimentation using public, mocked, synthetic, or approved non-sensitive data  |
| Department Workspace     | Suitable for approved department-level exploration or prototypes with clear owner and deputy owner         |
| BIA Production Workspace | Suitable for BIA-managed production analytics assets, with direct workspace access restricted to BIA users |

Confirm:

* [ ] The model or experiment is in the correct workspace for its purpose
* [ ] Personal workspace outputs are not being treated as shared or official assets
* [ ] Sandbox outputs are clearly labelled as learning or experimental
* [ ] Department workspace outputs have clear owner and deputy owner, where applicable
* [ ] BIA Production Workspace access remains restricted to BIA users, where applicable
* [ ] Non-BIA users consume approved production outputs through approved report or app sharing channels, where applicable

## 4. Use Case Type

Select the closest use case type.

| Use Case Type              | Select One | Notes                                |
| -------------------------- | ---------- | ------------------------------------ |
| Descriptive profiling      |            | Summarises patterns or profiles      |
| Segmentation or clustering |            | Groups similar records               |
| Classification             |            | Predicts a category or class         |
| Regression                 |            | Predicts a continuous value          |
| Forecasting                |            | Predicts future values over time     |
| Scoring or ranking         |            | Produces a score or priority order   |
| Recommendation             |            | Suggests possible actions or options |
| Other                      |            |                                      |

## 5. Data Used

| Field                                 | Response                                                                      |
| ------------------------------------- | ----------------------------------------------------------------------------- |
| Input dataset or table                |                                                                               |
| Data source                           |                                                                               |
| Data owner                            |                                                                               |
| Data steward or subject matter expert |                                                                               |
| Data period covered                   |                                                                               |
| Number of records                     |                                                                               |
| Unit of analysis / grain              |                                                                               |
| Sensitivity label                     | Confidential - SUSS / Restricted - SUSS / Unrestricted - SUSS / None / Unsure |
| Is the data approved for this use?    | Yes / No / Unsure                                                             |
| Data limitations                      |                                                                               |

## 6. Feature Summary

List the fields used to generate the model or output.

| Feature Group                             | Fields Used | Notes |
| ----------------------------------------- | ----------- | ----- |
| Numeric features                          |             |       |
| Categorical features                      |             |       |
| Date or time features                     |             |       |
| Derived features                          |             |       |
| Excluded fields                           |             |       |
| Fields that may introduce leakage         |             |       |
| Fields that require domain interpretation |             |       |
| Sensitive or high-risk fields, if any     |             |       |

## 7. Target or Output

| Field                                     | Response                                                                   |
| ----------------------------------------- | -------------------------------------------------------------------------- |
| Target variable, if applicable            |                                                                            |
| Output type                               | Cluster / Segment / Prediction / Score / Classification / Forecast / Other |
| Output field name                         |                                                                            |
| Output table or file                      |                                                                            |
| Output location                           |                                                                            |
| Output refresh or rerun requirement       | One-off / Recurring / Unsure                                               |
| How should the output be interpreted?     |                                                                            |
| How should the output not be interpreted? |                                                                            |

## 8. Method Used

| Field                                  | Response                                                                            |
| -------------------------------------- | ----------------------------------------------------------------------------------- |
| Method used                            | Clustering / Classification / Regression / Forecasting / Rule-based scoring / Other |
| Algorithm or technique                 |                                                                                     |
| Tool used                              | Fabric notebook / AutoML / Python / PySpark / Power BI / Other                      |
| Notebook, script, or workflow location |                                                                                     |
| Key parameters or settings             |                                                                                     |
| Baseline or comparison method, if any  |                                                                                     |
| Reason this method was chosen          |                                                                                     |

## 9. Evaluation or Profiling

Use this section to summarise how the output was checked.

For clustering or segmentation:

| Question                                                      | Response           |
| ------------------------------------------------------------- | ------------------ |
| How many clusters or segments were produced?                  |                    |
| Are the clusters interpretable?                               | Yes / No / Unsure  |
| What variables distinguish the clusters?                      |                    |
| Are any clusters too small or too broad?                      |                    |
| Was the cluster output reviewed by a subject matter expert?   | Yes / No / Not yet |
| Are the segment labels understandable to non-technical users? | Yes / No / Unsure  |

For classification, regression, scoring, or forecasting:

| Question                                                                             | Response                  |
| ------------------------------------------------------------------------------------ | ------------------------- |
| Evaluation metric used                                                               |                           |
| Main result                                                                          |                           |
| Baseline or comparison                                                               |                           |
| Does performance appear acceptable for the intended use?                             | Yes / No / Unsure         |
| Known weaknesses                                                                     |                           |
| Additional validation needed                                                         |                           |
| Has the model been tested on a suitable holdout or future dataset, where applicable? | Yes / No / Not applicable |

## 10. Plain-Language Interpretation

Summarise the output in plain language.

| Area                                            | Response |
| ----------------------------------------------- | -------- |
| What the output appears to suggest              |          |
| What this may be useful for                     |          |
| What users should be careful about              |          |
| What should not be concluded from this output   |          |
| What follow-up question should be explored next |          |

## 11. Limitations and Caveats

| Limitation or Caveat                     | Notes |
| ---------------------------------------- | ----- |
| Data quality limitations                 |       |
| Missing variables or missing context     |       |
| Sample size concerns                     |       |
| Time period limitations                  |       |
| Feature limitations                      |       |
| Model performance concerns               |       |
| Stability concerns                       |       |
| Interpretability concerns                |       |
| Operational limitations                  |       |
| Fairness or bias concerns, if applicable |       |
| Other caveats                            |       |

## 12. Risks of Misuse

| Risk                                                 | Notes |
| ---------------------------------------------------- | ----- |
| Users may treat the output as a final decision       |       |
| Users may overinterpret correlations or patterns     |       |
| Users may ignore caveats or limitations              |       |
| Users may apply the output to the wrong population   |       |
| Users may use the output beyond the approved purpose |       |
| Users may assume the model is production-ready       |       |
| Users may treat sandbox output as official           |       |
| Other risk                                           |       |

## 13. Responsible Use Guidance

| Question                                              | Response          |
| ----------------------------------------------------- | ----------------- |
| Should this output be used for real decisions?        | Yes / No / Unsure |
| Should this remain sandbox?                           | Yes / No / Unsure |
| What caveat must accompany the output?                |                   |
| Who should validate the output before wider use?      |                   |
| What approval is needed before moving beyond sandbox? |                   |
| Is BIA review required?                               | Yes / No / Unsure |
| Is productionisation review required?                 | Yes / No / Unsure |

## 14. Connection to Reporting or Dashboards

| Question                                                                                        | Response                  |
| ----------------------------------------------------------------------------------------------- | ------------------------- |
| Will the output be shown in a report or dashboard?                                              | Yes / No / Unsure         |
| Which report or dashboard may consume it?                                                       |                           |
| Are caveats visible in the report?                                                              | Yes / No / Unsure         |
| Could report users misinterpret the output?                                                     | Yes / No / Unsure         |
| Is the output clearly marked as sandbox, experimental, department-facing, or production-facing? | Yes / No / Unsure         |
| Has the report review checklist been completed, if applicable?                                  | Yes / No / Not applicable |

## 15. Access, Sharing and Production Boundary

| Question                                                    | Response                                                                 |
| ----------------------------------------------------------- | ------------------------------------------------------------------------ |
| Who is allowed to view the model output?                    |                                                                          |
| Who is allowed to edit or rerun the model?                  |                                                                          |
| Is export allowed?                                          | Yes / No / Unsure                                                        |
| Can the output be shared beyond the workspace?              | Yes / No / Unsure                                                        |
| Is external collaborator access involved?                   | Yes / No / Unsure                                                        |
| If production-facing, what is the approved sharing channel? | Workspace access / Report sharing / App sharing / Other / Not applicable |

Confirm:

* [ ] Access is limited to the intended audience
* [ ] Sensitivity label and data handling expectations are understood
* [ ] Export and screenshot risks are considered
* [ ] Sandbox outputs are not shared as official results
* [ ] If this becomes a BIA production output, direct BIA Production Workspace access remains restricted to BIA users
* [ ] Non-BIA users consume approved production outputs through approved report or app sharing channels, where applicable

## 16. Review and Decision

| Decision Option                         | Select One |
| --------------------------------------- | ---------- |
| Keep as sandbox learning only           |            |
| Improve and rerun                       |            |
| Validate with subject matter expert     |            |
| Discuss as possible department use case |            |
| Escalate to BIA for review              |            |
| Not suitable for further use            |            |

## 17. Follow-Up Actions

| Action | Owner | Target Date | Status                           |
| ------ | ----- | ----------- | -------------------------------- |
|        |       |             | Not started / In progress / Done |
|        |       |             | Not started / In progress / Done |
|        |       |             | Not started / In progress / Done |

## 18. Final Notes

| Area                  | Response |
| --------------------- | -------- |
| Additional notes      |          |
| Recommended next step |          |
| Follow-up owner       |          |
| Follow-up date        |          |
