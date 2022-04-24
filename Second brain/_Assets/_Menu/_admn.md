# Menu - Administration de la base
## Status invalide
```dataview
table file.path, status where !(
(status="toread") OR
(status="draft") OR
(status="ready"))
where !contains(file.path,"_Template")
```
## Type invalide ou none
```dataview
table file.path, type
where !(
(type = "admin") OR
(type = "article") OR
(type = "audio") OR
(type = "citation") OR
(type = "concept") OR
(type = "cours") OR
(type = "exemple") OR
(type = "howto") OR
(type = "idée") OR
(type = "index") OR
(type = "moc") OR
(type = "outil") OR
(type = "people") OR
(type = "project") OR
(type = "sandbox") OR
(type = "template") OR
(type = "texte") OR
(type = "todolist") OR
(type = "video"))
where !contains(file.path,"_Template")
```
## Fiches sans [[MOC (index)|map of content]]
```dataview
table file.path from [[MOC/NONE]]
where !contains(file.path,"_Template")
```
## metadata invalide
```dataview
table file.path, metadata where metadata < 01
```
## Fiches sans Projet
```dataview
table file.path from [[_Projects/None]]
where !contains(file.path,"_Template")
```
