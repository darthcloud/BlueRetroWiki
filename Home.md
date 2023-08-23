# BlueRetro's documentation

# Table of contents
* [1 - Building hardware HW1](#1---building-hardware-hw1)
* [2 - Building hardware HW2](#2---building-hardware-hw2)
* [3 - Pairing Bluetooth controller](#3---pairing-bluetooth-controller)
* [4 - Web config](#4---web-config)
  * [4.1 - System Specific Web Config User Manual](#41---system-specific-web-config-user-manual)
* [5 - Physical buttons usage](#5---physical-buttons-usage)
  * [5.1 - EN (Reset)](#51---en-reset)
  * [5.2 - BOOT (IO0) External adapter](#52---boot-io0-external-adapter)
  * [5.3 - BOOT (IO0) Internal install](#53---boot-io0-internal-install)
* [6 - Button combinations functions](#6---button-combinations-functions)
* [7 - LED usage IO17](#7---led-usage-io17)
* [8 - Updating firmware](#8---updating-firmware)
  * [8.1 - Via USB serial](#81---via-usb-serial)
  * [8.2 - Via Web-Bluetooth interface (OTA FW update)](#82---via-web-bluetooth-interface-ota-fw-update)
* [9 - BlueRetro debugging](#9---blueretro-debugging)
* [10 - BlueRetro development](#10---blueretro-development)

# 1 - Building hardware HW1
HW1 is the original BlueRetro specification and the easiest one to build yourself.
Port usage can't be detected and as such any installed controller plug on the BlueRetro
is required to be plug in the console. Unused port pin need to be wired in a stable state
as described in the cable building guide.

* [DIY ESP32 module flashing & wiring instructions](BlueRetro-DIY-Build-Instructions)
* [BlueRetro Cables Build Instructions](BlueRetro-Cables-Build-Instructions)
* [BlueRetro Consolize system](BlueRetro-Consolize-Build-Instructions)

[pmgducati](https://github.com/pmgducati) created very nice pcbs that make it very easy
to make DIY BlueRetro universal with detachable cable adapters: https://github.com/pmgducati/Blue-Retro-AIO-Units

# 2 - Building hardware HW2
HW2 specification require a lot more connection and as such is not recommended
for novice in electronic at all. HW2 main feature is active port connection detection.
This allow making internal install without intefering with wired controllers (Wired
controllers take precedance on the bus). This also allow external adapter with multiple
cable plugs to not require every plugs to be connected.

Power & Reset management are optional feature supported by HW2 aswell.

I'm not providing guide for HW2, only a specification so if you go that route I'm
expecting you known what your are doing.

If you are not sure if you should build HW1 or HW2: the answer is build HW1!

* [Internal install HW2 spec](BlueRetro-HW2-Internal-Install-Specification)
* [External adapter HW2 spec](BlueRetro-HW2-External-Specification)

[Nostalgic Indulgences](https://twitter.com/nosIndulgences) created multiple guides base on HW2 for internal install. Checkout his GitHub repo: https://github.com/nostalgic-indulgences/BlueRetro_Internal_Installation

# 3 - Pairing Bluetooth controller

In default configuration BlueRetro is always in inquiry mode (LED pulsing) if no controller is connected\
Pair via inquiry first (SYNC or pairing mode), on subsequent connection you can simply page (button press or power on button).\
You may change this behavior by switching inquiry mode in the web config to manual.\
Pressing BOOT buttons for 3 sec will activate inquiry mode.\
Up to 16 connection keys for classic BT and also up to 16 keys for BLE devices can be stored for persistent pairing.

See this list & guide for more specific instruction for each controller type:\
[Controller List & Pairing Guide](Controller-pairing-guide)

# 4 - Web config

Power on system and connect via Web Bluetooth at https://blueretro.io to configure adapter.\
**The config mode is only available if no controller is connected.** \
**Supported only in Desktop or Android Chrome**

See [BlueRetro BLE Web Config User Manual](BlueRetro-BLE-Web-Config-User-Manual) for more detail.

## 4.1 - System Specific Web Config User Manual
This page describe how the generic options of the Web Config apply to each systems supported by BlueRetro.

[System Specific Web Config User Manual](BlueRetro-System-Specific-User-Manual)

# 5 - Physical buttons usage

## 5.1 - EN (Reset)

* Reboot BlueRetro

## 5.2 - BOOT (IO0) External adapter

* Button press under < 3 sec (All LEDs solid):\
  If in pairing mode: Stop pairing mode otherwise all BT devices are disconnect.
* Button press between > 3 sec and < 6 sec (All LEDs blink slowly):\
  Start pairing mode.
* Button press between > 6 sec and < 10 sec (All LEDs blink fast):\
  Factory reset ESP32 to original BlueRetro firmware the device shipped with & reset configuration.

## 5.3 - BOOT (IO0) Internal install

### 5.3.1 - System reset behavior while ESP32 on and system on
* Button press under < 3 sec (All LEDs solid):\
  Usual system reset.
* Button press between > 3 sec and < 6 sec (All LEDs blink slowly):\
  If in pairing mode: Stop pairing mode otherwise all BT devices are disconnect.
* Button press between > 6 sec and < 10 sec (All LEDs blink fast):\
  Start pairing mode.
* Button press over > 10 sec (All LEDs blink very fast):\
  Factory reset ESP32 to original BlueRetro firmware the device shipped with & reset configuration.

### 5.3.2 - System reset behavior while ESP32 off & system off
* Holding system reset and then powering system put the ESP32 in boot (download) mode. Effectively disabling it for the current power session.

### 5.3.3 - System reset behavior while ESP32 on & system off
* System is powered on via power relay / power pin

### 5.3.4 - System reset behavior while ESP32 off and system on
* While the ESP32 is in boot mode or in deep sleep the system reset function is lost.

# 6 - Button combinations functions
Their is two forms of button combo to activate macro functions:
* Base1 + Base2 + Base3 + CommonFunction
* Base1 + Base2 + Base3 + Base4 + RestrictedFunction

The default mapping for the base buttons is as follow:
* LM (SNES L, PS L2) -> Base1
* RM (SNES R, PS R2) -> Base2
* MM (Start) -> Base3
* RB Up (SNES X, PS Triangle) -> Base4

The default mapping for the common function last button:
* RB Left (SNES Y, PS Square) -> System Reset
* RB Down (SNES B, PS X) -> System Shutdown/Controller disconnect
* RB Right (SNES A, PS Circle) -> Toggle BT pairing mode on/off

The default mapping for the restricted function last button
* D-pad Up -> Facotry Reset
* D-pad Down -> Disable BlueRetro (Deep sleep)

These default can be modified via the [advance config mapping section](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-BLE-Web-Config-User-Manual#24---mapping-config).\
Those mapping are generaly located at the end of the mapping list.\
Simply change the source button to alter the mapping of a base, common function or restricted function button.

Refer to [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vT9rPK2__komCjELFpf0UYz0cMWwvhAXgAU7C9nnwtgEaivjsh0q0xeCEiZAMA-paMrneePV7IqdX48/pubhtml) to translate BlueRetro label to specific system button names.

# 7 - LED usage (IO17)

* See [5 - Physical buttons usage](#5---physical-buttons-usage) for LED meaning while button BOOT (IO0) is pressed
* Solid: An error occured, try power cycle, check serial logs for detail.
* Pulsing: Bluetooth inquiry mode enable (new pairing).
* Off: No error and Bluetooth inquiry mode disabled.

# 8 - Updating firmware
**Once flashed via OTA Web interface, FW flashed via USB won't be loaded anymore until the adapter is factory reset. (See [5 - Physical buttons usage](https://github.com/darthcloud/BlueRetro/wiki#5---physical-buttons-usage))**

Download latest binary from [GitHub](https://github.com/darthcloud/BlueRetro/releases) and flash them on your BlueRetro.\
\
Only internal flash (SPIFFS) firmware are now supported. An universal version with system auto detection is provided in addition to system hard-coded versions.

## 8.1 - Via USB serial

* Linux:
```
esptool.py -p /dev/ttyUSB0 -b 460800 --before default_reset --after hard_reset --chip esp32  write_flash\
--flash_mode dio --flash_size detect --flash_freq 40m 0x1000 bootloader.bin 0x8000 partition-table.bin 0x10000 BlueRetro.bin
```

* Windows: [Flashing firmware Windows 10](https://github.com/darthcloud/BlueRetro/wiki/Flashing-firmware-Windows-10)

## 8.2 - Via Web-Bluetooth interface (OTA FW update)

**Required FW v0.19 minimum to be already programmed via USB serial**

1. Go to https://blueretro.io/ota.html and connect to your BlueRetro adapter (make sure it's powered on and no controller connected).
2. Select the BlueRetro\*.bin you want then click Update Firmware button.
3. Via PC Chrome update should take around 5 minutes, with Android Chrome it will take around 45 minutes (!!!).

See [OTA FW Update section](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-BLE-Web-Config-User-Manual#5---ota-fw-update-page)
of the Web config manual for a video example.

# 9 - BlueRetro debugging

* See [Getting BlueRetro debug logs via Serial port Windows 10](Getting-BlueRetro-debug-logs-via-Serial-port-Windows-10)
* See [Getting Bluetooth HCI trace with Windows 10](Bluetooth-HCI-trace-with-Win10)

# 10 - BlueRetro development

All information regarding setting up a development environment and building for BlueRetro is located in the root repo:\
https://github.com/darthcloud/BlueRetroRoot

