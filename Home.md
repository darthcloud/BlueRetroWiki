Welcome to the BlueRetro wiki!

# BlueRetro User Manual
## Table of contents
* [Updating firmware](https://github.com/darthcloud/BlueRetro/wiki#updating-firmware)
* [SD card format](https://github.com/darthcloud/BlueRetro/wiki#sd-card-format)
* [Web config](https://github.com/darthcloud/BlueRetro/wiki#web-config)
* [Pairing Bluetooth controller](https://github.com/darthcloud/BlueRetro/wiki#pairing-bluetooth-controller)
## Updating firmware
Download latest binary from [GitHub](https://github.com/darthcloud/BlueRetro/releases) and flash them on your BlueRetro.\
Linux:\
`~/BlueRetroRoot/python_env/idf4.2_py3.7_env/bin/python ~/BlueRetroRoot/esp-idf/components/esptool_py/esptool/esptool.py -p /dev/ttyUSB0 -b 460800 --before default_reset --after hard_reset --chip esp32  write_flash --flash_mode dio --flash_size detect --flash_freq 40m 0x1000 bootloader.bin 0x8000 partition-table.bin 0x10000 BlueRetro.bin`\
Windows:\
[Flashing firmware Windows 10](https://github.com/darthcloud/BlueRetro/wiki/Flashing-firmware-Windows-10)

## SD card format
Insert blank SD card. BlueRetro will format the card itself.

## Web config
Power on system and connect via Web Bluetooth to configure adapter.\
The config mode is only available if no controller is connected. \
(Supported only in Desktop or Android Chrome) \
https://blueretro.io

## Pairing Bluetooth controller
BlueRetro is always in pairing mode if no controller connected (and stay in pairing mode for 1 minute after one device connected)\
Pair via inquiry first (SYNC or pairing mode), on subsequent connection you can simply page (button press or power on button).\
See guide for more specific instruction: [Pairing Guide](https://github.com/darthcloud/BlueRetro/wiki/Controller-pairing-guide)