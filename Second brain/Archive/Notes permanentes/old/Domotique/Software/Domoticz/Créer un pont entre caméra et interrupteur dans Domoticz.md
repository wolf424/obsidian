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
# Créer un [[pont]] entre [[Caméra]] et [[interrupteur]] dans [[Domoticz]]
## Create bridge between cameras and [[switches]]
In [[Domoticz]] :
- Configuration / Hardware
- Fill name, eg : Pont
- Fill type : Dummy
- In the bridge, for each camera click on Créer un capteur virtuel
  - Nom, eg : esp32cam01
  - Type : Interrupteur
- Onglet Interrupteurs : dummy switches appear for each [[camera]]

Link motion notification to [[Domoticz]]. In [[Motion Eye]] :
- Motion Notification
- Call a web hook
- Web hook URL, eg : (http://192.168.0.151:8080/json.htm?type=command&param=switchlight&idx=2&switchcmd=On)
  - IP in the URL = [[Domoticz]] IP
  - idx=2 (replace 2 by the idx of the switch in domoticz)
    - To get it, in [[Domoticz]] / Interrupteurs / Modifier

Configure switch of the [[camera]]in [[Domoticz]] :
- Interrupteurs / modifier
- Type : Motion Sensor
- Délai d'extinction : 5
- Action On : (http://192.168.0.162/cm?cmnd=Power%20On)
- Action On : (http://192.168.0.162/cm?cmnd=Power%20Off)
## Liens
[[DOMOTIQUE]] [[Domoticz]] [[camera]] [[interrupteur]]