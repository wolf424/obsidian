---
alias:
metadata: 02
author: AUGST-MERELLE Alexandra
type: index
status: ready
keywords: main, diy, domotique
creation: 2021-06-27
modification: 2021-06-27
---
 | 
------------ | ------------
MOC | [[DOMOTIQUE]]
Project | [[Domotique (Projet)]]
Template | [[Archive/Notes permanentes]]
Source | [[AUGST-MERELLE Alexandra]]
# Domotique
## Hardware
### Sonoff
```dataview
list
from "Archive/Notes permanentes" AND [[Domotique (Projet)]]
where contains(keywords,"hardware") AND contains(keywords,"sonoff")
sort type, file.name
```
### esp32
```dataview
list
from "Archive/Notes permanentes" AND [[Domotique (Projet)]]
where contains(keywords,"hardware") AND contains(keywords,"esp32")
sort type, file.name
```
### Autres
```dataview
list
from "Archive/Notes permanentes" AND [[Domotique (Projet)]]
where contains(keywords,"hardware") 
AND !contains(keywords,"esp32")
AND !contains(keywords,"sonoff")
sort type, file.name
```
## Firmware
```dataview
list
from "Archive/Notes permanentes" AND [[Domotique (Projet)]]
where contains(keywords,"firmware")
sort type, file.name
```
## Software
### Flasher le firmware
```dataview
list
from "Archive/Notes permanentes" AND [[Domotique (Projet)]]
where contains(keywords,"flash")
sort type, file.name
```
### Software
```dataview
list
from "Archive/Notes permanentes" AND [[Domotique (Projet)]]
where contains(keywords,"software")
sort type, file.name
```
