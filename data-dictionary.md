---
title: Data Dictionary
parent: Data Export
has_children: false
nav_order: 0
layout: page
---

# Data Dictionary 

## Bibliographic Information

This section allows you to export the bibliographic information about the studies in your SyRF project.

[Bibliographic information example](https://help.syrf.org.uk/spreadsheet_templates/bibliographic_information_example.csv)

[Bibliographic information example - Systematic Search Import Compatibility format](https://help.syrf.org.uk/spreadsheet_templates/bibliographic_information_systematic-search-import-compatibility-format_example.csv)


### Column Headings

##### StudyId*

A unique 32 digit alphanumeric identifier which SyRF uses to refer to the specific study. 

##### Title 

Title of the study

##### Authors  

List of authors of study separated by a semi-colon.

##### PublicationName 

Name of the journal in which the study was published. 

##### AlternateName

Alternate name of the journal in which the study was published. (Former name, abbreviation, etc)

##### Abstract 

Full text of the study abstract.

##### Url 

Link to full-text PDF 

##### AuthorAddress

Contact information for primary author. (institutional affiliation, e-mail address)

##### Year

Year study was published. 

##### Doi	

Unique Digital Object Identifier (DOI) assigned to study.

##### ReferenceType	

Type of reference (Journal article / book chapter / conference proceedings)

##### Keywords

Keywords associated with study. 

##### PdfRelativePath

Path to PDF of study from root directory.

##### DateTimeCreated*

Date and time study was added in format "10/02/2019 14:53:58"

##### SystematicSearchId*

A unique 32 digit alphanumeric identifier which SyRF uses to refer to the specific search.

##### SystematicSearchName*

Unique search name. 

##### CustomId

...

\* Column is omitted if "SyRF systematic search import compatable format" is ticked.




## Screening Data

[Long-format example](https://help.syrf.org.uk/spreadsheet_templates/screening_data_unblinded_long-format_example.csv)

[Wide-format example](https://help.syrf.org.uk/spreadsheet_templates/screening_data_unblinded_wide-format_example.csv)

##### Reconciled

<!---True / False indicating whether discrepancies between reviewers have been reconciled. --->

...

##### InvestigatorId	

A unique 32 digit alphanumeric identifier which SyRF uses to refer to the specific investigator.

##### InvestigatorName	

The full name of the investigator.

##### ScreeningDecision	

Did the investigator include or exclude the study?

##### ScreeningStatus

Was the study ultimately included or excluded? Two reviewers must agree for a study to be included or excluded. 




## Annotation

The spreadsheets output from the annotation section will contain questions specific to the systematic review being performed, as input by the team conducting the systematic review. 

[Long-format example](https://help.syrf.org.uk/spreadsheet_templates/annotation_data-extraction-stage_study-level_long-format_example.csv)

[Wide-format example](https://help.syrf.org.uk/spreadsheet_templates/annotation_data-extraction-stage_study-level_wide-format_example.csv)

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

