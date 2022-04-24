# Menu - Citations
↑[[_perm|Notes permanentes]]
## Nouvelle citation
Depluis le menu ->[[Citations|Citations]]
## Toutes les citations

%%
dataview:
- Table avec les champs path, type, status
- Notes contenant un lien vers MOC/NONE
- Tri par path, name
%%

```dataview
table file.path, type, status
from "Archive/Notes permanentes"
where type="quote"
sort file.path, file.name
```
