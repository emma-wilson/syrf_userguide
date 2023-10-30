---
title: Screening (Wide Format)
parent: Data Dictionaries
grand_parent: Data Export
has_children: false
nav_order: 3
layout: page
---

# Screening (Wide Format) Data Dictionary

The spreadsheet output from a wide format screening data export will contain the screening decisions against the inclusion/exclusion criteria specific to the project, as input by the team conducting the systematic review.

In wide format each row corresponds to a single study and contains the screening decisions of all reviewers.

## Data Export Example

[Screening export example (wide format)](./spreadsheet_templates/screening_data_unblinded_wide-format_example.csv)

---

## Column Headings

#### [Bibliographic Data Columns](../bibliographic.html)

If the `Show bibliographic data` option is selected in the SyRF interface then [bibliographic data columns](../bibliographic.html) are included in the export.

The `StudyId`, `DateTimeStudyAdded`, `SystematicSearchId` and `SystematicSearchName` columns will always be included regardless.

#### [Investigator Info Columns](../data-dictionary/investigator-info.html)

Investigator information columns will be included depending on which option is selected for the "**Choose level of blinding**" setting. [Click here for more details](../data-dictionary/investigator-info.html).

- ##### **DateTimeOfScreenings**

  When the study was screened by the reviewers in SyRF. Multiple screening dates will be separated with the "**;**" character. In the ISO 8601 format, e.g. "2019-02-26 14:53:58;2019-03-14 16:43:24"
  
  _(DateTime\[;DateTime\]\*)_

- ##### **ScreeningDecisions**

  Did the investigators include or exclude the study? Multiple screening decisions will be separated with the "**;**" character.
  
  _("Included"\|"Excluded"\[;"Included"\|"Excluded"\]*)_

- ##### **ScreeningStatus**
  Was the study ultimately included or excluded or has it not yet been sufficiently screened?
  
  _("Included"\|"Excluded"\|"InsufficientlyScreened")_