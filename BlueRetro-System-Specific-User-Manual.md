# Table of contents
* [NES](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-System-Specific-User-Manual#nes)
* [SNES](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-System-Specific-User-Manual#snes)
* [Saturn](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-System-Specific-User-Manual#saturn)
* [Nintendo 64](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-System-Specific-User-Manual#nintendo-64)
* [Dreamcast](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-System-Specific-User-Manual#dreamcast)
* [GameCube](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-System-Specific-User-Manual#gamecube)
* [JVS](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-System-Specific-User-Manual#jvs)
# NES
## Multitap Config
* **None**: BlueRetro will emulate the device selected in output config #1 on NES port 1.\
        BlueRetro will emulate the device selected in output config #2 on NES port 2.
* **Slot 1**: BlueRetro will emulate a Four Score multitap with 4 controllers (Use both NES ports).
* **Slot 2**: BlueRetro will emulate a Four Score multitap with 4 controllers (Use both NES ports).
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
# Saturn
## Multitap Config
* **None**: BlueRetro will emulate the device selected in output config #1 on Saturn port 1.\
  BlueRetro will emulate the device selected in output config #2 on Saturn port 2.
* **Slot 1**: BlueRetro will emulate a Saturn Multitap with 6 controllers on port 1 as configured in output config #1-6.\
  BlueRetro will emulate the device selected in output config #7 on Saturn port 2.
* **Slot 2**: BlueRetro will emulate the device selected in output config #1 on Saturn port 1.\
  BlueRetro will emulate a Saturn Multitap with 6 controllers on port 2 as configured in output config #2-7.
* **Dual**: BlueRetro will emulate a Saturn Multitap with 6 controllers on port 1 & 2 (Total 12 controllers) as configured in output config #1-12.
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
# Nintendo 64
## Multitap Config
* **None**: BlueRetro will emulate the device selected in output 1 config on NES port 1.\
        BlueRetro will emulate the device selected in output 2 config on NES port 2.
* **Slot 1**: BlueRetro will emulate a Four Score multitap with 4 controllers (Use both NES ports).
* **Slot 2**: BlueRetro will emulate a Four Score multitap with 4 controllers (Use both NES ports).
* **Dual**: BlueRetro will emulate a Four Score multitap with 4 controllers (Use both NES ports).
* **Alt**: BlueRetro will emulate a Japanese 4P adapter multitap with 4 controllers (Use both NES ports & FC DB15).
## Output Config
### Mode
* **GamePad**: BlueRetro will emulate a standard 8 buttons NES controller.
* **GamePadAlt**: BlueRetro will emulate a standard 8 buttons NES controller.
* **Keyboard**: **TBD** ~~BlueRetro will emulate a Famicom keyboard.~~
* **Mouse**: **TBD** ~~BlueRetro will emulate a Famicom Hori Trackball.~~
### Accessories
Accessories config has no effect.
## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vRln_dhkahEIhq4FQY_p461r5qvLn-Hkl89ZtfyIOGAqdnPtQZ5Ihfsjvd94fRbaHX8wU3F-r2ODYbM/pubhtml) for Bluetooth controller & N64 controller buttons label correspondence.
# Dreamcast
## Multitap Config
* **None**: BlueRetro will emulate the device selected in output 1 config on NES port 1.\
        BlueRetro will emulate the device selected in output 2 config on NES port 2.
* **Slot 1**: BlueRetro will emulate a Four Score multitap with 4 controllers (Use both NES ports).
* **Slot 2**: BlueRetro will emulate a Four Score multitap with 4 controllers (Use both NES ports).
* **Dual**: BlueRetro will emulate a Four Score multitap with 4 controllers (Use both NES ports).
* **Alt**: BlueRetro will emulate a Japanese 4P adapter multitap with 4 controllers (Use both NES ports & FC DB15).
## Output Config
### Mode
* **GamePad**: BlueRetro will emulate a standard 8 buttons NES controller.
* **GamePadAlt**: BlueRetro will emulate a standard 8 buttons NES controller.
* **Keyboard**: **TBD** ~~BlueRetro will emulate a Famicom keyboard.~~
* **Mouse**: **TBD** ~~BlueRetro will emulate a Famicom Hori Trackball.~~
### Accessories
Accessories config has no effect.
## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vRln_dhkahEIhq4FQY_p461r5qvLn-Hkl89ZtfyIOGAqdnPtQZ5Ihfsjvd94fRbaHX8wU3F-r2ODYbM/pubhtml) for Bluetooth controller & Dreamcast controller buttons label correspondence.
# GameCube
## Multitap Config
* **None**: BlueRetro will emulate the device selected in output 1 config on NES port 1.\
        BlueRetro will emulate the device selected in output 2 config on NES port 2.
* **Slot 1**: BlueRetro will emulate a Four Score multitap with 4 controllers (Use both NES ports).
* **Slot 2**: BlueRetro will emulate a Four Score multitap with 4 controllers (Use both NES ports).
* **Dual**: BlueRetro will emulate a Four Score multitap with 4 controllers (Use both NES ports).
* **Alt**: BlueRetro will emulate a Japanese 4P adapter multitap with 4 controllers (Use both NES ports & FC DB15).
## Output Config
### Mode
* **GamePad**: BlueRetro will emulate a standard 8 buttons NES controller.
* **GamePadAlt**: BlueRetro will emulate a standard 8 buttons NES controller.
* **Keyboard**: **TBD** ~~BlueRetro will emulate a Famicom keyboard.~~
* **Mouse**: **TBD** ~~BlueRetro will emulate a Famicom Hori Trackball.~~
### Accessories
Accessories config has no effect.
## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vRln_dhkahEIhq4FQY_p461r5qvLn-Hkl89ZtfyIOGAqdnPtQZ5Ihfsjvd94fRbaHX8wU3F-r2ODYbM/pubhtml) for Bluetooth controller & GameCube controller buttons label correspondence.
# JVS
## Multitap Config
* **None**: BlueRetro will emulate the device selected in output 1 config on NES port 1.\
        BlueRetro will emulate the device selected in output 2 config on NES port 2.
* **Slot 1**: BlueRetro will emulate a Four Score multitap with 4 controllers (Use both NES ports).
* **Slot 2**: BlueRetro will emulate a Four Score multitap with 4 controllers (Use both NES ports).
* **Dual**: BlueRetro will emulate a Four Score multitap with 4 controllers (Use both NES ports).
* **Alt**: BlueRetro will emulate a Japanese 4P adapter multitap with 4 controllers (Use both NES ports & FC DB15).
## Output Config
### Mode
* **GamePad**: BlueRetro will emulate a standard 8 buttons NES controller.
* **GamePadAlt**: BlueRetro will emulate a standard 8 buttons NES controller.
* **Keyboard**: **TBD** ~~BlueRetro will emulate a Famicom keyboard.~~
* **Mouse**: **TBD** ~~BlueRetro will emulate a Famicom Hori Trackball.~~
### Accessories
Accessories config has no effect.
## Mapping
See [BlueRetro mapping reference](https://docs.google.com/spreadsheets/d/e/2PACX-1vRln_dhkahEIhq4FQY_p461r5qvLn-Hkl89ZtfyIOGAqdnPtQZ5Ihfsjvd94fRbaHX8wU3F-r2ODYbM/pubhtml) for Bluetooth controller & JVS controller buttons label correspondence.