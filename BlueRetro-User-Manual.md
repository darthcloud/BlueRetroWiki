# Table of contents
* [System Specific User Manual](https://github.com/darthcloud/BlueRetro/wiki#system-specific-user-manual)
* [ESP32 buttons usage](https://github.com/darthcloud/BlueRetro/wiki#esp32-buttons-usage)
* [Updating firmware](https://github.com/darthcloud/BlueRetro/wiki#updating-firmware)
* [SD card format](https://github.com/darthcloud/BlueRetro/wiki#sd-card-format)
* [Web config](https://github.com/darthcloud/BlueRetro/wiki#web-config)
* [Pairing Bluetooth controller](https://github.com/darthcloud/BlueRetro/wiki#pairing-bluetooth-controller)
* [Getting BlueRetro debug logs](https://github.com/darthcloud/BlueRetro/wiki#getting-blueretro-debug-logs)
* [Building adapter cables](https://github.com/darthcloud/BlueRetro/wiki#building-adapter-cables)
# System Specific User Manual
[System Specific User Manual](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-System-Specific-User-Manual)
## ESP32 buttons usage
* BOOT: Disconnect all Bluetooth devices from the adapter.
* EN: Reboot BlueRetro.
## Updating firmware
Download latest binary from [GitHub](https://github.com/darthcloud/BlueRetro/releases) and flash them on your BlueRetro.\
\
Two types of build are now available: the SD card version as before (now named BlueRetro_universal_sd.bin) and also internal flash (SPIFFS). For each type I also provide the regular universal version with system auto detection. But in addition system hard-coded versions are available. A total of 24 variants are available.\
\
Linux:\
`~/BlueRetroRoot/python_env/idf4.2_py3.7_env/bin/python ~/BlueRetroRoot/esp-idf/components/esptool_py/esptool/esptool.py -p /dev/ttyUSB0 -b 460800 --before default_reset --after hard_reset --chip esp32  write_flash --flash_mode dio --flash_size detect --flash_freq 40m 0x1000 bootloader.bin 0x8000 partition-table.bin 0x10000 BlueRetro.bin`\
Windows:\
[Flashing firmware Windows 10](https://github.com/darthcloud/BlueRetro/wiki/Flashing-firmware-Windows-10)

# SD card format
If you use a SD card type build, insert blank SD card. BlueRetro will format the card itself.

# Web config
Power on system and connect via Web Bluetooth at https://blueretro.io to configure adapter.\
**The config mode is only available if no controller is connected.** \
**SD card is required to be able to save the settings between power cycle** \
**Supported only in Desktop or Android Chrome**

# Pairing Bluetooth controller
**SD card is required to be able to save the Bluetooth pairing keys required by some controllers for quick reconnect** \
BlueRetro is always in pairing mode if no controller connected (and stay in pairing mode for 1 minute after one device connected)\
Pair via inquiry first (SYNC or pairing mode), on subsequent connection you can simply page (button press or power on button).\
See guide for more specific instruction: [Pairing Guide](https://github.com/darthcloud/BlueRetro/wiki/Controller-pairing-guide)

# Getting BlueRetro debug logs
See [Getting BlueRetro debug logs via Serial port Windows 10](https://github.com/darthcloud/BlueRetro/wiki/Getting-BlueRetro-debug-logs-via-Serial-port-Windows-10)

# Building adapter cables
See [BlueRetro Cables Build Instructions](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-Cables-Build-Instructions)