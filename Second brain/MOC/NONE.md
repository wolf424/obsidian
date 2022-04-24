---
alias:
creation: 2021-08-25
modification: 2021-08-25
type: moc
status: ready
---

%%
header: #v1-01-11 (header version)

description: MOC NONE pour autres MOCs

type:
- moc: Map of Content (MOC)

template:
- _Templates/_moc: Map of Content (MOC)

Page de menu de niveau supérieur
- _HOME: menu principal

Page de menu de ce niveau
- _Menu/_moc: menu des Maps of Content (MOC)

MOC de cette note
- MOC/NONE: par défaut (une MOC n'appartient pas à une MOC)

TODO:
- 
%%

%% MENU
- ⇈ : page de menu principale (HOME)
- ? : page d'aide principale
- T : template pour les notes de ce type
%%

[[_HOME|⇈]] [[_HELP|?]] [[_Templates/_moc|T]] menu: ↑[[_HOME|HOME]] ==[[_Assets/_Menu/_moc|MOCs]]==

# MOC - NONE
MOC [[MOC/NONE|NONE]] %% hashtags %% #moc #none [[_Assets/_Menu/_help/_def/Map of Content|?]] 

%% Navigation dans l'arborescence de cette MOC %%

↓[[MOC/current/DAYS|DAYS]]: espace des notes quotidiennes (dailies)
↓[[MOC/current/LITT|LITT]] : espace des notes littéraires
↓[[MOC/current/PERM|PERM]] : espace des notes permanente
↓[[MOC/current/MENU|MENU]] : espace des pages de menu
↓[[MOC/current/PROJ|PROJ]] : espace des pages de projet
↓[[MOC/current/ASST|ASST]] : espace des références à ma bibliothèque (assets)
↓[[MOC/current/SAND|SAND]] : espace des expérimentations dans le bac à sable (sandbox)
↓[[MOC/current/TODO|TODO]] : espace des TODO lists
↓[[MOC/current/ADMN|ADMN]] : espace des pages d'administration de ma base
↓[[MOC/current/HELP|HELP]] ! espace des pages d'aide

## Notes rattachées à cette MOC
%% hashtags %% #note [[Note|?]]

Notes rattachées à MOC/NONE

%%
dataview:
- Table avec les champs path, type, status
- Notes contenant un lien vers MOC/NONE
- Tri par path, name
%%

```dataview
table file.path, type, status
from [[MOC/NONE]] 
sort type, file.path, file.name
```