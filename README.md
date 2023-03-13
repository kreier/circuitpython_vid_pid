# circuitpython_vid_pid
A small collection of USB VIDs and PIDs used by [circuitpython](https://github.com/adafruit/circuitpython).

## Current collection

```
0D28 NXP
  0204 Arm Embed - used by Micro:bit v1 "BBC micro:bit CMSIS-DAP"
  
239A Adafruit Industries
  006a Blackpill SSIS edition
  8019 CircuitPlayground Express
  8023 Feather M0 Express 
  8046 Circuit Playground Bluefruit
  80f4 Pico
  8120 Pico W
  d1ed HalloWing M0 Express

2E8A Raspberry Pi
  0003 RP2 Boot
  000A PicoArduino - Lilygo T-PicoC3 after boot
  00C0 RaspberryPi Pico not flashed yet
  
303A Espressif
  7003 ESP32-S3-DevKitC-1-N8R8
  8007 TTGO T8 ESP32-S2 - Circuitpython with display (tested)
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
mk@mbp ~ % lsusb
Bus 000 Device 002: ID 303a:7003 303a ESP32-S3-DevKitC-1-N8R8  Serial: 4F21AF2E840E
Bus 001 Device 001: ID 2e8a:00c0 2e8a RaspberryPi Pico  Serial: 086461E62C5A7243
Bus 001 Device 001: ID 2e8a:0003 2e8a RP2 Boot  Serial: E0C9125B0D9B
Bus 001 Device 001: ID 239a:80f4 239a Pico  Serial: E661640843725A2C
Bus 001 Device 001: ID 239a:8120 239a Pico W  Serial: E661640843725A2C
Bus 000 Device 001: ID 0d28:0204 0d28 "BBC micro:bit CMSIS-DAP"  Serial: 9900000048154e4500649016000000380000000097969901
Bus 000 Device 001: ID 239a:8019 239a CircuitPlayground Express  Serial: 9DAF57C53152525020312E39111117FF
Bus 000 Device 001: ID 239a:8046 239a Circuit Playground Bluefruit  Serial: 1BE13AEBECCD3905
Bus 000 Device 001: ID 239a:8019 239a CircuitPlayground Express  Serial: 9DAF57C53152525020312E39111117FF
Bus 000 Device 001: ID 239a:d1ed 239a HalloWing M0 Express  Serial: 31A1308C4C31505120204A4A381808FF
Bus 000 Device 001: ID 239a:8023 239a Feather M0 Express  Serial: C178485A4E514E5020202034233619FF
Bus 001 Device 001: ID 303a:8007 303a TTGO T8 ESP32-S2  Serial: 487F30C709A0
Bus 001 Device 001: ID 239a:006a 239a Blackpill SSIS edition  Serial: 0F004C000F51393235343934
Bus 000 Device 000: ID 239a:8046 239a USB 3.1 Bus 
Bus 000 Device 001: ID 1d6b:0003 Linux Foundation 3.0 root hub 
```
