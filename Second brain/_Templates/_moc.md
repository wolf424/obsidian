---
alias:
creation: {{date}}
modification: {{date}}
type: moc
status: draft
---

%%
header: #v1-01-11 (header version)

FILL_HERE:
description: MOC pour les FILL_HERE

type:
- moc: Map of Content (MOC)

FILL_HERE:
description: descriptif de cette MOC

template:
- _Templates/_moc: Map of Content (MOC)

Page de menu de niveau supérieur
- _HOME: menu principal

Page de menu de ce niveau
- _Menu/_moc: menu des Maps of Content (MOC)

FILL_HERE5:
Titre de cette MOC

MOC de cette note
- MOC/NONE: par défaut (une MOC n'appartient pas à une MOC)

FILL_HERE7:
Hashtags associés à cette MOC

TODO:
- 
%%

%% MENU
- ⇈ : page de menu principale (HOME)
- ? : page d'aide principale
- T : template pour les notes de ce type
%%

[[_HOME|⇈]] [[_HELP|?]] [[_Templates/_moc|T]] menu: ↑[[_HOME|HOME]] ==[[_Assets/_Menu/_moc|MOCs]]==

# MOC - Titre`FILL_HERE5`
MOC [[MOC/NONE|NONE]] %% hashtags %% #moc `FILL_HERE7` [[_Assets/_Menu/_help/_def/Map of Content|?]] 

%% Navigation dans l'arborescence de cette MOC %%
↑[[MOC/NONE|NONE]]
↓[[MOC/current/?|Niveaux inférieurs]] `FILL_HERE10`

## Notes rattachées à cette MOC
%% hashtags %% #note [[Note|?]]

Notes rattachées à MOC/NONE`FILL_HERE`

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