---
alias:
creation: 2021-08-26
modification: 2021-08-26
type: menu
status: draft
---

%%
header: #v1-01-11 (header version)

description: page de menu principale

type:
- menu: page de menu

template:
- _Templates/menu: pages de menu

TODO:
- 
%%

%% MENU
- ⇈ : page de menu principale (HOME)
- ? : page d'aide principale
- T : template pour les notes de ce type
%%

[[_HOME|⇈]] [[_HELP|?]] [[_Templates/menu|T]] menu: ==[[_HOME|HOME]]== ↓[[_Assets/_Menu/_moc|moc]] ↓[[_days|days]] ↓[[_litt|litt]] ↓[[_perm|perm]] ↓[[_menu|menu]] ↓[[_proj|proj]] ↓[[_asst|asst]] ↓[[_sand|sand]] ↓[[_Assets/_Menu/_todo|todo]] ↓[[_admn|admn]] ↓[[_Assets/_Menu/_help|help]]

# Menu - HOME
MOC [[MOC/current/MENU|MENU]] %% hashtags %% #menu [[_HELP_|?]]

## Seeds
%% hashtags %% #seed [[_Menu/_help/_def/Seed|?]]

Notes non classées :

%%
dataview:
- Liste
- Depuis le dossier "_Seeds"
- Trier par type, path et nom de fichier
%%
```dataview
list
from "_Seeds"
sort type, file.path, file.name
```

## [[_proj|Projets]]
%% hashtags %% #projet [[Projet|?]]

### [[Archive/Projets/old|Ancienne version]]

## Notes littéraires
**[[_Sandbox/dataview|dataview]]** : notes du dossier "Archive/Notes littéraires/current"

%%
dataview:
- Liste
- Depuis le dossier "Archive/Notes littéraires/current"
- Trier par type, path et nom de fichier
%%
```dataview
list
from [[MOC/current/LITT]]
sort type, file.path, file.name
```
### [[Archive/Notes littéraires/old|Ancienne version]]


## Notes permanentes
```dataview
table file.path, type, keywords
from "Archive/Notes permanentes"
AND [[_Projects/THEME (Project)]]
where status!="draft"
where file.name!="_index"
sort type, file.name
```
### Anciennes notes
#obsolete
```dataview
list file.path
from "Archive/Notes permanentes"
where type="index"
sort type, file.name
```
## Notes en draft
```dataview
table file.path, type, keywords
from "Archive/Notes permanentes"
AND [[_Projects/THEME (Project)]]
where status="draft"
sort type, file.name
```

## Consulter
Fiches dont le status est toread (sauf templates)
```dataview
list
where status="toread"
where !contains(file.path,"_Template")
```
### Brouillons
- Mes brouillons sont les fiches dont le status est [[Status|draft]]
(sauf celles du dossier templates)
```dataview
table file.path
where status="draft"
where !contains(file.path,"_Template")
```


