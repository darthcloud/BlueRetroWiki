# Table of contents

* [Introduction](#introduction)
* [Advance config page](#advance-config-page)
* [Presets page](#presets-page)
* [System manager page](#system-manager-page)
* [OTA FW update page](#ota-fw-update-page)
* [Files Manager page](#files-manager-page)
* [N64 controller pak manager page](#n64-controller-pak-manager-page)

# Introduction

BlueRetro configuration is all done via various small web pages that use the
Web Bluetooth API to connect localy to your BlueRetro device over Bluetooth
Low Energy (BLE). Nothing need to be installed beside having a Google Chrome
based browser.

* [Advance config](https://blueretro.io/advance.html): The main configuration page were
  you can configure what type of accessories BlueRetro will emulate and define custom
  axes/buttons mapping for each player.
* [Presets config](https://blueretro.io/presets.html): This page allow to load predefined
  controller axes/buttons mapping.
* [System manager](https://blueretro.io/system.html): This page let you reboot, put to
  sleep or factory reset your BlueRetro device.
* [OTA FW update](https://blueretro.io/ota.html): This page let you update your BlueRetro
  device firmware wirelessly.
* [Files Manager](https://blueretro.io/files.html): This page let you delete files from
  the BlueRetro file system.
* [N64 controller pak manager](https://blueretro.io/n64_ctrlpak.html): This page let you
  manage N64 controller pak data.

# Advance config page

## Global config

From this section you can configure global settings like forcing system type or using system detection (Auto) (Only auto right now). You can enable multitap emulation as well (TBD).

## Output config

Here you can configure the wired output device type (gamepad, alternative gamepad (like 6 buttons),  keyboard or mouse) and if applicable accessories used with the controller (rumble pak, memory card).

## Mapping config

Up to 128 mapping can be added. Simply click on +/- buttons to add or remove a mapping. The label used are as generic as possible but still describe the usual function well. I say usual because even if the name implies an axis direction or a button it might not be the case. For example, the N64 destination RX-Left is C-Left button. See BlueRetro label mapping reference for the exact mapping on source and destination controllers.

For each mapping you can configure various options which might or not be used base on what the source and destination end up to be a button or an axis and vice versa.

**If all you want to do is a simple button remapping, all you need to touch is the src and dest colums, leave everything else to default value.**

* Src - This is the source button/axis on the Bluetooth controller
* Dest - This is the destination button/axis on the wired interface.
* Dest ID - This is the ID of the wired interface.
* Max  - If source & destination is an axis then this is the scaling factor base on the
  destination maximum.\
  If source is a button & destination is an axis then this is the value base on
  destination maximum that the axis will be set.
* Threshold - If source is an axis and destination is a button, this is the threshold
  requires on the source axis before the button is pressed.
* Deadzone - This is the axis dead zone around reset value.
* Turbo - Turbo function base on the system frame rate.
* Scaling - Various response curve for scaling. (Only Passthrough and Linear available,
  others not yet implemented)
* Diagonal - (Not yet implemented) ~~Diagonal scaling options between joystick type.~~

# Presets page

Presets are predefined button mapping for a specific game or game type. They are JSON files located on the server that the client list via GitHub API. A user could simply fork the page on GitHub and upload its own presets.

# System manager page

# OTA FW update page

# Files Manager page

# N64 controller pak manager page
