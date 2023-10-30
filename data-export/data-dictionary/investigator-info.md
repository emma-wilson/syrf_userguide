---
title: Investigator Information
parent: Data Dictionaries
grand_parent: Data Export
has_children: false
nav_order: 1
layout: page
---

# Investigator Information Columns Dictionary

Investigator information columns will be included depending on which option is selected for the "**Choose level of blinding**" setting.

## Column Headings

### Show investigator name and unique ID - _not blinded_

- ##### **InvestigatorId(s)**

  A unique 32 digit alphanumeric identifier which SyRF uses to refer to the specific investigator. Mulitiple IDs will be seperated with the "**;**" character.

  _(UUID\[;UUID\]\*)_

- ##### **InvestigatorName(s)**

  The full name(s) of the investigator(s). Mulitiple names will be seperated with the "**;**" character.

  _(String\[;String\]\*)_

---

### Show only investigator unique ID - _partially blinded_

- ##### **InvestigatorId(s)**

  A unique 32 digit alphanumeric identifier which SyRF uses to refer to the specific investigator. Mulitiple IDs will be seperated with the "**;**" character.

  _(UUID\[;UUID\]\*)_
