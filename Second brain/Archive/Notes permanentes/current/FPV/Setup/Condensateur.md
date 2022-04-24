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

# Condensateur
MOC [[MOC/current/PERM|PERM]] %% hashtags %% #perm #fpv [[_Menu/_help/_def/Note permanente|?]]

Petit composant souvent sous-estimé, son rôle est d’**absorber les pics de tension** pour protéger l’électronique et **filtrer le bruit généré par les [[ESC]]s**.

On l’utilise avant tout pour limiter les perturbations qui peuvent apparaître dans le retour vidéo en analogique, mais il ne faut pas oublier ses effets « invisibles » de protection et de filtrage, par exemple : le gyroscope est très sensible, et plus le signal en entrée est propre, mieux le contrôleur de vol saura faire son travail (moins de filtrage logiciel à appliquer).

Le placement idéal d’un condensateur est au plus près de la source du bruit, et donc des ESCs. Pour des ESCs 4-en-1, on le soudera au niveau des pads de la pigtail permettant de connecter la LiPo. Pour des ESCs séparés, l’idéal est de mettre un petit condensateur sur chaque ESC. Un condensateur se soude en parallèle de l’alimentation, sur le « + » et le « -« , en prenant soin de respecter la polarité.

Un condensateur est définit par sa **capacité** (en µF) et sa **tension de service limite**, à [dimensionner en fonction de la configuration du quad](https://www.wearefpv.fr/best-of-forum-condensateur-low-esr-20171123/). Dernier point, il faut impérativement utiliser un condensateur « **LOW ESR** » (faible résistance série).
