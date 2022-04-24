# Admin - Infrastructure
## [[_templates|Templates]]
### Template racine
[[_none|NONE]] : template racine (le plus générique)
- Son entête doit être de même version que [[block_header|block_header]]
- Son menu doit être celui de [[block_menu|block_menu]]
- Son titre doit être celui de [[block_titles|block_titles]]
#### Blocs de texte
Tous les blocs de texte :
%%
dataview:
- Table avec les champs file.path
- Depuis le dossier "_Templates/blocks"
- Seulement les file.tags ne contenant pas #v0-01-05
- Seulement les file.name contenant "block_"
%%

```dataview
table file.path
from "_Templates/blocks"
sort file.name
```

### Templates à mettre à jour

Templates sans le tag #v0-01-05:

%%
dataview:
- Table avec les champs type, status, file.path
- Depuis le dossier "_Templates"
- Seulement les file.tags ne contenant pas #v0-01-05
- Seulement les file.name ne contenant pas "block_"
%%

```dataview
table type, status, file.path
from "_Templates"
where !contains(file.tags,"#v0-01-05") AND !contains(file.name,"block_") 
sort file.name
```
## [[_Assets/_Menu/_moc|MOCs]]
## [[_Assets/_Menu/_help|Aide]] de cette vault
## [[_days|Dailies]]
## [[_Menu/_def]]