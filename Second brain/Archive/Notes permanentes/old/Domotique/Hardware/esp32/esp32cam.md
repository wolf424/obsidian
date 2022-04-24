---
alias:
metadata: 02
author: AUGST-MERELLE Alexandra
type: article
status: ready
keywords: hardware, esp32, caméra
creation: 2021-06-27
modification: 2021-11-07
---
 | 
------------ | ------------
MOC | [[DOMOTIQUE]]
Project | [[Domotique (Projet)]]
Template | [[Archive/Notes permanentes]]
Source | [[AUGST-MERELLE Alexandra]]
# esp32cam
## Dans Arduino
Type de carte : ESP32 Wrover Module
Partition scheme : Huge APP (3M No OTA/1MB SPIFFS)
Upload speed : 115200
## Flashage [[Tasmota]]
[[Caméra]] sur [[esp32]] flashable avec [[Tasmota]]
- Logiciel de [[flashage]] : [[ESPHome-Flasher]]
- Le [[Firmware]] : tasmota32-webcam.bin
  Source : https://ota.tasmota.com/tasmota32/release/tasmota32-webcam.bin

- Plug ESP32 Camera (usb)

- Run ESPHome-Flasher-1.3.0-Ubuntu-x64.exec
  - Keep the camera shield pluged
  - Select serial port
  - Firmware : choose tasmota32-webcam.bin
  - Flash ESP
  - WIFI and IP appears on log. Example :
```[22:01:06]00:00:01.096 HTP: Web server active on tasmota_C7C73C-1852 with IP address 192.168.4.1```
  - Connect to this IP within this wifi
  - Configure wifi SSID and password
  - Declare ESP32CAM on the router and in /etc/hosts

- Go on the ESP32 camera IP adress in a http brower
  - Configure
  - Configure other
  - In template, replace text by :
```
{"NAME":"AITHINKER CAM","GPIO":[4992,1,672,1,416,5088,1,1,1,6720,736,704,1,1,5089,5090,0,5091,5184,5152,0,5120,5024,5056,0,0,0,0,4928,576,5094,5095,5092,0,0,5093],"FLAG":0,"BASE":2}

Another one:
{« NAME »: »TasmotaCAM », »GPIO »:[1,1,1,1,4992,5120,1,1,1,5089,5090,64,1,1,5024,65,0,640,608,5056,0,5184,1,5152,0,0,0,0,1,1,5088,5091,5095,5094,5093,5092], »FLAG »:0, »BASE »:1}
```
  - Check Activate
  - Save
  - In Configure / Configure module / Module type, choose AITHINKER CAM
## Auto-enabling the webcam server at boot
- Go to the ESP32-cam webUI and then **Console**.
```
Rule1 ON System#Boot DO WcInit END
```
- To enable `Rule1`, enter the following command:
```
Rule1 1
```
- Restart the ESP32-cam with the following command:
```
Restart 1
```
## RTSP server
- Navigate to the ESP32-cam webUI and then go to the **Console**.
- **Enable the RTSP server** by entering the following command:
```
WcRtsp 1
```
- Now, the video stream should be accessible via RTSP using the following address:
```
rtsp://DEVICE_IP:8554/mjpeg/1
```
## Resolution
- to set the stream resolution to 480x320, go to the **Console** and enter the following command :
```
WcResolution 7
```

## Commands
Command
- `Wc` : Displays all the current webcam settings
- `WcBrightness` Image brightness
`-2`, `-1`, `0`, `1`, `2`
- `WcContrast` : Image contrast
`-2`, `-1`, `0`, `1`, `2`
- `WCFlip` : Flips the image vertically
`1`, `0`
- `WcInit` : Initializes the HTTP webcam server
- `WCMirror` : Flips the image horizontally
`1`, `0`
- `WcRtsp` : RTSP server
`0`: disable, `1`: enable
- `WcSaturation` : Image saturation
`-2`, `-1`, `0`, `1`, `2`
- `WcStream` : Controls the video streaming
`0`: stop, `1`: start
### Resolution
- `WcResolution` : Image resolution
`0`: `FRAMESIZE 96x96`
`1`: `FRAMESIZE 160x120`
`2`: `FRAMESIZE 176x144`
`3`: `FRAMESIZE 240x176`
`4`: `FRAMESIZE 240x240`
`5`: `FRAMESIZE 320x240`
`6`: `FRAMESIZE 400x256`
`7`: `FRAMESIZE 480x320`
`8`: `FRAMESIZE 640x480`
`9`: `FRAMESIZE 800x600`
`10`: `FRAMESIZE 1024x768`
`11`: `FRAMESIZE 1280x720`
`12`: `FRAMESIZE 1280x1024`
`13`: `FRAMESIZE 1600x1200`

For example, to set the stream resolution to 800x600, go to the **Console** and enter the following command :

```
WcResolution 9
```

### Commands via http
Alternatively, it’s possible to send commands via HTTP.
```
http://DEVICE_IP/cm?cmnd=WcResolution%209
```
If using a terminal, you can send via `curl`, as follows:
```
curl http://DEVICE_IP/cm?cmnd=WcResolution%209
```
## Liens
https://cgomesu.com/blog/Esp32cam-tasmota-webcam-server/
[[DOMOTIQUE]]