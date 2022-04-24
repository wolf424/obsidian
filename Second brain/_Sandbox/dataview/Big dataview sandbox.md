---
metadata: 01
type: sandbox
status: ready
---
 |
------------ | ------------
MOC | [[MISC]]
Project |
Template | [[Archive/Notes permanentes]]
Source | [[AUGST-MERELLE Alexandra]]

# Gros bac à sable [[Big dataview sandbox|dataview]]
## Listes
#### Notes du dossier Archive, alphabétiquement

%%
dataview:
- Lister depuis le dossier /Archive
- Tri alphabétique sur le nom de fichier
%%

```dataview
list from "Archive"
sort type, file.name
```
#### Notes avec le tag #article

Avec list from
%%
dataview:
- Lister depuis #article
%%

```dataview
list from #article 
```
Avec ̀list where contains

%%
dataview:
- Tout lister
- Ne retenir que file.tags contenant #article
%%

```dataview
list  where contains(file.tags,"#article")
```
#### Notes sans tag
%%
dataview:
- Tout lister
- Ne retenir que file.tags de longueur nulle
%%
```dataview
list  where length(file.tags) < 1
```
#### Notes contenant un lien vers [[DROIT]]
%%
dataview:
- Contenant un lien vers [[DROIT]]
%%

```dataview
list from [[Droit]] 
```
## Tables
### Avec tri
Par date de modification sur les notes liées à [[DROIT]]
%%
dataview:
- Table avec les champs
  - file.ctime
  - file.mtime renommé en "Modif"
- Contenant un lien vers [[DROIT]]
- Tri descendant par date de modification
%%

```dataview
table file.ctime, file.mtime as "Modif" 
from [[Droit]]
sort file.mtime desc
```

### Avec filtre
#### Les plus gros fichiers
Par date de modification sur les notes liées à [[DROIT]]
%%
dataview:
- Table avec les champs
  - file.size
- Ne retenir que les notes de taille > 1000 octets
- Tri descendant par taille
%%

```dataview
table file.size
where file.size>1000
sort file.size desc
```

#### Les fichiers modifiées les 2 derniers jours
%%
dataview:
- Table avec les champs
  - file.mtime
- Ne retenir que les notes où file.mtime >= aujourd'hui - 2 jours
- Tri descendant par date de modification
%%

```dataview
table file.mtime
where file.mtime >= date(today) - dur(2 days)
sort file.mtime desc
```
## Task
```dataview
task from "_Sandbox"
```
## Metadata
### Plusieurs acteurs par fiche
```dataview
table acteurs from "_Sandbox/Tests dataview/Films" where pays="France"
```
### Flatten : 1 acteurs par fiche
```dataview
table acteurs from "_Sandbox/Tests dataview/Films" where pays="France" flatten acteurs
```
### Le pays contient SA
```dataview
table acteurs from "_Sandbox/Tests dataview/Films" where contains(pays,"SA")
```
## Références
[Tutoriel Obsidian en français, le plugin Dataview créer des listes de notes](https://www.youtube.com/watch?v=jdNyKhm0QsM)
## Liens