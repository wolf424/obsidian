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

# Récepteur radio (Rx)
MOC [[MOC/current/PERM|PERM]] %% hashtags %% #perm #fpv [[_Menu/_help/_def/Note permanente|?]]

En général abrégé en « **Rx** » (pour Receiver), c’est lui qui reçoit les commandes envoyées par la radio et les transfère au quad (une fois la procédure de « **[[binding]]** » effectuée comme dans [cet exemple](https://www.youtube.com/watch?v=jhblEwYsMMg)). Certains modèles prennent également en charge la **télémétrie**, qui permet au drone et à la radio d’échanger d’autres informations, dans les 2 sens (par exemple pour faire remonter à la radio l’état de la LiPo ou la position GPS).

Le Rx utilise un protocole pour échanger avec le quad. Les plus répandus sont le **[[SBUS]]**, l’[[IBUS]], le [[F.Port]] ou le [[Crossfire]] (CRSF), en fonction des solutions choisies.

Le logiciel embarqué ([[Firmware]]) du Rx peut être mise à jour, souvent grâce à la [[radiocommande]], avec ou sans fil, pour supporter de nouvelles fonctionnalités.

## Recepteurs compatibles [[Access]]
Actuellement (mise à jour au 27/08/2019), voici la liste des [[Rx]] compatibles avec le protocole [[Access]] (via une mise à jour) :
- [[R-XSR]]
- [[R-X4R]]
- [[X-X6R]]
- [[G-RX6]]
- [[G-RX8]]
- [[XM+]]
- [[XM]]

Le [**R-XSR**](https://www.studiosport.fr/recepteur-frsky-r-xsr-a14022.html) **semble être un excellent choix** dans tous les cas !