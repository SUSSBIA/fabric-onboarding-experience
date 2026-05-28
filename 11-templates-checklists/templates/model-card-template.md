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

| Field                                       | Response                                                     |
| ------------------------------------------- | ------------------------------------------------------------ |
| Model or experiment name                    |                                                              |
| Workspace                                   |                                                              |
| Related sandbox experiment or use case      |                                                              |
| Owner                                       |                                                              |
| Reviewer                                    |                                                              |
| Date created                                |                                                              |
| Date reviewed                               |                                                              |
| Status                                      | Sandbox / Draft / Review / Production candidate / Production |
| Related report, notebook, or semantic model |                                                              |

## 2. Purpose and Intended Use

| Question                                               | Response |
| ------------------------------------------------------ | -------- |
| What question does this model or experiment address?   |          |
| Why was this model or experiment created?              |          |
| Who is the intended audience?                          |          |
| What decision, discussion, or analysis may it support? |          |
| What is the intended use?                              |          |
| What is it not intended for?                           |          |

## 3. Use Case Type

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

## 4. Data Used

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

## 5. Feature Summary

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

## 6. Target or Output

| Field                                 | Response                                                                   |
| ------------------------------------- | -------------------------------------------------------------------------- |
| Target variable, if applicable        |                                                                            |
| Output type                           | Cluster / Segment / Prediction / Score / Classification / Forecast / Other |
| Output field name                     |                                                                            |
| Output table or file                  |                                                                            |
| Output location                       |                                                                            |
| Output refresh or rerun requirement   | One-off / Recurring / Unsure                                               |
| How should the output be interpreted? |                                                                            |

## 7. Method Used

| Field                                  | Response                                                                            |
| -------------------------------------- | ----------------------------------------------------------------------------------- |
| Method used                            | Clustering / Classification / Regression / Forecasting / Rule-based scoring / Other |
| Algorithm or technique                 |                                                                                     |
| Tool used                              | Fabric notebook / AutoML / Python / PySpark / Power BI / Other                      |
| Notebook, script, or workflow location |                                                                                     |
| Key parameters or settings             |                                                                                     |
| Baseline or comparison method, if any  |                                                                                     |
| Reason this method was chosen          |                                                                                     |

## 8. Evaluation or Profiling

Use this section to summarise how the output was checked.

For clustering or segmentation:

| Question                                                    | Response           |
| ----------------------------------------------------------- | ------------------ |
| How many clusters or segments were produced?                |                    |
| Are the clusters interpretable?                             | Yes / No / Unsure  |
| What variables distinguish the clusters?                    |                    |
| Are any clusters too small or too broad?                    |                    |
| Was the cluster output reviewed by a subject matter expert? | Yes / No / Not yet |

For classification, regression, scoring, or forecasting:

| Question                                                 | Response          |
| -------------------------------------------------------- | ----------------- |
| Evaluation metric used                                   |                   |
| Main result                                              |                   |
| Baseline or comparison                                   |                   |
| Does performance appear acceptable for the intended use? | Yes / No / Unsure |
| Known weaknesses                                         |                   |
| Additional validation needed                             |                   |

## 9. Plain-Language Interpretation

Summarise the output in plain language.

| Area                                          | Response |
| --------------------------------------------- | -------- |
| What the output appears to suggest            |          |
| What this may be useful for                   |          |
| What users should be careful about            |          |
| What should not be concluded from this output |          |

## 10. Limitations and Caveats

| Limitation or Caveat                 | Notes |
| ------------------------------------ | ----- |
| Data quality limitations             |       |
| Missing variables or missing context |       |
| Sample size concerns                 |       |
| Time period limitations              |       |
| Feature limitations                  |       |
| Model performance concerns           |       |
| Stability concerns                   |       |
| Interpretability concerns            |       |
| Operational limitations              |       |
| Other caveats                        |       |

## 11. Risks of Misuse

| Risk                                                 | Notes |
| ---------------------------------------------------- | ----- |
| Users may treat the output as a final decision       |       |
| Users may overinterpret correlations or patterns     |       |
| Users may ignore caveats or limitations              |       |
| Users may apply the output to the wrong population   |       |
| Users may use the output beyond the approved purpose |       |
| Users may assume the model is production-ready       |       |
| Other risk                                           |       |

## 12. Responsible Use Guidance

| Question                                              | Response          |
| ----------------------------------------------------- | ----------------- |
| Should this output be used for real decisions?        | Yes / No / Unsure |
| Should this remain sandbox?                           | Yes / No / Unsure |
| What caveat must accompany the output?                |                   |
| Who should validate the output before wider use?      |                   |
| What approval is needed before moving beyond sandbox? |                   |
| Is BIA review required?                               | Yes / No / Unsure |

## 13. Connection to Reporting or Dashboards

| Question                                                                     | Response          |
| ---------------------------------------------------------------------------- | ----------------- |
| Will the output be shown in a report or dashboard?                           | Yes / No / Unsure |
| Which report or dashboard may consume it?                                    |                   |
| Are caveats visible in the report?                                           | Yes / No / Unsure |
| Could report users misinterpret the output?                                  | Yes / No / Unsure |
| Is the output clearly marked as sandbox, experimental, or production-facing? | Yes / No / Unsure |

## 14. Review and Decision

| Decision Option                         | Select One |
| --------------------------------------- | ---------- |
| Keep as sandbox learning only           |            |
| Improve and rerun                       |            |
| Validate with subject matter expert     |            |
| Discuss as possible department use case |            |
| Escalate to BIA for review              |            |
| Not suitable for further use            |            |

## 15. Follow-Up Actions

| Action | Owner | Target Date | Status                           |
| ------ | ----- | ----------- | -------------------------------- |
|        |       |             | Not started / In progress / Done |
|        |       |             | Not started / In progress / Done |
|        |       |             | Not started / In progress / Done |

## 16. Final Notes

| Area                  | Response |
| --------------------- | -------- |
| Additional notes      |          |
| Recommended next step |          |
| Follow-up owner       |          |
| Follow-up date        |          |
