---
title: Annotation (Long Format)
parent: Data Dictionaries
grand_parent: Data Export
has_children: false
nav_order: 6
layout: page
---

# Annotation (Long Format) Data Dictionary

The spreadsheet output from a long format annotation data export will contain questions specific to the project, as input by the team conducting the systematic review.

In long format each row corresponds to a single annotation of a single study by a single reviewer. Each child-question will be in a separate row. A complete review of a single study will consist of many annotation rows.

## Data Export Example

[Long-format example](./spreadsheet_templates/annotation_data-extraction-stage_study-level_long-format_example.csv)

_This examples contains questions from a review conducted by CAMARADES Berlin. The questions in your spreadsheet will depend on the specific questions in your systematic review._

---

## Column Headings

#### [Bibliographic Data Columns](../bibliographic.html)

If the `Show bibliographic data` option is selected in the SyRF interface then [bibliographic data columns](../bibliographic.html) are included in the export.

The `StudyId`, `DateTimeStudyAdded`, `SystematicSearchId` and `SystematicSearchName` columns will always be included regardless.

- ##### **Reconciled**
  Whether the annotation is part of a reconciliation session.

  _("TRUE"\|"FALSE")_

#### [Investigator Info Columns](../data-dictionary/investigator-info.html)

Investigator information columns will be included depending on which option is selected for the "**Choose level of blinding**" setting. [Click here for more details](../data-dictionary/investigator-info.html).

- ##### **DateTimeAnnotated**
  When the annotation was submitted by the reviewer in SyRF. In the ISO 8601 format, e.g. "2019-02-26 14:53:58"

  _(DateTime)_

- ##### **AnnotationId**

  The unique 32 digit alphanumeric identifier that SyRF uses to refer to this specific annotation.

  _(UUID)_

- ##### **Question**

  The text of the question as input by the researcher conducting the review.

  _(String)_

- ##### **QuestionId**

  The unique 32 digit alphanumeric identifier that SyRF uses to refer to this specific question.

  _(UUID)_

- ##### **Answer**

  The answer to the question as input by the reviewer.

  _(String)_

- ##### **Comments**

    Any comments added by the reviewer pertaining to the question.

  _(String)_

- ##### **AnswerType**

  The data type of the answer.

  _("string"\|"boolean"\|"integer"\|"stringArray"\|"integerArray")_

- ##### **IsRootQuestion**

  Whether this is a root-question or a child-question.

  _("TRUE"\|"FALSE")_

- ##### **ParentQuestionId**

  If question is a not a root-question, what is the QuestionId of the root-question.

  _(UUID)_

- ##### **ChildQuestionIds**

  If question has child-questions, what are the QuestionIds of the child-questions.

  _(UUID\[;UUID\]\*)_

- ##### **HasChildQuestions**

  Whether this question has child-questions.

  _("TRUE"\|"FALSE")_

- ##### **ParentAnnotationId**

  What is the AnnotationId of the annotation which contains the parent-question of this question?

  _(UUID)_

- ##### **ChildAnnotationIds**

  What is the AnnotationId of the annotation which contains the child-question of this question?

  _(UUID\[;UUID\]\*)_

- ##### **HasChildAnnotations**
  Whether this question has child-annotations.

  _("TRUE"\|"FALSE")_
