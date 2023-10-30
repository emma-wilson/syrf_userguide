---
title: Annotation (Wide Format)
parent: Data Dictionaries
grand_parent: Data Export
has_children: false
nav_order: 7
layout: page
---

# Annotation (Wide Format) Data Dictionary

The spreadsheet output from a wide format annotation data export will contain the annotation questions and answers specific to the systematic review being performed, as input by the team conducting the systematic review.

## Data Export Example

[Wide-format example](./spreadsheet_templates/annotation_data-extraction-stage_study-level_wide-format_example.csv)

_This examples contains questions from a review conducted by CAMARADES Berlin. The questions in your spreadsheet will depend on the specific questions in your systematic review._

---

## Column Headings

#### [Bibliographic Data Columns (click to view)](../bibliographic.html)

If the `Show bibliographic data` option is selected in the SyRF interface then [bibliographic data columns](../bibliographic.html) are included in the export.

The `StudyId`, `DateTimeStudyAdded`, `SystematicSearchId` and `SystematicSearchName` columns will always be included regardless.

- ##### **Reconciled**

  Whether the annotation is part of a reconciliation session.

  _("TRUE"\|"FALSE")_

#### [Investigator Info Columns (click to view)](../data-dictionary/investigator-info.html)

Investigator information columns will be included depending on which option is selected for the "**Choose level of blinding**" setting. [Click here for more details](../data-dictionary/investigator-info.html).

### Each annotation level after Study level has additional standard columns

#### Disease Model Induction Level

- ##### **DiseaseModelId**

  The unique 32 digit alphanumeric identifier that SyRF uses to refer to this specific disease model entry.

  _(UUID)_

- ##### **DiseaseModelLabel**
  String input by the reviewer to label this disease model.

#### Treatment Level

- ##### **TreatmentId**

  The unique 32 digit alphanumeric identifier that SyRF uses to refer to this specific treatment entry.

  _(UUID)_

- ##### **TreatmentLabel**

  String input by the reviewer to label this treatment entry.

  _(String)_

#### Outcome Assessment Level

- ##### **OutcomeId**

  The unique 32 digit alphanumeric identifier that SyRF uses to refer to this specific outcome assessment entry.

  _(UUID)_

- ##### **OutcomeLabel**

  String input by the reviewer to label this outcome assessment entry.

  _(String)_

#### Cohort Level

- ##### **CohortId**

  The unique 32 digit alphanumeric identifier that SyRF uses to refer to this specific cohort entry.

  _(UUID)_

- ##### **CohortLabel**

  String input by the reviewer to label this cohort entry.

  _(String)_

#### Experiment Level

- ##### **ExperimentId**

  The unique 32 digit alphanumeric identifier that SyRF uses to refer to this specific experiment entry.

  _(UUID)_

- ##### **ExperimentLabel**

  String input by the reviewer to label this experiment entry.

  _(String)_

### Each annotation question

Each annotation question is represented with the four columns defined below.
These column headers also contain

1. The question text
2. The question ID (except when the `Single header row simple` option is selected for the [**Choose wide format header type**](../annotation.html#choose-wide-format-header-type-only-available-in-wide-format) property)

**N.b.** The format of the headers for each of these four columns is determined by the options selected for the property [**Choose wide format header type**](../annotation.html#choose-wide-format-header-type-only-available-in-wide-format) in the annotation data export settings (wide format). [Click here for more detail](../annotation.html#choose-wide-format-header-type-only-available-in-wide-format).

- ##### **AnnotationId**

  The unique 32 digit alphanumeric identifier that SyRF uses to refer to this specific annotation.

  _(UUID)_

- ##### **Answer**

  The answer to the question as input by the reviewer.

  _(String)_

- ##### **Comments**

  Any comments added by the reviewer pertaining to the question.

  _(String)_

- ##### **DateTimeAnnotated**

  The Date and time of the annotation In the ISO 8601 format, e.g. "2019-02-26 14:53:58"

  _(DateTime)_.
