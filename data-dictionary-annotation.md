---
title: Annotation Data Dictionary
parent: Data Export
has_children: false
nav_order: 6
layout: page
---

# Data Dictionary 

## Annotation

The spreadsheets output from the annotation section will contain questions specific to the systematic review being performed, as input by the team conducting the systematic review. 

[Long-format example](./spreadsheet_templates/annotation_data-extraction-stage_study-level_long-format_example.csv)

[Wide-format example](./spreadsheet_templates/annotation_data-extraction-stage_study-level_wide-format_example.csv)

_These examples contain the same information and are questions from a review conducted by CAMARADES Berlin. The questions in your spreadsheet will depend on the specific questions in your systematic review._

### Long-format

Each row corresponds to a single question from a single study. Each child-question will be in a separate row. A complete review of a single study will consist of many rows. 

##### AnnotationId

A unique 32 digit alphanumeric identifier which SyRF uses to refer to this specific annotation.

##### Question

The text of the question as input by the researcher conducting the review.

##### QuestionId

A unique 32 digit alphanumeric identifier which SyRF uses to refer to this specific question.

##### Answer

The answer to the question as input by the reviewer.

##### AnswerType

The data type of the answer (string/boolean/integer). 

##### Reconciled
...

##### IsRootQuestion

True/False whether this is a root-question or a child-question

##### ParentQuestionId

If question is a not a root-question, what is the QuestionId of the root-question.

##### ChildQuestionIds

If question has child-questions, what are the QuestionIds of the child-questions. 

##### HasChildQuestions

True/False whether this question has child-questions.

##### ParentAnnotationId

What is the AnnotationId of the annotation which contains the parent-question of this question?

##### ChildAnnotationIds

What is the AnnotationId of the annotation which contains the child-question of this question?

##### HasChildAnnotations

True/False whether this question has child-annotations.

### Wide-format

A single row corresponds to a single study, with each question requiring three columns, requiring double column-headings, with the upper column-heading containing:

1. The text of the question, as input by the researcher conducting the systematic review, and

2. The QuestionId of the question.

For example: 

    Is the study excluded_017899ae-9de4-47ce-8ee0-f097a9ab8149

The lower column-headings are:

##### AnnotationId

A unique 32 digit alphanumeric identifier which SyRF uses to refer to this specific annotation.

##### Answer

The answer to the question as input by the reviewer.

##### Comments

Any comments added by the reviewer pertaining to the question.


**Each level after Study level has additional standard columns**

#### Disease Model Induction Level

##### DiseaseModelId

A unique 32 digit alphanumeric identifier which SyRF uses to refer to this specific disease model entry.

##### DiseaseModelLabel

String input by the reviewer to label this disease model.

#### Treatment Level

##### TreatmentId

A unique 32 digit alphanumeric identifier which SyRF uses to refer to this specific treatment entry.

##### TreatmentLabel

String input by the reviewer to label this treatment entry.

#### Outcome Assessment Level

##### OutcomeId	

A unique 32 digit alphanumeric identifier which SyRF uses to refer to this specific outcome assessment entry.

##### OutcomeLabel

String input by the reviewer to label this outcome assessment entry.

#### Cohort Level

##### CohortId

A unique 32 digit alphanumeric identifier which SyRF uses to refer to this specific cohort entry.

##### CohortLabel

String input by the reviewer to label this cohort entry.

#### Experiment Level

##### ExperimentId

A unique 32 digit alphanumeric identifier which SyRF uses to refer to this specific experiment entry.

##### ExperimentLabel

String input by the reviewer to label this experiment entry.

