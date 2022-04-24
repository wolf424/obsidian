---
alias:
metadata: 02
author: AUGST-MERELLE Alexandra
type: project
status: ready
keywords: main,diy
creation: 2021-06-27
modification: 2021-06-27
---
%%
keywords: englobants
%%
 | 
------------ | ------------
MOC | [[EUKARYA]] [[DIY]] [[DOMOTIQUE]]
Project |
Template | [[Archive/Notes permanentes]]
Source | [[AUGST-MERELLE Alexandra]]
# Domotique (Projet)
## TODO
```dataview
list
from "_Projects"
where contains(keywords,"domotique")
where type="todolist"
sort type, file.name
```

## Pages principales
```dataview
list file.path
from "Archive/Notes permanentes"
where contains(keywords,"domotique")
where file.name="_index"
sort type, file.name
```
## Projets
```dataview
list
where type="project"
where contains(keywords,"domotique")
sort type, file.name
```
## Notes littéraires
```dataview
table type
from "Archive/Notes littéraires"
AND [[_Projects/Domotique (Projet)]]
sort type, file.name
```
## Notes permanentes
```dataview
table type
from "Archive/Notes permanentes"
AND [[_Projects/Domotique (Projet)]]
sort type, file.name
```
## Notes en draft
```dataview
table type, keywords
from "Archive/Notes permanentes"
AND [[_Projects/Domotique (Projet)]]
where status="draft"
sort type, file.name
```