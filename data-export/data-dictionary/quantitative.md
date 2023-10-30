---
title: Quantitative
parent: Data Dictionaries
grand_parent: Data Export
has_children: false
nav_order: 10
layout: page
---

# Quantitative Data Dictionary

The spreadsheet output from a quantitative data export will contain the quantitative data for the studies in your SyRF project.

Each row corresponds to a single timepoint and includes it's associated system and selected custom annotations. In addition, the associated IDs and labels for experiment, cohort, outcome, treatment, and diseaseModel entities are included.

## Data Export Example

[Quantitative data example](./spreadsheet_templates/quantitative_data_example.csv)

---

## Column Headings

#### [Bibliographic Data Columns](../data-dictionary/bibliographic.html)

If the `Show bibliographic data` option is selected in the SyRF interface then [Bibliographic Data Columns](../data-dictionary/bibliographic.html) are included in the export.

The `StudyId`, `DateTimeStudyAdded`, `SystematicSearchId` and `SystematicSearchName` columns will always be included regardless.

- ##### **Reconciled**

  Whether the annotation is part of a reconciliation session.

  _("TRUE"\|"FALSE")_

##### [Investigator Info Columns](../data-dictionary/investigator-info.html)

Investigator information columns will be included depending on which option is selected for the "**Choose level of blinding**" setting. [Click here for more details](../data-dictionary/investigator-info.html).

### Each selected annotation question

Every annotation question selected for the quantitative data export in the "[**select annotation questions to include in export**](/data-export/quantitative.html#select-annotation-questions-to-include-in-export)" is represented with a single column.

Each question header (below) contains the question text as defined by the project admins.

- ##### **\<QuestionText\>**

  Where \<QuestionText\> is the text of the selected annotation question.

  The value in each cell is the answer to that question that corresponds to the specific timepoint.

  _(String)_

### Standard Quantitative Data Columns

- ##### **DateTimeDataEntered**

  When the outcome data was entered by the reviewer in SyRF. In the ISO 8601 format, e.g. "2019-02-26 14:53:58"

  _(DateTime)_

- ##### **ExperimentId**

  The unique 32 digit alphanumeric identifier that SyRF uses to refer to this specific experiment entry.

  _(UUID)_

- ##### **ExperimentLabel**

  String input by the reviewer to label this experiment entry.

  _(String)_

- ##### **CohortId**

  The unique 32 digit alphanumeric identifier that SyRF uses to refer to this specific cohort entry.

  _(UUID)_

- ##### **CohortLabel**

  String input by the reviewer to label this cohort entry.

  _(String)_

- ##### **NumberOfAnimals**

  The number of animals defined in the cohort.

  _(Integer)_

- ##### **IsDiseaseModelControl**

  Whether the associated disease model(s) is a control. Multiple disease models associated with the cohort will have their control status separated with the "**;**" character.

  _("TRUE"\|"FALSE"\[;"TRUE"\|"FALSE"\]\*)_

- ##### **DiseaseModelId(s)**

  The unique 32 digit alphanumeric identifier that SyRF uses to refer to this specific disease model entry. Multiple disease models associated with the cohort will have their IDs separated with the "**;**" character.

  _(UUID\[;UUID\]\*)_

- ##### **DiseaseModelLabel(s)**

  String input by the reviewer to label this disease model. Multiple disease models associated with the cohort will have this value separated with the "**;**" character.

  _(String\[;String\]\*)_

- ##### **IsTreatmentControl**

  Whether the associated treatment(s) is a control. Multiple treatments associated with the cohort will have their control status separated with the "**;**" character.

  _("TRUE"\|"FALSE"\[;"TRUE"\|"FALSE"\]\*)_

- ##### **TreatmentId(s)**

  The unique 32 digit alphanumeric identifier that SyRF uses to refer to this specific treatment entry. Multiple treatments associated with the cohort will have their IDs separated with the "**;**" character.

  _(UUID\[;UUID\]\*)_

- ##### **TreatmentLabel(s)**

  String input by the reviewer to label this treatment entry. Multiple treatments associated with the cohort will have this value separated with the "**;**" character.

  _(String\[;String\]\*)_

- ##### **OutcomeId**

  The unique 32 digit alphanumeric identifier that SyRF uses to refer to this specific outcome assessment entry.

  _(UUID)_

- ##### **OutcomeLabel**

  String input by the reviewer to label this outcome assessment entry.

  _(String)_

- ##### **GreaterIsWorse**

  Whether the outcome assessment associated with this timepoint is a greater-is-worse outcome.

  _("TRUE"\|"FALSE")_

- ##### **TimeInMinutes**

  The timepoint in minutes.

  _(Integer)_

- ##### **OutcomeAverage**

  The average value of the outcome assessment associated with this timepoint.

  _(Number)_

- ##### **OutcomeAverageType**

  The type of average used to calculate the OutcomeAverage value.

  _("mean"\|"median"\|"mode")_

- ##### **OutcomeUnit**

  The unit of the outcome assessment associated with this timepoint.

  _(String)_

- ##### **OutcomeError**

  The error value of the outcome assessment associated with this timepoint.

  _(Number)_

- ##### **OutcomeErrorType**

  The type of error used to calculate the OutcomeError value.

  _("SD"\|"SEM"\|"IQR")_
