# circuitpython_vid_pid
A small collection of USB VIDs and PIDs used by circuitpython.

## Current collection

```
0D28 NXP
  0204 Arm Embed - used by Micro:bit v1
  
239A Adafruit Industries
  0018 Circuit Playground Express
  80f4 Pico
  8120 Pico W

2E8A Raspberry Pi
  0003 RP2 Boot
  00C0 RaspberryPi Pico not flashed yet
  
303A Espressif
  7003 ESP32-S3-DevKitC-1-N8R8
  80E9 | LILYGO TTGO T8 ESP32-S2-WROOM - Arduino
  80EA | LILYGO TTGO T8 ESP32-S2-WROOM - CircuitPython
  80EB | LILYGO TTGO T8 ESP32-S2-WROOM - UF2 Bootloader
  813E | LILYGO T-Display-S3 - Arduino
  813F | LILYGO T-Display-S3 - CircuitPython
  8140 | LILYGO T-Display-S3 - UF2 Bootloader
```
See:

- https://github.com/adafruit/Adafruit_Windows_Drivers/blob/main/Drivers/Adafruit_usbser/Adafruit_usbser.inf
- https://github.com/raspberrypi/usb-pid
- https://github.com/espressif/usb-pids/blob/main/allocated-pids.txt
 

## Output from lsusb

```
Bus 000 Device 002: ID 303a:7003 303a ESP32-S3-DevKitC-1-N8R8  Serial: 4F21AF2E840E
Bus 000 Device 000: ID 303a:7003 303a USB 3.1 Bus 
Bus 000 Device 001: ID 1d6b:0003 Linux Foundation 3.0 root hub 
(base) mk@mbp ~ % lsusb
Bus 000 Device 002: ID 303a:7003 303a ESP32-S3-DevKitC-1-N8R8  Serial: 4F21AF2E840E
Bus 001 Device 001: ID 2e8a:00c0 2e8a RaspberryPi Pico  Serial: 086461E62C5A7243
Bus 000 Device 000: ID 303a:7003 303a USB 3.1 Bus 
Bus 000 Device 000: ID 2e8a:00c0 2e8a USB 3.1 Bus 
(base) mk@mbp ~ % lsusb
Bus 001 Device 001: ID 2e8a:00c0 2e8a RaspberryPi Pico  Serial: 086461E62C5A7243
Bus 000 Device 000: ID 2e8a:00c0 2e8a USB 3.1 Bus 
(base) mk@mbp ~ % lsusb
Bus 001 Device 001: ID 2e8a:0003 2e8a RP2 Boot  Serial: E0C9125B0D9B
Bus 000 Device 000: ID 2e8a:0003 2e8a USB 3.1 Bus 
(base) mk@mbp ~ % lsusb
Bus 001 Device 001: ID 239a:80f4 239a Pico  Serial: E661640843725A2C
Bus 000 Device 000: ID 239a:80f4 239a USB 3.1 Bus 
(base) mk@mbp ~ % lsusb
Bus 001 Device 001: ID 239a:8120 239a Pico W  Serial: E661640843725A2C
Bus 000 Device 000: ID 239a:8120 239a USB 3.1 Bus 
```
