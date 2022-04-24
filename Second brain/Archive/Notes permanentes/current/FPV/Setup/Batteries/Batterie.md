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

# La batterie
MOC [[MOC/current/PERM|PERM]] %% hashtags %% #perm #fpv [[_Menu/_help/_def/Note permanente|?]]

Nos quads sont très énergivores, ils ont besoin de batteries capables de délivrer d’importantes puissances en très peu de temps. C’est pourquoi on utilise essentiellement des batteries à base de **Lithium Polymère**, que l’on nomme communément « **LiPos**« . Quelques caractéristiques importantes d’une [[LiPo]] :

- Le **nombre de cellules** (souvent de 1 à 6), qui définit la tension de la LiPo. La tension nominale d’une cellule est de 3,7V. Une LiPo 4S, contiendra 4 cellules en série et aura donc une tension nominale de 14,8V (3,7×4).
    
- Une **capacité**, indiquant la quantité de courant qu’elle peut délivrer pendant une heure, exemple : 1500 mAh.
    
- Un **taux de décharge**, permettant de calculer la quantité maximale de courant qu’une LiPo peut délivrer à un instant T. Une LiPo de 1500 mAh avec un taux de décharge de 100C, pourra délivrer en continu 1,5 x 100 = 150A. En général, elles sont en mesure de délivrer le double pendant quelques secondes. Cette caractéristique reste à prendre avec des pincettes, les fabricants prenant pas mal de libertés.
    
- Un **connecteur**, pour la brancher au quad ou au chargeur, le plus répandu étant le [[XT60]], ou le [[XT30]] pour les plus petites LiPos. Les plus petits engins volants comme les TinyWhoop ont des connecteurs encore plus petits, de type [[JST]], [[JST-PH]] et plus récemment [[BT2.0]].
  

Les LiPos peuvent être **dangereuses** et doivent être utilisées et stockées de manière **sécurisée**. Voici quelques règles à suivre pour éviter les mauvaises surprises :

-   Privilégier un chargeur de qualité (SkyRC, ISDT, etc.) supportant jusqu’à 6S et offrant quelques options utiles comme la décharge, le stockage, la mesure de la résistance interne, la gestion des LiPos HV (High Voltage, pouvant être chargées jusqu’à 4,35V par cellule au lieu de 4,2V pour une LiPo classique).
    
-   Ne pas charger trop fort ni trop lentement, idéalement à 1 ou 2C (par exemple à 2A pour une lipo de 1500mAh).
    
-   Ne jamais complètement décharger une LiPo (s’arrêter à 20% ou 3,5V par cellule), pour lui garantir une bonne durée de vie. Si une cellule descend sous les 3V, elle sera certainement irrécupérable.
    
-   Toujours rester à côté de ses LiPos pendant qu’elles chargent.
    
-   Toujours charger les LiPos en mode « balance » pour s’assurer que chaque cellule est également chargée.
    
-   Quand une LiPo n’est pas utilisée pendant une longue période, la passer en mode stockage (~3,85V par cellule), toujours pour préserver sa durée de vie.
    
-   Conserver ses LiPos dans un conteneur adapté. Les boites de munitions (en métal) sont bien adaptées, à condition de retirer une partie de l’étanchéité (pour éviter l’effet cocotte minute en cas de fuite ou de feu). On peut même ajouter un morceau de placoplatre au fond.