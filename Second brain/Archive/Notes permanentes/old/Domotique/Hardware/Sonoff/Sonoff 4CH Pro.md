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
# Sonoff 4CH Pro
## Flasher un Sonoff 4CH Pro avec Tasmota

Source : (https://projetsdiy.fr/hack-sonoff-4ch-pro-firmware-mqtt-tasmota-inclusion-domoticz/)

- Souder les connecteurs dupont femelle
  Comme indiqué ici :
  ![[sonoff-4chpro-01-connecteurs.jpg]]

- Relier GND au GPIO0, brancher par l'alim DC, ne relacher GPIO0 qu'après 2 sec
  La LED bleue (WIFI) ne doit pas s'allumer, signe que le Sonoff est en mode flashage
  Emplacement du GPIO0 :
![[sonoff-4chpro-02.jpg]]

- Brancher FTDI sur l'USB du PC, avec les 3 broches dupont GND,TX,RX
  GND sur GND
  RX sur TX
  TX sur RX
  Sur certains modèles, RX va sur RX et TX va sur TX
  Connexions :
  ![[sonoff-4chpro-03.jpg]]

- Download le firmware tasmota-FR.bin
  Source : (https://github.com/arendst/Tasmota/releases/)

- Flasher
  ```bash
  $ sudo apt-get install esptool
  $ sudo esptool --baud 115200 --after no_reset write_flash --flash_mode dout 0x00000 tasmota-FR.bin
  ```
## Liens
[[DOMOTIQUE]] [[electronique]] [[interrupteur]] [[Domoticz]] [[Modules Sonoff]] [[esp32]] [[Tasmota]]