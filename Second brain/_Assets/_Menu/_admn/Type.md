---
alias: types
metadata: 01
author: AUGST-MERELLE Alexandra
type: article
status: ready
creation: 2021-06-27
modification: 2021-06-27
---
 | 
------------ | ------------
MOC | [[ADMIN]]
Project |
Template | [[Archive/Notes permanentes]]
Source | [[AUGST-MERELLE Alexandra]]
# Types [[Obsidian]]
***Si modification de cette liste, mettre à jour les fiches suivantes :***
  - *[[_admn]]*
  - *[[Archive/Notes permanentes]]*
  - *[[_Templates/litt]]*
  - *[[_header]]*

Type | Descriptif|Index
--- | --- | ---
none | Valeur par défaut : à remplacer
admin | Administration de la base | [[_admn]]
article | article sur un sujet
audio | lien vers un support audio
citation | citation d'un auteur ou d'une source
concept | définition d'un concept
cours | cours ou formation
exemple | Un exemple pour illustrer
howto | procédure ou manuel
idée | Une [[idée]] qui vient
index | Un index de projet
moc | Map of content | [[MOC (index)]]
outil | Un outil pratique
people | Personne physique ou morale | [[People (index)]]
project | Projet | [[Projets (index)]]
sandbox | Bac à sable | [[dataview]]
template | modèle de fiche
texte | lien vers un support texte (pdf, odt, doc)
todolist | tâches à réaliser
video | lien vers un support video
## Fiches par type
### none
```dataview
table file.path where type="none" sort file.name
```
### admin
```dataview
list where type="admin" sort file.name
```
### article
```dataview
list where type="article" sort file.name
```
### audio
```dataview
list where type="audio" sort file.name
```
### citation
```dataview
list where type="citation" sort file.name
```
### concept
```dataview
list where type="concept" sort file.name
```
### cours
```dataview
list where type="cours" sort file.name
```
### exemple
```dataview
list where type="exemple" sort file.name
```
### howto
```dataview
list where type="howto" sort file.name
```
### idée
```dataview
list where type="idée" sort file.name
```
### index
```dataview
table file.path
where type="index"
sort file.name
```
### moc
```dataview
list where type="moc" sort file.name
```
### outil
```dataview
list where type="outil" sort file.name
```
### people
```dataview
list where type="people" sort file.name
```
### project
```dataview
list where type="project" sort file.name
```
### sandbox
```dataview
list where type="sandbox" sort file.name
```
### template
```dataview
list where type="template" sort file.name
```
### text
```dataview
list where type="text" sort file.name
```
### todolist
```dataview
list where type="todolist" sort file.name
```
### video
```dataview
list where type="video" sort file.name
```