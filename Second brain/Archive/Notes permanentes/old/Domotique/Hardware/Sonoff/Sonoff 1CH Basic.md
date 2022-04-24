---
alias:
metadata: 02
author: AUGST-MERELLE Alexandra
type: howto
status: ready
keywords: sonoff, hardware
creation: 2021-06-27
modification: 2021-06-27
---
 | 
------------ | ------------
MOC | [[DOMOTIQUE]]
Project | [[Domotique (Projet)]]
Template | [[Archive/Notes permanentes]]
Source | [[AUGST-MERELLE Alexandra]]
# Sonoff 1CH Basic
## Flasher un Sonoff 1CH Basic avec Tasmota
- Souder les connecteurs dupont femelle
  Comme indiqué ici : sonoff-1chbasic-01-connecteurs.jpg

- Brancher l'interface USB to TTL au Sonoff (mais pas au PC)
  Comme indiqué ici :
![[sonoff-1chbasic-01-connecteurs.jpg]]

- Maintenir l'interrupteur enfoncé, brancher l'USB-TTL dans le PC,
  relacher l'interrupteur

- Download le firmware tasmota-FR.bin
  Source : (https://github.com/arendst/Tasmota/releases/)

- Flasher
```bash
$ sudo apt-get install esptool
$ sudo esptool --baud 115200 --after no_reset write_flash --flash_mode dout 0x00000 tasmota-FR.bin
```
## Liens
[[DOMOTIQUE]] [[electronique]] [[interrupteur]] [[Domoticz]] [[Modules Sonoff]] [[esp32]] [[Tasmota]]