---
alias:
metadata: 02
author: AUGST-MERELLE Alexandra
type: project
status: ready
keywords: learn, sciences
creation: 2021-06-27
modification: 2021-06-27
---
%%
keywords: englobants
%%
 | 
------------ | ------------
MOC | [[SCIENCES]]
Project |
Template | [[Archive/Notes permanentes]]
Source | [[AUGST-MERELLE Alexandra]]
# Mathématiques (Projet)
## Pages principales
```dataview
list file.path
from "Archive/Notes permanentes"
AND [[Mathématiques (Projet)]]
where file.name="_index"
sort type, file.name
```
## Projets
```dataview
list
where type="project"
where contains(keywords,"mathématiques")
sort type, file.name
```
## Notes littéraires
```dataview
table type
from "Archive/Notes littéraires"
AND [[Mathématiques (Projet)]]
sort type, file.name
```
## Notes permanentes
```dataview
list
from "Archive/Notes permanentes"
AND [[Mathématiques (Projet)]]
where status!="draft"
where file.name!="_index"
sort type, file.name
```
## Notes en draft
```dataview
list
from "Archive/Notes permanentes"
AND [[Mathématiques (Projet)]]
where status="draft"
sort type, file.name
```