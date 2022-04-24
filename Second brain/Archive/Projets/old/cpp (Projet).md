
---
alias:
metadata: 02
author: AUGST-MERELLE Alexandra
type: project
status: ready
keywords: dev
creation: 2021-06-27
modification: 2021-06-27
---
%%
keywords: themes du niveau supérieur
%%
 | 
------------ | ------------
MOC | [[DEV]]
Project |
Template | [[Archive/Notes permanentes]]
Source | [[AUGST-MERELLE Alexandra]]
# cpp (Projet)
## Pages principales
```dataview
list file.path
from "Archive/Notes permanentes"
AND [[cpp (Projet)]]
where type="index"
sort type, file.name
```
## Projets
```dataview
list
where type="project"
where contains(keywords,"cpp")
sort type, file.name
```
## Notes littéraires
```dataview
table type
from "Archive/Notes littéraires"
AND [[cpp (Projet)]]
sort type, file.name
```
## Notes permanentes
```dataview
table file.path, type, keywords
from "Archive/Notes permanentes"
AND [[cpp (Projet)]]
where status!="draft"
where file.name!="_index"
sort type, file.name
```
## Notes en draft
```dataview
table file.path, type, keywords
from "Archive/Notes permanentes"
AND [[cpp (Projet)]]
where status="draft"
sort type, file.name
```