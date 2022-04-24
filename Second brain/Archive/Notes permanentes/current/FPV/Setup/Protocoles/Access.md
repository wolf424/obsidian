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

# Protocole - Access
MOC [[MOC/current/PERM|PERM]] %% hashtags %% #perm #fpv [[_Menu/_help/_def/Note permanente|?]]

https://blog.studiosport.fr/frsky-point-sur-le-nouveau-protocole-access/

- Access est un protocole de chez [[FrSky]]
- C'est le successeur de [[ACCST]]  

### De nouvelles fonctionnalités

ACCESS (pour Advanced Communication Control, Elevated Spread Spectrum) est le successeur de [[ACCST]] chez [[FrSky]], il reprend les bases posées par ce dernier et amène de nouvelles fonctionnalités :

-   **Smart Match** : une fonctionnalité permettant d’obtenir une double certification du Tx et Rx, permettant de sécuriser votre transmission.
    
-   **Smart Share** : une nouveauté permettant de binder plusieurs radiocommandes sur le même récepteur, tout en assurant une certification unique pour chaque. Particulièrement utile pour des drones écoles qui peuvent ainsi être bindés pour plusieurs pilotes. Le Smart Share permet de binder, upgrader et configurer le récepteur radio sans devoir le connecter en filaire. 
    
-   **Trio Control** : une fonctionnalité de sécurité particulièrement intéressante pour les plus grosses / chères machines. Elle permet de binder jusqu’à 3 récepteurs en redondance sur le drone (ou autre modèle) apportant ainsi un gros ajout en sécurité, notamment en cas de [[failsafe]] d’un récepteur.
    

### Une latence réduite et 24 voies disponibles

L’arrivée du nouveau protocole ACCESS marque la possibilité désormais d’avoir 24 voies disponibles dans votre système de transmission radio. Peu utile dans le monde du drone racer, certains utilisateurs de grands modèles pourront y trouver leur compte notamment dans l’utilisation de drones proposant des fonctions particulières. 

L’un des gros points forts du protocole est la réduction de la latence que ce soit en mode 8 et 16 voies par rapport au ACCST. Le **mode 24 voies** bénéficie lui aussi **d’une latence très faible**, à peine plus élevée qu’en 16 voies. 

De plus [[FrSky]] annonce une portée de contrôle et de retour télémétrique augmentée de 40%, ce qui vient une nouvelle fois sécuriser vos vols.

## Quelles radiocommandes sont compatibles ACCESS ?

- FrSky renouvelle entièrement son catalogue de radiocommandes pour passer ses produits du protocole ACCST à ACCESS.
- Ainsi les radiocommandes [Taranis X-](https://www.studiosport.fr/radiocommande-taranis-x-lite-s-a17704.html)[Lite S](https://www.studiosport.fr/radiocommande-taranis-x-lite-s-a17704.html), [X-Lite Pro](https://www.studiosport.fr/radiocommande-taranis-x-lite-pro-2.4-ghz), [X9 Lite](https://www.studiosport.fr/radio-taranis-x9-lite-a18054.html) sorties depuis quelques mois sont compatibles. Les toutes nouvelles FrSky Taranis Horus X10 Express, Horus X10S Express et X9D Plus 2019 utiliseront ACCESS. 

Pour autant ces modèles **seront toujours compatibles avec le D16 en ACCST**. Toutefois la prise en charge du mode D8 ne sera plus possible d’origine par ses radiocommandes. Et c’est là où les choses se compliquent un peu..

## Compatibilité du mode D8 avec les radios ACCESS

C’est le principal effet de bord que ce nouveau protocole implique. En effet, les radiocommandes utilisant le protocole ACCESS, ne prenne pas en charge le mode D8 et contrairement aux anciens modèles, **elles ne peuvent être flashées**.

Ainsi, la solution pour binder votre drone est d’avoir un récepteur compatible D16 (EU-LBT si vous achetez votre matériel en Europe) ou ACCESS.

Dans le cas où vous auriez un récepteur D8 (ou LR12), il existe deux solutions : 

-   Changer de radiocommande vers un ancien modèle FrSky, mais ce n’est surement pas la meilleure voie à suivre. 
    
-   **Acquérir un module externe XJT** permettant de rendre les radiocommandes ACCESS compatibles avec le mode D8. Ce module d’émission vient se plugger sur le module JR de votre radiocommande.
    

Et c’est surement cette dernière solution qui sera la plus utile. Le module XJT Lite sera compatible avec les radiocommandes Taranis X-Lite S, X-Lite Pro et X9 Lite, tandis que le XJT classique pourra être positionné sur les Taranis Horus X10 Express, Horus X10S Express et X9D Plus 2019. 

## Quels [[Rx|récepteurs]] sont compatibles ACCESS ?

Actuellement (mise à jour au 27/08/2019), voici la liste des [[Rx]] compatibles avec le protocole [[Access]] (via une mise à jour) :
- [[R-XSR]]
- [[R-X4R]]
- [[X-X6R]]
- [[G-RX6]]
- [[G-RX8]]
- [[XM+]]
- [[XM]]

Le [**R-XSR**](https://www.studiosport.fr/recepteur-frsky-r-xsr-a14022.html) **semble être un excellent choix** dans tous les cas !