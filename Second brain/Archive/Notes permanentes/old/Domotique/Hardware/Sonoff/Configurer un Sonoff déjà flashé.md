---
alias:
metadata: 02
author: AUGST-MERELLE Alexandra
type: howto
status: ready
keywords: sonoff, config
creation: 2021-06-27
modification: 2021-06-27
---
 | 
------------ | ------------
MOC | [[DOMOTIQUE]]
Project | [[Domotique (Projet)]]
Template | [[Archive/Notes permanentes]]
Source | [[AUGST-MERELLE Alexandra]]
# Config Sonoff déja [[flashé]]
## Configurer un Sonoff déja flashé
Modules [[Sonoff 1CH Basic]], [[Sonoff 4CH Pro]], [[Sonoff 4CH R3]], [[Sonoff IT T0EU3C]]
- Brancher le Sonoff flashé
- Son réseau wifi apparait (eg : tasmota_435DC8-7694)
- Se connecter sur son wifi
- Navigateur sur URL : (http://192.168.4.1)
- Renseigner SSID et mot de passe wifi, enregistrer
- Déclarer son IP dans le routeur et /etc/hosts
- Navigateur sur sa nouvelle URL
- Configuration / Configuration du module
  - Pour [[Sonoff 4CH Pro]]
    Type de module : Sonoff 4CH Pro, enregistrer
  - Pour [[Sonoff IT T0EU3C]] :
    Type de module : Sonoff T1 3CH, enregistrer
- Configuration [[MQTT]]
- Configuration [[Domoticz]]
  Reporter l'idx
## Liens
[[DOMOTIQUE]] [[electronique]] [[interrupteur]] [[Domoticz]] [[esp32]] [[Tasmota]]