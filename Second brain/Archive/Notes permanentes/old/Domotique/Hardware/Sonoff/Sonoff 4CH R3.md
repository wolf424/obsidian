---
alias:
metadata: 02
author: AUGST-MERELLE Alexandra
type: howto
status: ready
keywords: sonoff, hardware
creation: 2022-01-19
modification: 2022-01-19
---
 | 
------------ | ------------
MOC | [[DOMOTIQUE]]
Project | [[Domotique (Projet)]]
Template | [[Archive/Notes permanentes]]
Source | [[AUGST-MERELLE Alexandra]]
# Sonoff 4CH R3
## Flasher un Sonoff 4CH R3 avec Tasmota

Source : (https://flobul-domotique.fr/flasher-le-sonoff-4ch-pro-r3/

- Souder les connecteurs dupont femelle
  Comme indiqué ici :
  ![[sonoff-4chr3-01-connecteurs.jpg]]

- Brancher FTDI sur l'USB du PC, avec les 3 broches dupont GND,TX,RX
  GND sur GND
  RX sur TX
  TX sur RX
  Sur certains modèles, RX va sur RX et TX va sur TX
  
  Passons en mode maintenance :
-   appuyez et maintenez le BP1,
-   ensuite branchez le convertisseur USB-TTL à votre ordinateur,
-   enfin relâchez le BP1.
-   Si la SLED (Sonoff 4CH R3) se met à clignoter, recommencez la procédure.


- Download le firmware tasmota-FR.bin
  Source : (https://github.com/arendst/Tasmota/releases/)

- Flasher
  ```bash
  $ sudo apt-get install esptool
  $ sudo esptool --baud 115200 --after no_reset write_flash --flash_mode dout 0x00000 tasmota-FR.bin
  ```
## Liens
[[DOMOTIQUE]] [[electronique]] [[interrupteur]] [[Domoticz]] [[Modules Sonoff]] [[esp32]] [[Tasmota]]