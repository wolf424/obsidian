---
alias:
metadata: 02
author: AUGST-MERELLE Alexandra
type: article
status: ready
keywords: esp32, firmware
creation: 2021-06-27
modification: 2022-01-20
---
 | 
------------ | ------------
MOC | [[DOMOTIQUE]]
Project | [[Domotique (Projet)]]
Template | [[Archive/Notes permanentes]]
Source | [[AUGST-MERELLE Alexandra]]
# Tasmota
Tasmota est un [[Firmware]] libre pour [[esp32]] (et donc aussi [[Modules Sonoff|sonoff]])

## Télécharger Tasmota
(https://github.com/arendst/Tasmota/releases/tag/v9.3.1)
## Flasher Tasmota
On utilise [[esp-tool]]
## IP Statique sur Tasmota
Use Web Console and enter  
`IPAddress1 192.168.1.2`  
will do that

or use the command on [Web](https://github.com/arendst/Sonoff-Tasmota/wiki/Commands#web) line, e.g.  
`http://sonoff/cm?cmnd=IPAddress1%20192.168.1.2`
## Liens
[[DOMOTIQUE]][[esp32]]