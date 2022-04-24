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

# Betaflight
MOC [[MOC/current/PERM|PERM]] %% hashtags %% #perm #fpv [[_Menu/_help/_def/Note permanente|?]]
    
### Flash et configuration du contrôleur de vol

On l’a vu précédemment, il existe plusieurs firmwares pour nos FC. On utilisera l’exemple de BetaFlight, mais les autre firmwares suivent le même principe, avec des logiciels différents.

Tout d’abord, il faut différencier 2 concepts :

-   Le **[[Firmware]]** (**BetaFlight**) : c’est le logiciel installé sur la FC qui s’exécutera pour faire fonctionner votre drone.
    
-   Le **configurateur** (**BetaFlight Configurator**) : c’est le logiciel qui permettra de configurer le firmware via une interface graphique ergonomique mais également de flasher votre FC pour mettre à jour le firmware (ou en installer un nouveau).
    

Nous allons survoler rapidement l’interface de BetaFlight Configurator pour donner un aperçu rapide : sa configuration est un sujet à part entière et de [nombreux tutoriaux](https://www.youtube.com/watch?v=sq5vvs5SU_g&list=PLr-Mb5AXisr8Ccn7yrT0l4dk7Lro8ft4B) sont disponibles pour vous aider.

Une fois que vous avez téléchargé la dernière version de [BetaFlight Configurator](https://github.com/betaflight/betaflight-configurator/releases), vous pouvez le démarrer et connecter la FC de votre quad à votre PC avec un câble USB. Il suffit de choisir le port qui est apparu dans la liste déroulante en haut à droite et cliquer sur « Connexion ». Vous êtes maintenant connecté à votre drone :

On remarque également un bouton en haut à droite « Mise à jour du firmware ». C’est grâce à ce bouton que l’on pourra installer une nouvelle version du firmware sur la FC.

L’application est organisée sous forme d’onglets accessibles via la colonne de gauche. Elle va nous permettre de configurer tout le matériel que nous avons vu un peu plus tôt dans cet article. Voici les principaux onglets :

-   **Installation :** c’est l’écran d’accueil une fois la connexion au quad établie. Il permet de sauvegarder ou charger la configuration du drone, calibrer l’accéléromètre (utilisé en vol stabilisé) et affiche quelques informations, notamment un modèle 3D du quad qui s’anime en temps réel en fonction de la position du quad.
    
-   **Ports :** cet onglet permet de configurer les entrées/sorties (UARTs) de la FC. On y indiquera sur quel port est connecté le récepteur radio par exemple
    
-   **Configuration :** certainement le plus important, il permet de configurer les paramètres principaux comme le protocole à utiliser pour communiquer avec les ESCs (ex: DShot 600), celui à utiliser pour communiquer avec le récepteur radio (ex: Serial SBUS), la fréquence de lecture du gyro et de la boucle PIDs, l’orientation de la FC etc.
    
-   **Alimentation et batterie :** permet de configurer des informations liées à l’utilisation de la lipo : seuil des alertes, ajustement des capteurs de tension et courant etc. En général, on n’a pas besoin de toucher grand-chose ici
    
-   **Réglages de PID :** c’est ici que l’on ajuste le comportement du quad. Les réglages de base sont supposés fonctionner sur pas mal de machines. Il est organisé en 3 sous-onglets : les PIDs (pour que le drone vole proprement), les rates (pour ajuster le comportement du quad par rapport aux mouvements des sticks de la radio) et les filtres, pour ajuster la manière dont le quad va nettoyer les différents signaux en entrée (gyroscope) et en sortie (D Term)
    
-   **Récepteur :** cet onglet permet de vérifier que la communication entre la radio et la FC (en passant par le Rx) est fonctionnelle, on pourra notamment voir les valeurs transmises pour chaque « voie » (gaz, roll, pitch, yaw, interrupteurs). D’autres réglages liés au récepteur radio sont disponibles. En fonction des FC, il peut être nécessaire de brancher la LiPo pour que le Rx soit alimenté
    
-   **Modes :** la radio transmet les actions du pilotes via des « voies ». Certaines voies sont dédiées à des interrupteurs de la radio pour des actions spécifiques : armer le quad, faire sonner le buzzer, activer/désactiver la stabilisation etc. Cet onglet « Modes » permet de dire au contrôleur de vol à quelle fonction correspond chaque voie arrivant depuis la radio.
    
-   **Moteurs :** cet onglet permet de tester les moteurs (sans hélices !). Là aussi, la LiPo devra impérativement être branchée. C’est grâce à cet onglet que l’on peut vérifier facilement que chaque moteur est à la bonne place et tourne dans le bon sens
    
-   **OSD :** ici on configure quelles informations on souhaite voir dans le retour vidéo et à quel endroit elles devront apparaître
    
-   **Émetteur vidéo :** si le vTx fournit une fonctionnalité comme le Smart Audio, pour configurer le vTx depuis la FC, cet onglet permet de configurer la fonctionnalité
    
-   **Blackbox :** dédié à l’enregistrement des données pour analyser un vol, il s’agit d’une fonctionnalité avancée permettant de diagnostiquer d’éventuels problèmes ou d’avoir des informations pour optimiser au maximum les réglages du drone
    
-   **CLI :** donne accès à une ligne de commandes pour communiquer avec la FC. Tous les réglages faits via les interfaces peuvent être faits en ligne de commande, et certains réglages sont accessibles uniquement via le CLI. Voici quelques commandes qu’il est bon de connaître :
    
    -   status : fournit un ensemble d’informations de base (versions, statut de l’armement, occupation du CPU etc.)
        
    -   bl (anciennement dfu) : permet de redémarrer la FC en mode « flashage » (dfu) pour installer un nouveau firmware
        
    -   dump : extrait toute la configuration du quad (il suffira de copier/coller le contenu d’un dump dans le CLI pour recharger une configuration complète)
        
    -   diff all : extrait la configuration du quad qui a été modifiée par rapport à la configuration par défaut (c’est souvent suffisant et plus facile à exploiter qu’un dump)
        
    -   save : sauvegarde les modifications sur la FC
    