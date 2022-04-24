# Dailies
->[[Archive/Dailies/old|Mes anciennes notes]]
## Mes notes quotidiennes
%%
dataview:
- Table avec les champs path, type, status
- Notes contenant un lien vers MOC/current/DAYS
- Tri par type, path, name
%%

```dataview
table file.path, type, status
from "Archive/Dailies/current"
where type="daily"
sort type, file.path, file.name
```
