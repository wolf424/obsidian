# Aide - Architecture
Architecture de ma base
## Catégories d'objets
**Maps of Content (MOC)** : espaces de nommage.
- Toute note est rattachée à une et une seule MOC, via un lien sous son titre
- Des notes de plusieurs types peuvent être rattachées à la même MOC.

**Types**
- Le type est spécifié dans l'entête de la note
- Les types sont prédéfinis dans le bloc racine
- Le type d'une note correspond à une mise en forme de cette note
- À cette fin, chaque nouvelle note est créée à partir d'un template

**Templates**
- Un template est un modèle de note
- Un template est toujours rattaché à une et une seule MOC
- Plusieurs templates peuvent être rattachés à un même type de note

**Notes**

## Description
### Entête
Des [[Blocs de texte|blocs de texte]] sont définis dans les templates. Ils sont à la source d'une cascade de dépendances :

Les fragments Une entête générique est définie sous la forme d'un fragment [[_Templates/blocks/block_header]] et
### MOCs
### 
## Dépendances
Opérations dans l'ordre pour mettre à jour l'entête
- MAJ [[_Templates/blocks/block_header]]
- MAJ [[_Templates/_none]]
- MAJ [[_Templates/_moc]]
- MAJ [[MOC/NONE]]
- MAJ toutes les [[_Assets/_Menu/_moc|MOCs]]
- MAJ tous les [[_templates|templates]]