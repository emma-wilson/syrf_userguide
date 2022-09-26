---
title: Bibliographic Data Dictionary
parent: Data Export
has_children: false
nav_order: 2
layout: page
---

# Data Dictionary 

## Bibliographic Information

This section allows you to export the bibliographic information about the studies in your SyRF project.

[Bibliographic information example](./spreadsheet_templates/bibliographic_information_example.csv)

[Bibliographic information example - Systematic Search Import Compatibility format](./spreadsheet_templates/bibliographic_information_systematic-search-import-compatibility-format_example.csv)


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

A string input by the user at the time of upload, which can be used to refer to the library. (Endnote library name, etc)

\* Column is omitted if "SyRF systematic search import compatable format" is ticked.