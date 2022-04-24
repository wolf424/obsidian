---
alias:
metadata: 02
author: AUGST-MERELLE Alexandra
type: howto
status: ready
keywords: sonoff, mqtt, bash
creation: 2021-06-27
modification: 2021-06-27
---
 | 
------------ | ------------
MOC | [[DOMOTIQUE]]
Project | [[Domotique (Projet)]]
Template | [[Archive/Notes permanentes]]
Source | [[www.eclipse.org]]
## Allumer-éteindre module [[Modules Sonoff]] via [[bash]]
```bash
mosquitto_pub -h sarbecovirus -t cmnd/sonoff02/power -m "on"
mosquitto_pub -h sarbecovirus -t cmnd/sonoff02/power -m "off"
```
## Liens
[[code]] [[bash]] [[MQTT]] [[Modules Sonoff]]