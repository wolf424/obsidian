---
alias:
metadata: 02
author: AUGST-MERELLE Alexandra
type: project
status: ready
keywords: diy
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
# Electronique (Projet)
## TODO
```dataview
list
from "_Projects"
where contains(keywords,"électronique")
where type="todolist"
sort type, file.name
```
## Pages principales
```dataview
list file.path
from "Archive/Notes permanentes"
AND [[Electronique (Projet)]]
where type="index"
sort type, file.name
```
## Projets
```dataview
list
where type="project"
where contains(keywords,"électronique")
sort type, file.name
```
## Notes littéraires
```dataview
table type
from "Archive/Notes littéraires"
AND [[Electronique (Projet)]]
sort type, file.name
```
## Notes permanentes
```dataview
table file.path, type, keywords
from "Archive/Notes permanentes"
AND [[Electronique (Projet)]]
where status!="draft"
where file.name!="_index"
sort type, file.name
```
## Notes en draft
```dataview
table file.path, type, keywords
from "Archive/Notes permanentes"
AND [[Electronique (Projet)]]
where status="draft"
sort type, file.name
```