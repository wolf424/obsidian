---
alias: projet, projets
metadata: 02
author: AUGST-MERELLE Alexandra
type: index
status: ready
keywords: 
creation: 2021-06-27
modification: 2021-06-27
---
 | 
------------ | ------------
MOC | [[MISC]]
Project |
Template | [[Archive/Notes permanentes]]
Source | [[AUGST-MERELLE Alexandra]]
# Index des thématiques
## Projets en cours
```dataview
list
where type="project"
where contains(keywords,"encours")
sort type, file.name
```
## Projets racine
```dataview
list
where type="project"
where contains(keywords,"main")
sort type, file.name
```
## Index
```dataview
list
from "Archive/Notes permanentes"
where type="index"
where status!="draft"
sort type, file.name
```
### Index en draft
```dataview
table file.path, type, keywords
from "Archive/Notes permanentes"
where type="index"
where status="draft"
sort type, file.name
```
## Notes en draft
### Notes littéraires
```dataview
list
from "Archive/Notes littéraires"
where contains(keywords,"main")
sort type, file.name
```
### Notes permanentes
```dataview
list
from "Archive/Notes permanentes"
where status="draft"
where type!="index"
sort type, file.name
```
## Maintenance
[[_admn]]