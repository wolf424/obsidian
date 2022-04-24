---
alias:
creation: 2021-09-06
modification: 2021-09-06
type: menu
status: draft
---

%%
header: #v1-01-11 (header version)

FILL_HERE:
description: page de menu des FILL_HERE

type:
- menu: page de menu

template:
- _Templates/menu: pages de menu

MOC de cette note
- MOC/current/MENU: espace des pages de menu

FILL_HERE13:
Aide contextuelle pour cette section

TODO:
- 
%%

%% MENU
- ⇈ : page de menu principale (HOME)
- ? : page d'aide principale
- T : template pour les notes de ce type
%%

[[_HOME|⇈]] [[_HELP|?]] [[_Templates/menu|T]] menu: ↑[[_HOME|HOME]] ==[[_Menu/todo|TODO]]==

# Menu - TODO lists
MOC [[MOC/current/MENU|MENU]] %% hashtags %% #menu #todo [[TODO list|?]]

## Dans les [[_days|notes quotidiennes]]
hashtags: #daily
%%
dataview:
- notes du dossier /_Dailies_
- qui contiennent le hashtag #todo
%%

```dataview
list from "_Dailies"
where contains(file.tags,"#todo")
```
## Contenant `#todo`
hashtags: #daily
%%
dataview:
- Table avec les champs type
- qui contiennent le hashtag #todo
%%

```dataview
table type
from #todo
```
