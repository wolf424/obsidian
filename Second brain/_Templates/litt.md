---
alias: FILL_HERE
creation: {{date}}
modification: {{date}}
type: litt
status: draft
---

%%
header: #v1-01-11 (header version)

FILL_HERE:
description: note littéraire, 

FILL_HERE:
alias: aliases pour cette note littéraire

type:
- litt: note littéraire
  - cours: cours
  - conférence: conférence
  - formation: formation
  - lecture: lecture d'article ou livre

FILL_HERE:
description: descriptif de cette note littéraire

template:
- _Templates/litt: notes littéraires
  - _Templates/litt/cours: cours
  - _Templates/litt/conference: conférences
  - _Templates/litt/formation: formations
  - _Templates/litt/lecture: lectures d'articles ou livres

Page de menu de ce niveau
- _Menu/_litt: menu des notes littéraires

Page de menu de niveau inférieur
- _Menu/_litt/Cours: menu des notes littéraires de type cours
- _Menu/_litt/Conférences: menu des notes littéraires de type conference 
- _Menu/_litt/Formations: menu des notes littéraires de type formation
- _Menu/_litt/Lectures: menu des notes littéraires de type lecture

FILL_HERE5:
Type (MOC ou type) et titre de cette note

MOC de cette note
- MOC/current/LITT: espace des notes littéraires

FILL_HERE7:
Hashtags portant sur toute cette note littéraire

FILL_HERE9:
Note de niveau supérieur dans les MOCs et types

FILL_HERE10:
Notes de niveau inférieur dans les MOCs et types

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

[[_HOME|⇈]] [[_HELP|?]] [[_Templates/litt|T]] menu: ↑[[_HOME|HOME]] ==[[_litt|litt]]== ↓[[Conférences|conférences]] ↓[[Cours|cours]] ↓[[Formations|formation]] ↓[[Lectures|lectures]]

# Note littéraire - Titre`FILL_HERE5`
MOC [[MOC/current/LITT|LITT]] %% hashtags %% `FILL_HERE7` [[_Menu/_help/_def/Note littéraire|?]]

## Section `FILL_HERE11`
%% hashtags %% `FILL_HERE12` [[_def|-?-]]`FILL_HERE13` 