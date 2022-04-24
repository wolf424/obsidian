---
alias:
metadata: 02
author: AUGST-MERELLE Alexandra
type: project
status: ready
keywords: main
creation: 2021-06-27
modification: 2021-06-27
---
%%
keywords: themes du niveau supérieur
%%
 | 
------------ | ------------
MOC | [[MISC]]
Project |
Template | [[Archive/Notes permanentes]]
Source | [[AUGST-MERELLE Alexandra]]
# Eukarya (Projet)
## Pages principales
```dataview
list file.path
from "Archive/Notes permanentes"
AND [[Eukarya (Projet)]]
where type="index"
sort type, file.name
```
## Projets
```dataview
list
where type="project"
where contains(keywords,"eukarya")
sort type, file.name
```
## Notes littéraires
```dataview
table type
from "Archive/Notes littéraires"
AND [[Eukarya (Projet)]]
sort type, file.name
```
## Notes permanentes
```dataview
table file.path, type, keywords
from "Archive/Notes permanentes"
AND [[Eukarya (Projet)]]
where status!="draft"
where file.name!="_index"
sort type, file.name
```
## Notes en draft
```dataview
table file.path, type, keywords
from "Archive/Notes permanentes"
AND [[Eukarya (Projet)]]
where status="draft"
sort type, file.name
```