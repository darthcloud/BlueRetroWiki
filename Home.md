# BlueRetro User Manual

# Table of contents
* [Building hardware](#building-hardware)
* [System Specific User Manual](#system-specific-user-manual)
* [ESP32 buttons usage](#esp32-buttons-usage)
* [LED usage](#led-usage-io17)
* [Updating firmware](#updating-firmware)
* [Web config](#web-config)
* [Pairing Bluetooth controller](#pairing-bluetooth-controller)
* [Getting BlueRetro debug logs](#getting-blueretro-debug-logs)

# Building hardware

* [DIY ESP32 module flashing & wiring instructions](BlueRetro-DIY-Build-Instructions)
* [BlueRetro Cables Build Instructions](BlueRetro-Cables-Build-Instructions)
* [BlueRetro Consolize system](BlueRetro-Consolize-Build-Instructions)
* [SNES Mini internal install](BlueRetro-SNES-Mini-Internal-Install)

# System Specific User Manual

[System Specific User Manual](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-System-Specific-User-Manual)

# ESP32 buttons usage

* BOOT:
  * Short press (outside BT inquiry mode): Disconnect all Bluetooth devices from the adapter.
  * Short press (BT inquiry mode): Cancel Bluetooth inquiry mode (new pairing).
  * 3 sec hold: Enable Bluetooth inquiry mode (new pairing).
  * 10 sec hold: Factory reset BlueRetro to default configuration and clear BT pairing keys.
* EN: Reboot BlueRetro.

# LED usage (IO17)

* Solid: An error occured, try power cycle, check serial logs for detail.
* Pulsing: Bluetooth inquiry mode enable (new pairing).
* Off: No error and Bluetooth inquiry mode disabled.

# Updating firmware
**Once flashed via OTA Web interface, FW flashed via USB won't be loaded anymore until the adapter is factory reset. (See [ESP32 buttons usage](#esp32-buttons-usage))**

Download latest binary from [GitHub](https://github.com/darthcloud/BlueRetro/releases) and flash them on your BlueRetro.\
\
Only internal flash (SPIFFS) firmware are now supported. An universal version with system auto detection is provided in addition to system hard-coded versions.

## Via USB serial

* Linux:\
`~/BlueRetroRoot/python_env/idf4.2_py3.7_env/bin/python ~/BlueRetroRoot/esp-idf/components/esptool_py/esptool/esptool.py -p /dev/ttyUSB0 -b 460800 --before default_reset --after hard_reset --chip esp32  write_flash --flash_mode dio --flash_size detect --flash_freq 40m 0x1000 bootloader.bin 0x8000 partition-table.bin 0x10000 BlueRetro.bin`\

* Windows:\
[Flashing firmware Windows 10](https://github.com/darthcloud/BlueRetro/wiki/Flashing-firmware-Windows-10)

## Via Web-Bluetooth interface (OTA FW update)

**Required FW v0.19 minimum to be already programmed via USB serial**

1. Go to https://blueretro.io/ota.html and connect to your BlueRetro adapter (make sure it's powered on and no controller connected).
2. Select the BlueRetro\*.bin you want then click Update Firmware button.
3. Via PC Chrome update should take around 5 minutes, with Android Chrome it will take around 45 minutes (!!!).

# Web config

Power on system and connect via Web Bluetooth at https://blueretro.io to configure adapter.\
**The config mode is only available if no controller is connected.** \
**Supported only in Desktop or Android Chrome**

# Pairing Bluetooth controller

In default configuration BlueRetro is always in inquiry mode (LED pulsing) if no controller is connected\
Pair via inquiry first (SYNC or pairing mode), on subsequent connection you can simply page (button press or power on button).\
You may change this behavior by switching inquiry mode in the web config to manual.
Pressing BOOT buttons for 3 sec will activate inquiry mode.
See guide for more specific instruction: [Pairing Guide](https://github.com/darthcloud/BlueRetro/wiki/Controller-pairing-guide)

Up to 16 connection keys for classic BT and also up to 16 keys for BLE devices can be stored for persistent pairing.

# Getting BlueRetro debug logs

See [Getting BlueRetro debug logs via Serial port Windows 10](https://github.com/darthcloud/BlueRetro/wiki/Getting-BlueRetro-debug-logs-via-Serial-port-Windows-10)
