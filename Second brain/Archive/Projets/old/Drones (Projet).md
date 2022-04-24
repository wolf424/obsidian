---
alias:
metadata: 02
author: AUGST-MERELLE Alexandra
type: project
status: ready
keywords: main drones
creation: 2021-08-19
modification: 2021-08-19
---
%%
keywords: englobants
%%
 | 
------------ | ------------
MOC | [[EUKARYA]] [[DRONES]]
Project |
Template | [[Archive/Notes permanentes]]
Source | [[AUGST-MERELLE Alexandra]]
# Drones (Projet)
## TODO
```dataview
list
from "_Projects"
where contains(keywords,"drones")
where type="todolist"
sort type, file.name
```

## Pages principales
```dataview
list file.path
from "Archive/Notes permanentes"
where contains(keywords,"drones")
where file.name="_index"
sort type, file.name
```
## Projets
```dataview
list
where type="project"
where contains(keywords,"drones")
sort type, file.name
```
## Notes littéraires
```dataview
table type
from "Archive/Notes littéraires"
AND [[_Projects/Drones (Projet)]]
sort type, file.name
```
## Notes permanentes
```dataview
table type
from "Archive/Notes permanentes"
AND [[_Projects/Drones (Projet)]]
sort type, file.name
```
## Notes en draft
```dataview
table type, keywords
from "Archive/Notes permanentes"
AND [[_Projects/Drones (Projet)]]
where status="draft"
sort type, file.name
```