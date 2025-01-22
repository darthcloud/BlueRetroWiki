# Table of contents
* [Parallel 1P (NeoGeo, Supergun, JAMMA)](#parallel-1p-12-buttons)
* [Parallel 2P (Atari 2600/7800, Master System)](#parallel-2p-6-buttons-each)
* [NES](#nes)
* [PCE / TG16](#pce--tg16)
* [Genesis](#genesis)
* [SNES](#snes)
* [CD-i](#cd-i)
* [3DO](#3do)
* [Jaguar](#jaguar)
* [PSX/PS2](#psxps2)
* [Saturn](#saturn)
* [PC-FX](#pc-fx)
* [JVS](#jvs)
* [Virtual Boy](#virtual-boy)
* [Nintendo 64](#nintendo-64)
* [Dreamcast](#dreamcast)
* [GameCube](#gamecube)
* [Wii-Ext](#wii-ext)

# Parallel 1P (12 buttons)

## System Config
If using universal firmware, it is required to set System to Parallel_1P_PP or Parallel_1P_OD in the global config and power cycle BlueRetro. Parallel 1P (12 buttons) mode can't be auto-detected.

## Multitap Config
Multitap config has no effect.

## Output Config

### Mode
Mode config has no effect.

### Accessories
Accessories config has no effect.

## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vT9rPK2__komCjELFpf0UYz0cMWwvhAXgAU7C9nnwtgEaivjsh0q0xeCEiZAMA-paMrneePV7IqdX48/pubhtml) for Bluetooth controller & Parallel 1P buttons label correspondence (Refer to the NeoGeo column).

# Parallel 2P (6 buttons each)

## System Config
If using universal firmware, it is required to set System to Parallel_2P_PP or Parallel_2P_OD in the global config and power cycle BlueRetro. Parallel 2P (6 buttons each) mode can't be auto-detected.


## Multitap Config
Multitap config has no effect.

## Output Config

### Mode
Mode config has no effect.

### Accessories
Accessories config has no effect.

## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vT9rPK2__komCjELFpf0UYz0cMWwvhAXgAU7C9nnwtgEaivjsh0q0xeCEiZAMA-paMrneePV7IqdX48/pubhtml) for Bluetooth controller & Parallel 2P buttons label correspondence (Refer to the Master System column).

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
* **Keyboard**: BlueRetro will emulate a Famicom keyboard. (Must use "Default Gamepad/Keyboard" preset)
* **Mouse**: BlueRetro will emulate a Famicom Hori Trackball. (Must use "Default Mouse" preset)

Keyboard & Mouse are only supported through the Famicom expansion port.\
They both need to be configure on output #1.

### Accessories
Accessories config has no effect.

## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vT9rPK2__komCjELFpf0UYz0cMWwvhAXgAU7C9nnwtgEaivjsh0q0xeCEiZAMA-paMrneePV7IqdX48/pubhtml) for Bluetooth controller & NES controller buttons label correspondence.

### Special buttons functions
** For FC Keyboard mode only. **
* **F9 + F10**: FC Keyboard output is disabled while holding both F9+F10. (Help to navigate everdrive menu)

# PCE / TG16

## Multitap Config
* **None**: BlueRetro will emulate the device selected in output config #1.
* **Slot 1**: BlueRetro will emulate a 5 port multitap with the device selected in output config #1 on all ports.
* **Slot 2**: Same as None.
* **Dual**: Same as None.
* **Alt**: Same as None.

## Output Config

### Mode
* **GamePad**: BlueRetro will emulate a standard 2/3 buttons PCE / TG16 controller.
* **GamePadAlt**: BlueRetro will emulate a standard 6 buttons PCE / TG16 controller.
* **Keyboard**: BlueRetro will emulate a PCE Keyboard. (Must use "Default Gamepad/Keyboard" preset)
* **Mouse**: BlueRetro will emulate a PCE mouse. (Must use "Default Mouse" preset) (Not supported in multitap mode)

### Accessories
Accessories config has no effect.

## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vT9rPK2__komCjELFpf0UYz0cMWwvhAXgAU7C9nnwtgEaivjsh0q0xeCEiZAMA-paMrneePV7IqdX48/pubhtml) for Bluetooth controller & PCE/TG16 controller buttons label correspondence.

### Special buttons functions
* **MT (Home)**: Toogle wired output mode between GamePad & GamePadAlt.

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
* **Mouse**: BlueRetro will emulate a Genesis Mouse. (Must use "Default Mouse" preset)

### Accessories
Accessories config has no effect.

## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vT9rPK2__komCjELFpf0UYz0cMWwvhAXgAU7C9nnwtgEaivjsh0q0xeCEiZAMA-paMrneePV7IqdX48/pubhtml) for Bluetooth controller & Genesis controller buttons label correspondence.

### Special buttons functions
* **MT (Home)**: Toogle wired output mode between GamePad & GamePadAlt.

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
* **Mouse**: BlueRetro will emulate a SNES Mouse. (Must use "Default Mouse" preset)

### Accessories
Accessories config has no effect.

## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vT9rPK2__komCjELFpf0UYz0cMWwvhAXgAU7C9nnwtgEaivjsh0q0xeCEiZAMA-paMrneePV7IqdX48/pubhtml) for Bluetooth controller & SNES controller buttons label correspondence.

# CD-i
**External power required as CD-i look for peripheral once before BlueRetro is fully done reading it's config. Power up BlueRetro externally first, then 1 sec later power on CD-i.**

BlueRetro will emulate the device selected in output config #1 on cord 1 main device.\
BlueRetro will emulate the device selected in output config #2 on cord 2 or cord 1 secondary device. \

## Multitap Config
Multitap config has no effect.

## Output Config

### Mode
* **GamePad**: BlueRetro will emulate a standard CD-i gamepad. (Must use "CD-i gamepad" preset)
* **GamePadAlt**: NA
* **Keyboard**: BlueRetro will emulate a CD-i Keyboard. (Must use "Default Gamepad/Keyboard" preset, Accessories config select type)
* **Mouse**: BlueRetro will emulate a CD-i Mouse. (Must use "Default Mouse" preset)

### Accessories
**Only valid for "Keyboard" mode.**
* **None**: BlueRetro will emulate a "K" type keyboard.
* **Memory**:BlueRetro will emulate a "X" type keyboard.
* **Rumble**:BlueRetro will emulate a "T" type keyboard.
* **Both**: NA

## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vT9rPK2__komCjELFpf0UYz0cMWwvhAXgAU7C9nnwtgEaivjsh0q0xeCEiZAMA-paMrneePV7IqdX48/pubhtml) for Bluetooth controller & CD-i controller buttons label correspondence.

# 3DO

## Multitap Config
Multitap config has no effect.

## Output Config

### Mode
* **GamePad**: BlueRetro will emulate a standard 3DO controller.
* **GamePadAlt**: BlueRetro will emulate a 3DO Flightstick controller.
* **Keyboard**: NA
* **Mouse**: BlueRetro will emulate a 3DO Mouse.

### Accessories
Accessories config has no effect.

## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vT9rPK2__komCjELFpf0UYz0cMWwvhAXgAU7C9nnwtgEaivjsh0q0xeCEiZAMA-paMrneePV7IqdX48/pubhtml) for Bluetooth controller & 3DO controller buttons label correspondence.

### Special buttons functions
* **MT (Home)**: Toogle wired output mode between GamePad & GamePadAlt.

# Jaguar

## Multitap Config
* **None**: BlueRetro will emulate the device selected in output config #1.
* **Slot 1**: BlueRetro will emulate a 4 port TeamTap with the device selected in output config #1 on all ports.
* **Slot 2**: Same as None.
* **Dual**: Same as None.
* **Alt**: Same as None.

## Output Config

### Mode
* **GamePad**: BlueRetro will emulate a standard Jaguar controller.
* **GamePadAlt**: BlueRetro will emulate a 6D controller.
* **Keyboard**: NA
* **Mouse**: NA

### Accessories
Accessories config has no effect.

## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vT9rPK2__komCjELFpf0UYz0cMWwvhAXgAU7C9nnwtgEaivjsh0q0xeCEiZAMA-paMrneePV7IqdX48/pubhtml) for Bluetooth controller & Jaguar controller buttons label correspondence.

# PSX/PS2

## Multitap Config
** PS2 Multitap is not supported **
* **None**: BlueRetro will emulate the device selected in output config #1 on PSX/PS2 port 1.\
  BlueRetro will emulate the device selected in output config #2 on PSX/PS2 port 2.
* **Slot 1**: BlueRetro will emulate a PSX Multitap with 4 devices on port 1 as configured in output config #1-4.\
  BlueRetro will emulate the device selected in output config #5 on PSX/PS2 port 2.
* **Slot 2**: BlueRetro will emulate the device selected in output config #1 on PSX/PS2 port 1.\
  BlueRetro will emulate a PSX Multitap with 4 devices on port 2 as configured in output config #2-5.
* **Dual**: BlueRetro will emulate a PSX Multitap with 4 devices on port 1 & 2 (Total 8 devices) as configured in output config #1-8.
* **Alt**: NA

## Output Config

### Mode
* **GamePad**: BlueRetro will emulate a DualShock 2 controller.
* **GamePadAlt**: BlueRetro will emulate a Flightstick (SCPH-1110 & Green LED mode).
* **Keyboard**: BlueRetro will emulate a Lightspan Keyboard.
* **Mouse**: BlueRetro will emulate a PSX Mouse. (Must use "Default Mouse" preset)

### Accessories
**Only valid for "Gamepad" mode.**
* **None**: BlueRetro will emulate a DualShock 2 controller with rumble disabled.
* **Memory**: NA
* **Rumble**: BlueRetro will emulate a DualShock 2 controller with rumble enable.
* **Both**: NA

## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vT9rPK2__komCjELFpf0UYz0cMWwvhAXgAU7C9nnwtgEaivjsh0q0xeCEiZAMA-paMrneePV7IqdX48/pubhtml) for Bluetooth controller & PSX/PS2controller buttons label correspondence.

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
* **GamePad**: BlueRetro will emulate a 3D controller in **Digital** mode.
* **GamePadAlt**: BlueRetro will emulate a 3D controller in **Analog** mode.
* **Keyboard**: BlueRetro will emulate a Saturn Keyboard.
* **Mouse**: BlueRetro will emulate a Saturn Mouse. (Must use "Default Mouse" preset)

### Accessories
Accessories config has no effect.

## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vT9rPK2__komCjELFpf0UYz0cMWwvhAXgAU7C9nnwtgEaivjsh0q0xeCEiZAMA-paMrneePV7IqdX48/pubhtml) for Bluetooth controller & Saturn controller buttons label correspondence.

### Special buttons functions
* **MT (Home)**: Toogle wired output mode between GamePad & GamePadAlt.

## Known issues
As stated in Output Config section, BlueRetro is emulating a 3D Controller in Digital (+) or Analog (O) modes ; **GamePad** mode is not emulating a standard Saturn Controller. As such, some games incompatible with the 3D Controller will not work properly, such as Golden Axe The Duel (see [issue #995](https://github.com/darthcloud/BlueRetro/issues/995)).

# PC-FX

## Multitap Config
Multitap config has no effect.

## Output Config

### Mode
* **GamePad**: BlueRetro will emulate a standard PC-FX controller.
* **GamePadAlt**: NA
* **Keyboard**: NA
* **Mouse**: BlueRetro will emulate a PC-FX Mouse.

### Accessories
Accessories config has no effect.

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
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vT9rPK2__komCjELFpf0UYz0cMWwvhAXgAU7C9nnwtgEaivjsh0q0xeCEiZAMA-paMrneePV7IqdX48/pubhtml) for Bluetooth controller & JVS controller buttons label correspondence.

# Virtual Boy
BlueRetro will emulate a standard Virtual Boy controller.

## Multitap Config
Multitap config has no effect.

## Output Config

### Mode
Mode config has no effect.

### Accessories
Accessories config has no effect.

## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vT9rPK2__komCjELFpf0UYz0cMWwvhAXgAU7C9nnwtgEaivjsh0q0xeCEiZAMA-paMrneePV7IqdX48/pubhtml) for Bluetooth controller & Virtual Boy controller buttons label correspondence.

### Special buttons functions
* **LJ (Stick left click)**: Toggle VirtualTap video mode. (ESP IO27)
* **RJ (Stick right click)**: Change VirtualTap pallette. (ESP IO16)

# Nintendo 64
BlueRetro will emulate the device selected in output config #1 on N64 port 1.\
BlueRetro will emulate the device selected in output config #2 on N64 port 2.\
BlueRetro will emulate the device selected in output config #3 on N64 port 3.\
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
* **Memory**: BlueRetro will emulate a standard N64 controller with Controller Pak.
* **Rumble**: BlueRetro will emulate a standard N64 controller with Rumble Pak.
* **Both**: NA

## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vT9rPK2__komCjELFpf0UYz0cMWwvhAXgAU7C9nnwtgEaivjsh0q0xeCEiZAMA-paMrneePV7IqdX48/pubhtml) for Bluetooth controller & N64 controller buttons label correspondence.

### Special buttons functions
* **MT (Home)**: Toggle accessory between Controller Pak and Rumble Pak.
* **MQ (Capture/TouchPad)**: Cycle active Controller Pak bank.

# Dreamcast
BlueRetro will emulate the device selected in output config #1 on Dreamcast port 1.\
BlueRetro will emulate the device selected in output config #2 on Dreamcast port 2.\
BlueRetro will emulate the device selected in output config #3 on Dreamcast port 3.\
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
**Only valid for "Gamepad" & "GamePadAlt" mode.**\
**Only one VMU can be emulated. Set Memory/Both on only one output.**
* **None**: BlueRetro will emulate a Dreamcast controller with 2 empty accessory slots
* **Memory**: BlueRetro will emulate a Dreamcast controller with VMU.
* **Rumble**: BlueRetro will emulate a Dreamcast controller with Jump Pack. **Experimental**
* **Both**: BlueRetro will emulate a Dreamcast controller with VMU & Jump Pack.

## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vT9rPK2__komCjELFpf0UYz0cMWwvhAXgAU7C9nnwtgEaivjsh0q0xeCEiZAMA-paMrneePV7IqdX48/pubhtml) for Bluetooth controller & Dreamcast controller buttons label correspondence.

### Special buttons functions
* **MT (Home)**: Toogle wired output mode between GamePad & GamePadAlt.

# GameCube
BlueRetro will emulate the device selected in output config #1 on GameCube port 1.\
BlueRetro will emulate the device selected in output config #2 on GameCube port 2.\
BlueRetro will emulate the device selected in output config #3 on GameCube port 3.\
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

See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vT9rPK2__komCjELFpf0UYz0cMWwvhAXgAU7C9nnwtgEaivjsh0q0xeCEiZAMA-paMrneePV7IqdX48/pubhtml) for Bluetooth controller & GameCube controller buttons label correspondence.

### Special buttons functions
* **MS (SELECT | VIEW | SHARE | -)**: Toggle face buttons mapping between **Standard position base mapping** & **Rotated name based mapping**.
  This is usefull for Switch controller that physically mimic a GameCube Controller.

# Wii-Ext
*refers to the connector found on the downside of Wii Remotes and on the front of NES Mini and SNES Mini consoles.*

BlueRetro will emulate the device selected in output config #1 on Wii port 1.\
BlueRetro will emulate the device selected in output config #2 on Wii port 2.

## Multitap Config
Multitap config has no effect.

## Output Config

### Mode
* **GamePad**: BlueRetro will emulate a Wii Classic Pro (Digital trigger).
* **GamePadAlt**: BlueRetro will emulate the original Wii Classic controller (Analog trigger).
* **Keyboard**: NA
* **Mouse**: NA

### Accessories
Accessories config has no effect.

## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vT9rPK2__komCjELFpf0UYz0cMWwvhAXgAU7C9nnwtgEaivjsh0q0xeCEiZAMA-paMrneePV7IqdX48/pubhtml) for Bluetooth controller & Wii controller buttons label correspondence.
