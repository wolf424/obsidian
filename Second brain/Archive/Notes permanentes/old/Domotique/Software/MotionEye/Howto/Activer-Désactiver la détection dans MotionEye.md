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

# Activer-Désactiver la [[détection]] dans [[Motion Eye]]
## Enable/disable detection
- To enable the control port you must edit [[/etc/motioneye/motioneye.conf]] and [[/etc/motioneye/motion.conf]] and then reboot.
- In [[/etc/motioneye/motion.conf]] change "webcontrol_localhost on" to  ""webcontrol_localhost off"
- In [[/etc/motioneye/motioneye.conf]] change "motion_control_localhost true" to "motion_control_localhost false"
- Now I can pause and restart [[motion detection]] with commands from my hard wired alarm system (running on a [[Beaglebone]]) based on the alarm enable status with:
  ```bash
  curl http://picam:7999/1/detection/pause
  curl http://picam:7999/1/detection/start
  ```
  ## Liens
  [[DOMOTIQUE]] [[camera]] [[Motion Eye]]