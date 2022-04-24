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

# Le transmetteur vidéo (VTX)
MOC [[MOC/current/PERM|PERM]] %% hashtags %% #perm #fpv [[_Menu/_help/_def/Note permanente|?]]

Communément appelé **vTx** (pour Video Transmitter), il récupère le flux vidéo filmé par la caméra FPV pour le transmettre à un récepteur (masque, lunettes, écran,etc.) via un signal radio, le plus souvent en 5.8 Ghz. La fréquence sur laquelle émet un VTX est déterminée par une **bande** et un **canal**.

En général, on se positionne sur la « **[[Raceband]]** » qui a le mérite de répartir au mieux les canaux sur des fréquences suffisamment espacées pour pouvoir voler à plusieurs sans se gêner. La **puissance** du vTx est également réglable, même si la législation française impose de ne pas dépasser les 25mW.

La plupart des émetteurs récents proposent une fonctionnalité « **Smart Audio** » ou « IRC Tramp » permettant de régler son vTx à distance.

Un vTx nécessite une **antenne** pour émettre. D’ailleurs prudence : ne jamais mettre un vTx sous tension sans antenne connectée sous peine de le griller. On retrouve 2 types de connecteurs au niveau du vTx : le **µ.Fl** et le **MMCX**.

## Faits
- La transmission d’un flux vidéo en temps réel utilise le plus souvent la technologie 5,8 GHz (plage de fréquences entre 5645 et 5945 MHz)
- cf [[Fréquence vidéo]]