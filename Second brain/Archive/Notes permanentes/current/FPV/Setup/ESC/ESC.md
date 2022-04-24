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

# Contrôleurs des moteurs (ESC)    
MOC [[MOC/current/PERM|PERM]] %% hashtags %% #perm #fpv [[_Menu/_help/_def/Note permanente|?]]

On les nomme **ESC**s pour **E**lectronic **S**peed **C**ontroller. Ce sont eux qui récupèrent l’énergie de la LiPo et la transforme à un format permettant de faire tourner les moteurs à la vitesse voulue. Ils utilisent une électronique assez avancée et intègrent un logiciel (**firmware**) pour assurer leur fonctionnement. Ce logiciel peut être mis à jour. Aujourd’hui, on retrouve essentiellement les firmwares **BLHeli_S** et **BLHeli_32** (le plus avancé).

Il y en un pour chaque moteur, parfois, ils sont « **séparés** » et trouvent leur place sur les bras du quad, mais de plus en plus, on les trouve au format « **4-en-1**« . Dans ce cas, ils sont réunis sur une même carte électronique au format 20×20 ou 30x30mm (espacement des trous pour la fixation).

Dans le cas de 4-en-1, c’est généralement sur la carte des ESCs que l’on connecte la LiPo. Pour des ESCs séparés, il faudra les alimenter autrement, par exemple en utilisant une **PDB** (Power Distribution Board) comme la [Airbot Matrix](https://www.youtube.com/watch?v=l9LOM1QI05Q) qui se chargera de fournir l’énergie aux différents composants du quad.

Les ESCs reçoivent les directives concernant concernant la vitesse que doit avoir chaque moteur grâce à un protocole leur permettant de communiquer avec le « cerveau » du quad. Au fil du temps, de nombreux protocoles se sont succédé. On retiendra qu’un protocole numérique s’est imposé, le **DShot**. Il est disponible sous plusieurs déclinaisons (DShot300, 600, 1200, etc.) dont la vitesse de communication est plus ou moins rapide.

### Flash et configuration des ESCs

Pour les ESCs, c’est plus simple, 2 firmwares équipent la plupart des ESCs du marché : **[[BLHeli_S]]** et **[[BLHeli_32]]**, ce dernier étant la version actuelle. BLHeli_S est encore très présent mais n’est plus mis à jour (excepté via ses déclinaisons JESC et JazzMaverick).

Pour mettre à jour et configurer des ESCs sous BLHeli_S, deux logiciels sont disponibles : [BLHeliSuite16](https://github.com/bitdump/BLHeli/tree/master/BLHeli_32%20ARM) et [BLHeli Configurator](https://github.com/blheli-configurator/blheli-configurator/releases).

Concernant BLHeli_32, un seul logiciel : [BLHeliSuite32](https://github.com/bitdump/BLHeli/tree/master/BLHeli_32%20ARM).

La connexion aux ESCs via ces logiciels passe également par le connecteur USB de la FC. Par contre, le quad doit être branché sur une LiPo, sinon les ESCs ne sont pas alimentés et ne seront donc pas accessibles. Il faut donc enlever les hélices des moteurs pour ce genre d’opération !

Généralement, on ne passe pas trop de temps sur cet outil, juste pour mettre à jour les ESCs si nécessaire et changer le sens de rotation des moteurs si certains ne tournent pas dans le bon sens. Sous BLHeli_32, une bonne recommandation est de passer le **PWM Frequency** à « 48 kHz » et le **Motor Timing** à « Auto ».

Comme pour BetaFlight, vous n’aurez aucune difficulté à trouver des tutos en ligne pour avoir plus de d’information concernant l’utilisation de ces logiciels.

###