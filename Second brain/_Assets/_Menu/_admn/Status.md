---
alias:
metadata: 01
author: AUGST-MERELLE Alexandra
type: article
status: ready
creation: 2021-06-27
modification: 2021-06-27
---
 | 
------------ | ------------
MOC | [[ADMIN]]
Project |
Template | [[Archive/Notes permanentes]]
Source | [[AUGST-MERELLE Alexandra]]
# Status [[Obsidian]]
- ***Si modification de cette liste, mettre à jour les fiches suivantes :***
  *[[_admn]]*
  
Type | Descriptif|Index
--- | --- | ---
toread | document à lire (en vue d'une éventuelle prise de notes)
draft | brouillon de document
ready | document prêt avec des metadata à jour
## Fiches par status
### toread
```dataview
table file.path where status="toread" sort file.name
```
### draft
```dataview
table file.path where status="draft" sort file.name
where !contains(file.path,"_Template")
```
### ready
```dataview
table file.path where status="ready" sort file.name
```
