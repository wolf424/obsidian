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
MOC | [[DEV]]
Project |
Template | [[Archive/Notes permanentes]]
Source | [[AUGST-MERELLE Alexandra]]
# Dev (Projet)
## TODO
```dataview
list
from "_Projects"
where contains(keywords,"dev")
where type="todolist"
sort type, file.name
```

## Pages principales
```dataview
list file.path
from "Archive/Notes permanentes"
AND [[Dev (Projet)]]
where type="index"
sort type, file.name
```
## Projets
```dataview
list
where type="project"
where contains(keywords,"dev")
sort type, file.name
```
## Notes littéraires
```dataview
table type
from "Archive/Notes littéraires"
AND [[Dev (Projet)]]
sort type, file.name
```
## Notes permanentes
```dataview
table file.path, type, keywords
from "Archive/Notes permanentes"
AND [[Dev (Projet)]]
where status!="draft"
where file.name!="_index"
sort type, file.name
```
## Notes en draft
```dataview
table file.path, type, keywords
from "Archive/Notes permanentes"
AND [[Dev (Projet)]]
where status="draft"
sort type, file.name
```