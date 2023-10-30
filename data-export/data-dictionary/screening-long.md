---
title: Screening (Long Format)
parent: Data Dictionaries
grand_parent: Data Export
has_children: false
nav_order: 3
layout: page
---

# Screening (Long Format) Data Dictionary

The spreadsheet output from a long format screening data export will contain the screening decisions against the inclusion/exclusion criteria specific to the project, as input by the team conducting the systematic review.

In long format each row corresponds to a single screening decision of a single study by a single reviewer. A complete review of a single study will consist of many screening rows.

## Data Export Example

[Screening export example (long format)](./spreadsheet_templates/screening_data_unblinded_long-format_example.csv)

---

## Column Headings

#### [Bibliographic Data Columns](../data-dictionary/bibliographic.html)

If the `Show bibliographic data` option is selected in the SyRF interface then [Bibliographic Data Columns](../data-dictionary/bibliographic.html) are included in the export.

The `StudyId`, `DateTimeStudyAdded`, `SystematicSearchId` and `SystematicSearchName` columns will always be included regardless.

#### [Investigator Info Columns](../data-dictionary/investigator-info.html)

Investigator information columns will be included depending on which option is selected for the "**Choose level of blinding**" setting. [Click here for more details](../data-dictionary/investigator-info.html).

- ##### **DateTimeOfScreening**

  When the study was screened by the reviewer in SyRF. In the ISO 8601 format, e.g. "2019-02-26 14:53:58"

  _(DateTime)_

- ##### **ScreeningDecision**

  Did the investigator include or exclude the study?
  
  _("Included"\|"Excluded")_

- ##### **ScreeningStatus**
  Was the study ultimately included or excluded or has it not yet been sufficiently screened?
  
  _("Included"\|"Excluded"\|"InsufficientlyScreened")_
