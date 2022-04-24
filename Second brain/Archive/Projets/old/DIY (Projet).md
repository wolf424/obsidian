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
keywords: englobants
%%
 | 
------------ | ------------
MOC | [[DIY]]
Project |
Template | [[Archive/Notes permanentes]]
Source | [[AUGST-MERELLE Alexandra]]
# DIY (Projet)
## TODO
```dataview
list
from "_Projects"
where contains(keywords,"diy")
where type="todolist"
sort type, file.name
```
## Pages principales
```dataview
list file.path
from "Archive/Notes permanentes"
where contains(keywords,"diy")
where file.name="_index"
sort type, file.name
```
## Projets
```dataview
list
where type="project"
where contains(keywords,"diy")
sort type, file.name
```
## Notes littéraires
```dataview
table type
from "Archive/Notes littéraires"
AND [[_Projects/DIY (Projet)]]
sort type, file.name
```
## Notes permanentes
```dataview
table type
from "Archive/Notes permanentes"
AND [[_Projects/DIY (Projet)]]
sort type, file.name
```
## Notes en draft
```dataview
table type, keywords
from "Archive/Notes permanentes"
AND [[_Projects/DIY (Projet)]]
where status="draft"
sort type, file.name
```