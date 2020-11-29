# Table of contents
* [Auto Parallel 1P](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-System-Specific-User-Manual#auto-parallel-1p-6-buttons)
* [Parallel 1P](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-System-Specific-User-Manual#parallel-1p-12-buttons)
* [Parallel 2P](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-System-Specific-User-Manual#parallel-2p-6-buttons-each)
* [NES](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-System-Specific-User-Manual#nes)
* [Genesis](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-System-Specific-User-Manual#genesis)
* [SNES](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-System-Specific-User-Manual#snes)
* [PSX/PS2](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-System-Specific-User-Manual#psx-ps2)
* [Saturn](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-System-Specific-User-Manual#saturn)
* [JVS](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-System-Specific-User-Manual#jvs)
* [Nintendo 64](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-System-Specific-User-Manual#nintendo-64)
* [Dreamcast](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-System-Specific-User-Manual#dreamcast)
* [GameCube](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-System-Specific-User-Manual#gamecube)

# Auto Parallel 1P (6 buttons)

## System Config
While in Auto mode trying to detect another system, BlueRetro will output a limited 1 player 6 buttons parallel output matching the SEGA Master System cable pinout.
This allow 1P game on Atari 2600, Master System, etc. without having to switch to Parallel 2P (6 buttons each) mode.

## Multitap Config
Multitap config has no effect.

## Output Config

### Mode
Mode config has no effect.

### Accessories
Accessories config has no effect.

## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vRln_dhkahEIhq4FQY_p461r5qvLn-Hkl89ZtfyIOGAqdnPtQZ5Ihfsjvd94fRbaHX8wU3F-r2ODYbM/pubhtml) for Bluetooth controller & Parallel 1P buttons label correspondence (Refer to the Master System column).

# Parallel 1P (12 buttons)

## System Config
It is required to set System to Parallel_1P in the global config and power cycle BlueRetro. Parallel 1P (12 buttons) mode can't be auto-detected.

## Multitap Config
Multitap config has no effect.

## Output Config

### Mode
Mode config has no effect.

### Accessories
Accessories config has no effect.

## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vRln_dhkahEIhq4FQY_p461r5qvLn-Hkl89ZtfyIOGAqdnPtQZ5Ihfsjvd94fRbaHX8wU3F-r2ODYbM/pubhtml) for Bluetooth controller & Parallel 1P buttons label correspondence (Refer to the NeoGeo column).

# Parallel 2P (6 buttons each)

## System Config
It is required to set System to Parallel_2P in the global config and power cycle BlueRetro. Parallel 2P (6 buttons each) mode can't be auto-detected.

## Multitap Config
Multitap config has no effect.

## Output Config

### Mode
Mode config has no effect.

### Accessories
Accessories config has no effect.

## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vRln_dhkahEIhq4FQY_p461r5qvLn-Hkl89ZtfyIOGAqdnPtQZ5Ihfsjvd94fRbaHX8wU3F-r2ODYbM/pubhtml) for Bluetooth controller & Parallel 2P buttons label correspondence (Refer to the Master System column).

# NES

## Multitap Config
* **None**: BlueRetro will emulate the device selected in output config #1 on NES port 1.\
  BlueRetro will emulate the device selected in output config #2 on NES port 2.
* **Slot 1**: Same as Dual.
* **Slot 2**: Same as Dual.
* **Dual**: BlueRetro will emulate a Four Score multitap with 4 controllers (Use both NES ports).
* **Alt**: BlueRetro will emulate a Japanese 4P adapter multitap with 4 controllers (Use both NES ports & FC DB15).

## Output Config

### Mode
* **GamePad**: BlueRetro will emulate a standard 8 buttons NES controller.
* **GamePadAlt**: Same as GamePad.
* **Keyboard**: **TBD** ~~BlueRetro will emulate a Famicom keyboard.~~
* **Mouse**: **TBD** ~~BlueRetro will emulate a Famicom Hori Trackball.~~

### Accessories
Accessories config has no effect.

## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vRln_dhkahEIhq4FQY_p461r5qvLn-Hkl89ZtfyIOGAqdnPtQZ5Ihfsjvd94fRbaHX8wU3F-r2ODYbM/pubhtml) for Bluetooth controller & NES controller buttons label correspondence.

# Genesis

## Multitap Config
* **None**: BlueRetro will emulate the device selected in output config #1 on Genesis port 1.\
  BlueRetro will emulate the device selected in output config #2 on Genesis port 2.
* **Slot 1**: BlueRetro will emulate a Genesis Team Player Multitap with 4 devices on port 1 as configured in output config #1-4.\
  BlueRetro will emulate the device selected in output config #5 on Genesis port 2.
* **Slot 2**: BlueRetro will emulate the device selected in output config #1 on Genesis port 1.\
  BlueRetro will emulate a Genesis Team Player Multitap with 4 devices on port 2 as configured in output config #2-5.
* **Dual**: BlueRetro will emulate a Genesis Team Player Multitap with 4 devices on port 1 & 2 (Total 8 devices) as configured in output config #1-8.
* **Alt**: BlueRetro will emulate a EA 4 Way Play multitap with 4 3 buttons controllers (Use both Genesis ports).

## Output Config

### Mode
* **GamePad**: BlueRetro will emulate a standard 3 buttons controller.
* **GamePadAlt**: BlueRetro will emulate a 6 buttons controller.
* **Keyboard**: **TBD** ~~BlueRetro will emulate a XBAND Keyboard. (Not supported for multitap)~~
* **Mouse**: **TBD** ~~BlueRetro will emulate a Genesis Mouse.~~

### Accessories
Accessories config has no effect.

## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vRln_dhkahEIhq4FQY_p461r5qvLn-Hkl89ZtfyIOGAqdnPtQZ5Ihfsjvd94fRbaHX8wU3F-r2ODYbM/pubhtml) for Bluetooth controller & Genesis controller buttons label correspondence.

# SNES

## Multitap Config
* **None**: BlueRetro will emulate the device selected in output config #1 on SNES port 1.\
  BlueRetro will emulate the device selected in output config #2 on SNES port 2.
* **Slot 1**: **TBD** ~~BlueRetro will emulate a Super Multitap with 4 controllers on port 1.~~\
  ~~BlueRetro will emulate the device selected in output config #5 on SNES port 2.~~
* **Slot 2**: BlueRetro will emulate the device selected in output config #1 on SNES port 1.\
  BlueRetro will emulate a Super Multitap with 4 controllers on port 2.
* **Dual**: **TBD** ~~BlueRetro will emulate a Super Multitap with 4 controllers on port 1 & 2 (Total 8 controllers).~~
* **Alt**: NA

## Output Config

### Mode
* **GamePad**: BlueRetro will emulate a standard 12 buttons SNES controller.
* **GamePadAlt**: Same as GamePad.
* **Keyboard**: **TBD** ~~BlueRetro will emulate a XBAND keyboard.~~
* **Mouse**: **TBD** ~~BlueRetro will emulate a SNES Mouse.~~

### Accessories
Accessories config has no effect.

## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vRln_dhkahEIhq4FQY_p461r5qvLn-Hkl89ZtfyIOGAqdnPtQZ5Ihfsjvd94fRbaHX8wU3F-r2ODYbM/pubhtml) for Bluetooth controller & SNES controller buttons label correspondence.

# PSX/PS2

## Multitap Config
* **None**: BlueRetro will emulate the device selected in output config #1 on PSX/PS2 port 1.\
  BlueRetro will emulate the device selected in output config #2 on PSX/PS2 port 2.
* **Slot 1**: BlueRetro will emulate a PSX/PS2 Multitap with 4 devices on port 1 as configured in output config #1-4.\
  BlueRetro will emulate the device selected in output config #5 on PSX/PS2 port 2.
* **Slot 2**: BlueRetro will emulate the device selected in output config #1 on PSX/PS2 port 1.\
  BlueRetro will emulate a PSX/PS2 Multitap with 4 devices on port 2 as configured in output config #2-5.
* **Dual**: BlueRetro will emulate a PSX/PS2 Multitap with 4 devices on port 1 & 2 (Total 8 devices) as configured in output config #1-8.
* **Alt**: NA

## Output Config

### Mode
* **GamePad**: BlueRetro will emulate a DualShock 2 controller.
* **GamePadAlt**: **TBD** ~~BlueRetro will emulate a Flightstick.~~
* **Keyboard**: **TBD** ~~BlueRetro will emulate a Lightspan Keyboard.~~
* **Mouse**: BlueRetro will emulate a PSX Mouse. (Must use "Default Mouse" preset)

### Accessories
Accessories config has no effect.

## Mapping
A regular Saturn Analog controller report it's Triggers both as analog and digital.
* Using the default mapping, BlueRetro will report triggers as analog only.
* Use the "Saturn Merge analog & digital trigger" preset to match the real Saturn Analog controller behavior.

See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vRln_dhkahEIhq4FQY_p461r5qvLn-Hkl89ZtfyIOGAqdnPtQZ5Ihfsjvd94fRbaHX8wU3F-r2ODYbM/pubhtml) for Bluetooth controller & Saturn controller buttons label correspondence.

# Saturn

## Multitap Config
* **None**: BlueRetro will emulate the device selected in output config #1 on Saturn port 1.\
  BlueRetro will emulate the device selected in output config #2 on Saturn port 2.
* **Slot 1**: BlueRetro will emulate a Saturn Multitap with 6 devices on port 1 as configured in output config #1-6.\
  BlueRetro will emulate the device selected in output config #7 on Saturn port 2.
* **Slot 2**: BlueRetro will emulate the device selected in output config #1 on Saturn port 1.\
  BlueRetro will emulate a Saturn Multitap with 6 devices on port 2 as configured in output config #2-7.
* **Dual**: BlueRetro will emulate a Saturn Multitap with 6 devices on port 1 & 2 (Total 12 devices) as configured in output config #1-12.
* **Alt**: NA

## Output Config

### Mode
* **GamePad**: BlueRetro will emulate an Analog controller in **Digital** mode.
* **GamePadAlt**: BlueRetro will emulate an Analog controller in **Analog** mode.
* **Keyboard**: **TBD** ~~BlueRetro will emulate a Saturn Keyboard.~~
* **Mouse**: **TBD** ~~BlueRetro will emulate a Saturn Mouse.~~

### Accessories
Accessories config has no effect.

## Mapping
A regular Saturn Analog controller report it's Triggers both as analog and digital.
* Using the default mapping, BlueRetro will report triggers as analog only.
* Use the "Saturn Merge analog & digital trigger" preset to match the real Saturn Analog controller behavior.

See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vRln_dhkahEIhq4FQY_p461r5qvLn-Hkl89ZtfyIOGAqdnPtQZ5Ihfsjvd94fRbaHX8wU3F-r2ODYbM/pubhtml) for Bluetooth controller & Saturn controller buttons label correspondence.

# JVS
BlueRetro will emulate a 12 players output with 16 buttons and 2 axis each.

## Multitap Config
Multitap config has no effect.

## Output Config

### Mode
Mode config has no effect.

### Accessories
Accessories config has no effect.

## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vRln_dhkahEIhq4FQY_p461r5qvLn-Hkl89ZtfyIOGAqdnPtQZ5Ihfsjvd94fRbaHX8wU3F-r2ODYbM/pubhtml) for Bluetooth controller & JVS controller buttons label correspondence.

# Nintendo 64
BlueRetro will emulate the device selected in output config #1 on N64 port 1.\
BlueRetro will emulate the device selected in output config #2 on N64 port 2. \
BlueRetro will emulate the device selected in output config #3 on N64 port 3. \
BlueRetro will emulate the device selected in output config #4 on N64 port 4.

## Multitap Config
Multitap config has no effect.

## Output Config

### Mode
* **GamePad**: BlueRetro will emulate a standard N64 controller.
* **GamePadAlt**: Same as GamePad.
* **Keyboard**: BlueRetro will emulate a Randnet Keyboard. (Must use "Default Gamepad/Keyboard" preset)
* **Mouse**: BlueRetro will emulate a N64 Mouse. (Must use "Default Mouse" preset)

### Accessories
**Only valid for "Gamepad" mode.**
* **None**: BlueRetro will emulate a standard N64 controller with empty accessory slot.
* **Memory**: **TBD** ~~BlueRetro will emulate a standard N64 controller with Controller Pak.~~
* **Rumble**: BlueRetro will emulate a standard N64 controller with Rumble Pak.
* **Both**: NA

## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vRln_dhkahEIhq4FQY_p461r5qvLn-Hkl89ZtfyIOGAqdnPtQZ5Ihfsjvd94fRbaHX8wU3F-r2ODYbM/pubhtml) for Bluetooth controller & N64 controller buttons label correspondence.

# Dreamcast
BlueRetro will emulate the device selected in output config #1 on Dreamcast port 1.\
BlueRetro will emulate the device selected in output config #2 on Dreamcast port 2. \
BlueRetro will emulate the device selected in output config #3 on Dreamcast port 3. \
BlueRetro will emulate the device selected in output config #4 on Dreamcast port 4.

## Multitap Config
Multitap config has no effect.

## Output Config

### Mode
* **GamePad**: BlueRetro will emulate a standard Dreamcast controller.
* **GamePadAlt**: BlueRetro will emulate a non-standard Dreamcast controller with 2nd Joystick, 2nd D-pad & C, D & Z buttons.
* **Keyboard**: BlueRetro will emulate a Dreamcast Keyboard. (Must use "Default Gamepad/Keyboard" preset)
* **Mouse**: BlueRetro will emulate a Dreamcast Mouse. (Must use "Default Mouse" preset)

### Accessories
**Only valid for "Gamepad" & "GamePadAlt" mode.**
* **None**: BlueRetro will emulate a Dreamcast controller with 2 empty accessory slots
* **Memory**: **TBD** ~~BlueRetro will emulate a Dreamcast controller with VMU.~~
* **Rumble**: BlueRetro will emulate a Dreamcast controller with Jump Pack. **Experimental**
* **Both**: **TBD** ~~BlueRetro will emulate a Dreamcast controller with VMU & Jump Pack.~~

## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vRln_dhkahEIhq4FQY_p461r5qvLn-Hkl89ZtfyIOGAqdnPtQZ5Ihfsjvd94fRbaHX8wU3F-r2ODYbM/pubhtml) for Bluetooth controller & Dreamcast controller buttons label correspondence.

# GameCube
BlueRetro will emulate the device selected in output config #1 on GameCube port 1.\
BlueRetro will emulate the device selected in output config #2 on GameCube port 2. \
BlueRetro will emulate the device selected in output config #3 on GameCube port 3. \
BlueRetro will emulate the device selected in output config #4 on GameCube port 4.

## Multitap Config
Multitap config has no effect.

## Output Config

### Mode
* **GamePad**: BlueRetro will emulate a standard GameCube controller.
* **GamePadAlt**: Same as GamePad.
* **Keyboard**: BlueRetro will emulate a ASCII/Sammy Keyboard. (Must use "Default Gamepad/Keyboard" preset)
* **Mouse**: NA

### Accessories
**Only valid for "Gamepad" mode.**
* **None**: BlueRetro will emulate a standard GameCube controller with rumble disabled.
* **Memory**: NA
* **Rumble**: BlueRetro will emulate a standard GameCube controller with rumble enable.
* **Both**: NA

## Mapping
A regular Gamecube controller trigger is composed of two buttons: the analog section and a digital buttons at the end.
Wii Original Classic controller and **TBD** ~~Steam controller~~ work this way. Those two controller will emulate the GameCube mapping properly using default config.
* Using the default mapping, BlueRetro will map the two section separately. (Use this if playing with Wii Original Classic or **TBD** ~~Steam controller~~
* Use the "GameCube Merge analog & digital trigger" preset to emulate the GameCube trigger using only the analog trigger. (Any other type of Bluetooth controller)

See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vRln_dhkahEIhq4FQY_p461r5qvLn-Hkl89ZtfyIOGAqdnPtQZ5Ihfsjvd94fRbaHX8wU3F-r2ODYbM/pubhtml) for Bluetooth controller & GameCube controller buttons label correspondence.