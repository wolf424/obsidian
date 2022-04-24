---
alias:
metadata: 01
author: AUGST-MERELLE Alexandra
type: howto
status: ready
creation: 2021-06-27
modification: 2021-06-27
---
 | 
------------ | ------------
MOC | [[DOMOTIQUE]]
Project | [[Domotique (Projet)]]
Template | [[Archive/Notes permanentes]]
Source | [[AUGST-MERELLE Alexandra]]
# Ajouter [[Caméra]] [[esp32cam]] [[Domoticz]] via [[Motion Eye]]
## Add a camera from [[Motion Eye]]
- In [[Motion Eye]] : Video Streaming / Snapshot URL : copy on clipboard
- In [[Domoticz]]
- Configuration / More options / Camera / Add a camera
- Fill name, eg : esp32cam01
- Fill (motioneye) IP, eg : 192.168.0.151
- Fill port : 8765
- Fill URL, picked from [[Motion Eye]], eg : picture/1/current
To get url, in [[Motion Eye]], go to Video Streaming / Snapshot URL
## Liens