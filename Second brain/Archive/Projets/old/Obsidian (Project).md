---
alias:
metadata: 02
author: AUGST-MERELLE Alexandra
type: project
status: ready
keywords: learn
creation: 2021-06-27
modification: 2021-06-27
---
%%
keywords: englobants
%%
 | 
------------ | ------------
MOC | [[DOC]]
Project |
Template | [[Archive/Notes permanentes]]
Source | [[AUGST-MERELLE Alexandra]]
# Apprendre obsidian (Projet)
## Pages principales
```dataview
list file.path
from "Archive/Notes permanentes"
AND [[Obsidian (Project)]]
where file.name="_index"
sort type, file.name
```
## Projets
```dataview
list
where type="project"
where contains(keywords,"obsidian")
sort type, file.name
```
## Notes littéraires
```dataview
table type
from "Archive/Notes littéraires"
AND [[Obsidian (Project)]]
sort type, file.name
```
## Notes permanentes
```dataview
list
from "Archive/Notes permanentes"
AND [[Obsidian (Project)]]
where status!="draft"
where file.name!="_index"
sort type, file.name
```
## Notes en draft
```dataview
list
from "Archive/Notes permanentes"
AND [[Obsidian (Project)]]
where status="draft"
sort type, file.name
```