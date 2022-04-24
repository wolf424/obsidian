---
alias:
creation: 2021-08-26
modification: 2021-08-26
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

FILL_HERE2:
Page de menu de niveau supérieur
- _HOME: menu principal


FILL_HERE4:
Page de menu de niveau inférieur
- _Menu/_moc: menu des Maps of Content (MOC)
- _Menu/_days: menu des notes quotidiennes (dailies)
- _Menu/_litt: menu des notes littéraires
- _Menu/_perm: menu des notes permanentes
- _Menu/_menu: menu des pages de menu
- _Menu/_proj: menu des pages de projet
- _Menu/_asst: menu des références à ma bibliothèque (assets)
- _Menu/_sand: menu des expérimentations dans le bac à sable (sandbox)
- _Menu/todo: menu des TODO lists
- _Menu/admn: menu des pages d'administration de ma base
- _Menu/help: menu des pages d'aide

- _Menu/_litt/Cours: menu des notes littéraires de type cours
- _Menu/_litt/Conférences: menu des notes littéraires de type conference 
- _Menu/_litt/Formations: menu des notes littéraires de type formation
- _Menu/_litt/Lectures: menu des notes littéraires de type lecture
- _Menu/_perm/Idées: menu des notes permanentes de type idee
- _Menu/_perm/Contacts: menu des notes permanentes de type contact
- _Menu/_perm/Références: menu des notes permanentes de type ref
- _Menu/_perm/Citations: menu des notes permanentes de type quote

FILL_HERE5:
Titre de cette page de menu

MOC de cette note
- MOC/current/MENU: espace des pages de menu

FILL_HERE7:
Hashtags portant sur toute cette page de menu

FILL_HERE8:
Lien vers ce qui sera l'aide contextuelle pour page de menu
- Par défaut : une définition de concept obsidian
  dans /_Menu/_help/_def/
- Ou bien une aide plus générale dans /_Menu/_help/

FILL_HERE11:
Titre de cette section

FILL_HERE12:
Hashtags portant sur cette section seulement

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

[[_HOME|⇈]] [[_HELP|?]] [[_Templates/menu|T]] menu: ↑[[_Menu/?|Niveau supérieur]]`FILL_HERE2` ==[[_Menu/?|Ce niveau]]==`FILL_HERE3` ↓[[_Menu/?|Niveaux inférieurs]] `FILL_HERE4`

# Menu - Titre`FILL_HERE5`
MOC [[MOC/current/MENU|MENU]] %% hashtags %% #menu `FILL_HERE7` [[_Menu/_help/_def/Menu/?|?]]`FILL_HERE8` 

## Section `FILL_HERE11`
%% hashtags %% `FILL_HERE12` [[_def|?]]`FILL_HERE13` # Menu - Map of Contents (MOC)
## MOC/NONE
[[MOC/NONE|NONE]] : MOC à laquelle sont rattachées les autres MOCs
## Toutes les MOCs
%%
dataview:
- Table avec les champs path, type, status
- Notes contenant un lien vers MOC/current
- Tri par path, name
%%

```dataview
table file.path, type, status
from "MOC/current" 
sort file.path, file.name
```
