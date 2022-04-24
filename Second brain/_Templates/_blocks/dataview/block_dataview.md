
%%
dataview:
- Table avec les champs path, type, status
- Notes contenant un lien vers MOC/NONE
- Tri par type, path, name
%%

```dataview
table file.path, type, status
from [[MOC/NONE]] 
sort type, file.path, file.name
```
