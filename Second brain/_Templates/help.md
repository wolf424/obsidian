%%
header: #v0-01-07  (header version)
description: FILL_HERE

FILL_HERE:
alias: aliases pour cette note
type:
- none: par défaut (non spécifié)
- moc: Map of Content (MOC)
- days: note quotidienne (dailies)
- litt: note littéraire
  - cours: cours
  - conférence: conférence
  - formation: formation
  - lecture: lecture d'article ou livre
- perm: note permanente
  - idea: idée
  - contact: contact (personne, organisme)
  - ref: référence (vers une url)
  - quote: citation
- menu: page de menu
- projet: page de projet
- asset: référence à ma bibliothèque (assets)
- sandbox: expérimentation dans le bac à sable (sandbox)
- todo: TODO list
- admin: page d'administration de ma base
- help:  page d'aide
description: descriptif de cette note

FILL_HERE1:
Lien vers ce qui sera l'aide contextuelle pour cette note
- Par défaut : une définition de concept obsidian
  dans /_Menu/_help/_def/
- Ou bien une aide plus générale dans /_Menu/_help/

FILL_HERE2:
template:
- _Templates/_none: par défaut (non spécifié)
- _Templates/_moc: Map of Content (MOC)
- _Templates/days: notes quotidiennes (dailies)
- _Templates/litt: notes littéraires
  - _Templates/litt/cours: cours
  - _Templates/litt/conference: conférences
  - _Templates/litt/formation: formations
  - _Templates/litt/lecture: lectures d'articles ou livres
- _Templates/perm: notes permanentes
  - _Templates/perm/idea: idées
  - _Templates/perm/contact: contacts (personnes, organismes)
  - _Templates/perm/ref: références (vers une url)
  - _Templates/perm/quote: citations
- _Templates/menu: pages de menu
- _Templates/proj: pages de projet
- _Templates/asst: référence à ma bibliothèque (assets)
- _Templates/sand: expérimentations dans le bac à sable (sandbox)
- _Templates/todo: TODO lists
- _Templates/admn: pages d'administration de ma base
- _Templates/help: pages d'aide

FILL_HERE3:
Items du sous-menu

FILL_HERE4:
Titre principal de la note

FILL_HERE5:
MOC de cette note
- MOC/NONE: par défaut (MOC non spécifié)
- MOC/current/DAYS: espace des notes quotidiennes (dailies)
- MOC/current/LITT: espace des notes littéraires
- MOC/current/PERM: espace des notes note permanente
- MOC/current/MENU: espace des pages de menu
- MOC/current/PROJ: espace des pages de projet
- MOC/current/ASST: espace des références à ma bibliothèque (assets)
- MOC/current/SAND: espace des expérimentations dans le bac à sable (sandbox)
- MOC/current/TODO: espace des TODO lists
- MOC/current/ADMN: espace des pages d'administration de ma base
- MOC/current/HELP! espace des pages d'aide

FILL_HERE6:
Hashtags portant sur toute cette note

FILL_HERE7:
Titre d'une section

FILL_HERE8:
Aide contextuelle pour cette section

FILL_HERE9:
Hashtags portant sur cette section seulement

TODO:
- 
%%

%% MENU
- H : Retour à la page (HOME)
- ? : Aide principale
- C : Aide contextuelle pour cette note
- T : Template pour les notes de ce type
%%

[[_HOME|H]] [[_Assets/_Menu/_help|?]] [[_Menu/_help/_def/?|C]]`FILL_HERE1` [[_Templates/help|T]]

%% SUB-MENU %%

-> [[_Menu/?|Items du sous-menu]]`FILL_HERE3`

# Aide - `FILL_HERE4`
MOC [[MOC/NONE|NONE]]`FILL_HERE5` %% hashtags %% `FILL_HERE6`

## Section `FILL_HERE7`
[[_def|-?-]]`FILL_HERE8`  %% hashtags %% #help `FILL_HERE9` 



- **Description** : `FILL_HERE`

- **Contraintes** :
  - `FILL_HERE`

- **Propriétés** : `FILL_HERE`




%% SUB-MENU %%

-> [[_Menu/?|Items du sous-menu]]`FILL_HERE3`

%% MENU

[[_HOME|H]] [[_Assets/_Menu/_help|?]] [[_Templates/help|T]]

%% SUB-MENU %%

-> [[_Menu/_help/?|Aide connexe]]`FILL_HERE3`


