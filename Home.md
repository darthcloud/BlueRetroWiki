Welcome to the BlueRetro wiki!

# Dev board setup
## ESP32-DevKitC V4
1. Linux only: Follow step "Dev env setup" at [BlueRetroRoot](https://github.com/darthcloud/BlueRetroRoot).

2. Download latest binary from [GitHub](https://github.com/darthcloud/BlueRetro/releases) and flash them on your ESP32.\
  Linux:\
  `~/BlueRetroRoot/python_env/idf4.2_py3.7_env/bin/python ~/BlueRetroRoot/esp-idf/components/esptool_py/esptool/esptool.py -p /dev/ttyUSB0 -b 460800 --before default_reset --after hard_reset --chip esp32  write_flash --flash_mode dio --flash_size detect --flash_freq 40m 0x1000 bootloader.bin 0x8000 partition-table.bin 0x10000 BlueRetro.bin`\
  Windows:\
  [Flashing firmware Windows 10](https://github.com/darthcloud/BlueRetro/wiki/Flashing-firmware-Windows-10)

3. Burn the flash voltage eFuses for avoiding conflict between D2 & MTDI strapping.
https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-reference/peripherals/sd_pullup_requirements.html

4. Install DB25 connector & PmodMicroSD board.
https://github.com/darthcloud/BlueRetroHW/blob/master/BlueRetro.pdf

5. Build target system cable adapter.
https://github.com/darthcloud/BlueRetroHW/blob/master/BlueRetro.pdf

6. Insert blank SD card.

7. (Optional) Power on system and connect via Web Bluetooth to configure adapter.
https://darthcloud.github.io/samples/web-bluetooth/blueretro.html
https://darthcloud.github.io/samples/web-bluetooth/blueretro_presets.html

8. Pair via inquiry first, on subsequent connection you can simply page.

## ESP-WROVER-KIT V4.1
1. Linux only: Follow step "Dev env setup" at [BlueRetroRoot](https://github.com/darthcloud/BlueRetroRoot).

2. Download latest binary from [GitHub](https://github.com/darthcloud/BlueRetro/releases) and flash them on your ESP32.\
Linux:
`~/BlueRetroRoot/python_env/idf4.2_py3.7_env/bin/python ~/BlueRetroRoot/esp-idf/components/esptool_py/esptool/esptool.py -p /dev/ttyUSB0 -b 460800 --before default_reset --after hard_reset --chip esp32  write_flash --flash_mode dio --flash_size detect --flash_freq 40m 0x1000 bootloader.bin 0x8000 partition-table.bin 0x10000 BlueRetro.bin`\
Windows:\
[Flashing firmware Windows 10](https://github.com/darthcloud/BlueRetro/wiki/Flashing-firmware-Windows-10)

3. Remove R11, R23, R134, R136, R136, R137, R138, R139, R164 & R168\
   Short R12 & R24\
   Don't short TXD and RXD0

4. Install DB25 connector
https://github.com/darthcloud/BlueRetroHW/blob/master/BlueRetro.pdf

5. Build target system cable adapter.
https://github.com/darthcloud/BlueRetroHW/blob/master/BlueRetro.pdf

6. Insert blank SD card.

7. (Optional) Power on system and connect via Web Bluetooth to configure adapter.
https://darthcloud.github.io/samples/web-bluetooth/blueretro.html
https://darthcloud.github.io/samples/web-bluetooth/blueretro_presets.html

8. Pair via inquiry first, on subsequent connection you can simply page.
