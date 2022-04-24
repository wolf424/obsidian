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

# Flight Controler (FC)
MOC [[MOC/current/PERM|PERM]] %% hashtags %% #perm #fpv [[_Menu/_help/_def/Note permanente|?]]

Contrôleur de vol
C’est le chef d’orchestre, un vrai petit ordinateur.

Il embarque d’ailleurs un microprocesseur ou **[[MPU]]** (de génération **[[F4]],** **[[F7]]** ou encore **[[H7]]** pour les plus récents), des [[capteurs]] (gyroscope, accéléromètre, capteur de tension, etc.) et propose des entrées/sorties (**[[UART]]s**), accessibles grâce à des pads à souder pour y connecter le reste des périphériques du quads ([[ESC]]s, [[Rx]], [[vTx]], etc.).

Bien souvent, c’est la FC qui ajoute l’**OSD** au-dessus du flux vidéo de la caméra. L’OSD permet de visualiser dans le retour vidéo plein d’informations utiles (comme l’état des lipos, la durée du vol, la qualité du signal radio etc.).

Il se présente sous la forme d’une carte électronique, au format 20×20 ou 30×30 (et même 16×16 ou 26×26 pour les nano quads). Quand la FC est vendue avec des ESCs 4-en-1, on parle de « **stack** » (pile de cartes électroniques).

On notera l’existence de FC « **AiO** » (All-In-One), qui intègrent plusieurs fonctionnalités :

-   PDB, pour l’usage d’ESCs séparés.
    
-   ESCs, de plus en plus fréquent pour les TinyWhoop ou Toothpicks.
    
-   Le vTx et le Rx sont parfois aussi de la partie.
    
Pour fonctionner, une FC s’appuie sur un logiciel embarqué. Comme pour les ESCs, on parle de **firmware**. Les plus répandus étant
- [[Betaflight]]
  (https://www.youtube.com/watch?v=sq5vvs5SU_g&list=PLr-Mb5AXisr8Ccn7yrT0l4dk7Lro8ft4B)
- [[KISS]]
  (https://www.youtube.com/watch?v=miXcl5HMsCA&list=PLr-Mb5AXisr_D6p395AJLbB8Mq4DUrsQV)
- [[Emuflight]]
  (https://www.youtube.com/watch?v=KkUiwEqJIKk&list=PLr-Mb5AXisr94s2kqSuUOXb1nSdfn5sKY)
- [[FlightOne]]/[[FalcoX]]
  (https://www.youtube.com/watch?v=8y9pf4I91rU&list=PLr-Mb5AXisr9wweJmBUqyp-N2UjQ4CXuh)
  
D’autres sont plus orientés « vol autonome », comme c’est le cas pour [[iNav]].

Ce firmware a la lourde tâche d’analyser en temps réel tout ce qui se passe pour adapter le comportement du quad aux ordres reçus via le Rx. C’est lui qui indique aux [[ESC]]s à quelle vitesse faire tourner chaque moteur.

Chaque quad étant différent, on peut aider le firmware à ajuster son comportement pour qu’il corresponde le mieux possible au quad, et ainsi procurer de meilleures sensations de vol. Ces ajustements se font via des paramètres : les **[[PIDs]]** (Proportionnelle, Intégrale, Dérivée) et les **filtres** (qui visent à supprimer les parasites des différents signaux). Ce sujet dépasse largement le cadre de cet article, mais sachez que ça existe, et un jour ou l’autre, vous vous y intéresserez de plus près.
