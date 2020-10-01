# Bill of materials
* ESP32-DEVKITC-32D or ESP32-DEVKITC-32E with ESP-WROOM-32
* DB-25 Female connector solder cup
* Digilent Pmod MicroSD
* Jumper wires (<= 2 inch)

# Build instructions
1. Linux:\
   Install [esp-idf prerequisites](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/linux-setup.html).\
   Windows:\
   Install [esp-idf prerequisites](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/windows-setup.html).
   
2. Download latest binary from [GitHub](https://github.com/darthcloud/BlueRetro/releases) and flash them on your ESP32.\
  Linux:\
  `~/BlueRetroRoot/python_env/idf4.2_py3.7_env/bin/python ~/BlueRetroRoot/esp-idf/components/esptool_py/esptool/esptool.py -p /dev/ttyUSB0 -b 460800 --before default_reset --after hard_reset --chip esp32  write_flash --flash_mode dio --flash_size detect --flash_freq 40m 0x1000 bootloader.bin 0x8000 partition-table.bin 0x10000 BlueRetro.bin`\
  Windows:\
  [Flashing firmware Windows 10](https://github.com/darthcloud/BlueRetro/wiki/Flashing-firmware-Windows-10)

3. Burn the flash voltage eFuses for avoiding conflict between D2 & MTDI strapping. (Only for WROOM or WROVER**-B** module)\
https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-reference/peripherals/sd_pullup_requirements.html#strapping-conflicts-dat2

4. Install DB25 connector & PmodMicroSD board.\
   It is important to keep the sd card jumper wire very short (<= 2 inch) and plug them directly to the ESP32 pin (not via breadboard).\
   It's critical for the 2 GND on the PMOD to be plug directly to the ESP32 GND pin via short wire!!\
https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/BlueRetroDIY.pdf

5. Build target system cable adapter.\
https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/Dreamcast.pdf
https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/GameCube.pdf
https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/N64.pdf
https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/NES.pdf
https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/SNES.pdf
https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/Saturn.pdf

6. Insert blank SD card. BlueRetro will format the card itself.

7. (Optional) Power on system and connect via Web Bluetooth to configure adapter.\
   The config mode is only available if no controller is connected. \
https://blueretro.io

8. BlueRetro is always in pairing mode if no controller connected (and stay in pairing mode for 1 minute after one device connected)\
   Pair via inquiry first (SYNC or pairing mode), on subsequent connection you can simply page (button press or power on button).
   See guide for more specific instruction: [Pairing Guide](https://github.com/darthcloud/BlueRetro/wiki/Controller-pairing-guide)