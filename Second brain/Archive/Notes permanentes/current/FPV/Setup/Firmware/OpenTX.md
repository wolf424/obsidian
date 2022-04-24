---
alias:
creation: 2021-09-07
modification: 2021-09-07
type: perm
status: draft
---

%%
header: #v1-01-11 (header version)

FILL_HERE:
description: note permanente

FILL_HERE:
alias: aliases pour cette note permanente

type:
- perm: note permanente
  - idea: idée
  - contact: contact (personne, organisme)
  - ref: référence (vers une url)
  - quote: citation

FILL_HERE7:
Hashtags portant sur toute cette note permanente

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

[[_HOME|⇈]] [[_HELP|?]] [[_Templates/perm|T]] menu: ↑[[_HOME|HOME]] ==[[_perm|perm]]== ↓[[_perm|Citations]] ↓[[_perm|Contacts]] ↓[[_perm|Idées]] ↓[[_perm|Références]]

# OpenTX
MOC [[MOC/current/PERM|PERM]] %% hashtags %% #perm #fpv [[_Menu/_help/_def/Note permanente|?]]

Firmware pour radiocommande

### Flash et configuration de la radiocommande

La radiocommande ne fait pas exception, elle aussi dispose de son firmware. Le plus répandu est le projet Open Source **OpenTX** (et ses déclinaisons par certains constructeurs).

Pour mettre à jour votre version d’OpenTX vous pouvez utiliser l’outil [OpenTX Companion](https://www.open-tx.org/downloads). Ce site vous donnera accès à un ensemble de ressources pour chaque version d’OpenTX (Companion, fichiers à déposer sur la carte SD de la radio).

Au delà de la mise à jour d’OpenTX, Companion permet de configurer votre radiocommande. Cette configuration peut aussi être faite à la main, directement sur la radio.

Sans entrer dans les détails, il faut savoir que la configuration de la radio se base sur la création de « Modèles ». Chaque modèle contient l’ensemble des infos permettant de décrire le « contrat » pour communiquer avec un quad (protocole, assignation des axes et interrupteurs sur des voies, binding avec les récepteurs radio etc.). Un même modèle peut-être utilisé avec plusieurs quads, si ces derniers utilisent le même protocole et que l’assignation des voies/modes est la même au niveau du contrôleur de vol.