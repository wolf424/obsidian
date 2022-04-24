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
# Sonoff IT T0EU3C
## Flasher un Sonoff 4CH Pro avec Tasmota
- Ne pas alimenter en 220V

- Relier les 4 connecteurs de droite (VCC, GND, TX, RX) à l'USB-TTL

- Maintenir Relié le GND de gauche à R19 (en haut vers la gauche) puis brancher l'USB-TTL dans le PC

- On peut maintenant retirer le cable de R19

- Download le firmware tasmota-FR.bin
  Source : (https://github.com/arendst/Tasmota/releases/)

- Flasher
  ```bash
  $ sudo apt-get install esptool
  $ sudo esptool --baud 115200 --after no_reset write_flash --flash_mode dout 0x00000 tasmota-FR.bin
  ```
## Liens
[[DOMOTIQUE]] [[electronique]] [[interrupteur]] [[Domoticz]] [[Modules Sonoff]] [[esp32]] [[Tasmota]]