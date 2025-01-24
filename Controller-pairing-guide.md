# Table of contents

* [i - Your controller not in the list?](#i---your-controller-not-in-the-list)
* [ii - BlueRetro Joystick calibration](#ii---blueretro-joystick-calibration)
* [1 - List of tested Bluetooth devices](#1---list-of-tested-bluetooth-devices)
  * [1.1 - List of tested Bluetooth Gamepads](#11---list-of-tested-bluetooth-gamepads)
  * [1.2 - List of tested Bluetooth Keyboards](#12---list-of-tested-bluetooth-keyboards)
  * [1.3 - List of tested Bluetooth Mouses](#13---list-of-tested-bluetooth-mouses)
* [2 - PS3 Pairing Guide](#2---ps3-pairing-guide)
  * [2.1 - First pairing](#21---first-pairing)
    * [2.1.1 - Windows](#211---windows)
    * [2.1.2 - OSX](#212---osx)
  * [2.2 - Reconnect](#22---reconnect)
* [3 - PS4 & PS5 Pairing Guide](#3---ps4--ps5-pairing-guide)
* [4 - Xbox Pairing Guide](#4---xbox-pairing-guide)
* [5 - Wii & WiiU Pro Pairing Guide](#5---wii--wiiu-pro-pairing-guide)
* [6 - Switch Pairing Guide](#6---switch-pairing-guide)
  * [6.1 - First pairing](#61---first-pairing)
  * [6.2 - Reconnect](#62---reconnect)
  * [6.3 - Dual Joycon Pairing Guide](#63---dual-joycon-pairing-guide)
* [7 - 8bitdo Pairing Guide](#7---8bitdo-pairing-guide)
  * [7.1 - First pairing](#71---first-pairing)
  * [7.2 - Reconnect](#72---reconnect)
  * [7.3 - D-pad as Joystick or D-pad configuration](#73---d-pad-as-joystick-or-d-pad-configuration)
* [8 - Retro-Bit Pairing Guide](#8---retro-bit-pairing-guide)
* [9 - Steam Controller Pairing Guide](#9---steam-controller-pairing-guide)
* [10 - RetroFighters Warrior Adapter Pairing Guide](#10---retrofighters-warrior-adapter-pairing-guide)
* [11 - RetroFighters Brawler64 Bluetooth Pairing Guide](#11---retrofighters-brawler64-bluetooth-pairing-guide)
  * [11.1 - First pairing](#111---first-pairing)
    * [11.1.1 - Switch Mode](#1111---switch-mode)
    * [11.1.2 - Xinput Mode](#1112---xinput-mode)
  * [11.2 - Reconnect](#112---reconnect)
* [12 - Exlene GameCube Pairing Guide](#12---exlene-gamecube-pairing-guide)
* [13 - Hyperkin Admiral Pairing Guide](#13---hyperkin-admiral-pairing-guide)
* [14 - Google Stadia Pairing Guide](#14---google-stadia-pairing-guide)
* [15 - 8BitDo N64 Modkit Pairing Guide](#15---8bitdo-n64-modkit-pairing-guide)
* [16 - 8BitDo NGC Modkit Pairing Guide](#16---8bitdo-ngc-modkit-pairing-guide)
* [17 - Atari VCS Pairing Guide](#17---atari-vcs-pairing-guide)

# i - Your controller not in the list?

I can add support for it if it's uniquely identifiable in one of its modes of operation.\
Follow this guide to get me a Bluetooth trace of it:\
[Getting BlueRetro Debug Trace](Debug-trace)

# ii - BlueRetro Joystick calibration

Each time a controller is connected to BlueRetro every axis (Joysticks & Triggers) neutral value is calibrated.
This calibration assume the joysticks and triggers are left to their neutral position during the connection process.

Some controller like Xbox, Stadia or any device in XInput mode do not send report update if no buttons/axes are pressed.

So for Xbox, Stadia or any device in XInput mode it's important to press a button (like A) a couple time after connection
while the joysticks and triggers are left to their neutral position so that BlueRetro is able to calibrate the neutral values properly.

# 1 - List of tested Bluetooth devices

## 1.1 - List of tested Bluetooth Gamepads

* Controller may have multiple hardware revision; only the ones listed under **Product Number** were tested.
* Controller may have various mode of operation; only the ones listed under **Mode** is supported.
* Controller often spoof the name of another ones and may not be detectable; for thoses a mapping preset other than default may be required and is listed under **Mapping preset**.

| Name                               | Product Number | Mode         | Mapping Src Label     | Mapping preset                       | Pairing Guide                                                                                                      |
|------------------------------------|----------------|--------------|-----------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------------------|
| 8bitdo GBros. Adapter              | 83GA           | Xinput       | GameCube              | Default Gamepad                      | [7](#7---8bitdo-pairing-guide)                                                                                     |
| 8bitdo M30 Bluetooth               | 80HA           | Xinput       | Saturn                | Default Gamepad                      | [7](#7---8bitdo-pairing-guide), [7.3](#73---d-pad-as-joystick-or-d-pad-configuration)                              |
| 8bitdo N30 Arcade Stick            | NS30           | Xinput       | Xbox One S / X\|S     | Default Gamepad                      | [7](#7---8bitdo-pairing-guide)                                                                                     |
| 8bitdo N64                         | RB8-N64        | HID Generic  | N64                   | Default Gamepad                      |                                                                                                                    |
| 8bitdo N64 Modkit                  |                | S            | Switch N64            | Default Gamepad                      | [15](#15---8bitdo-n64-modkit-pairing-guide)                                                                        |
| 8BitDo NGC Modkit                  |                | Android      | GameCube              | Default Gamepad                      | [16](#16---8bitdo-ngc-modkit-pairing-guide)                                                                        |
| 8bitdo NeoGeo Gamepad              |                | BT           | NeoGeo                | Default Gamepad                      |                                                                                                                    |
| 8bitdo SF30 Pro                    | 80DB           | Xinput       | 8bitdo SN30 / SF30    | Default Gamepad                      | [7](#7---8bitdo-pairing-guide)                                                                                     |
| 8bitdo S30 Modkit                  |                | Xinput       | Saturn                | Default Gamepad                      | [7](#7---8bitdo-pairing-guide), [7.3](#73---d-pad-as-joystick-or-d-pad-configuration)                              |
| 8bitdo N30 Modkit                  |                | Xinput       | NES                   | Default Gamepad                      | [7](#7---8bitdo-pairing-guide), [7.3](#73---d-pad-as-joystick-or-d-pad-configuration)                              |
| 8bitdo Ultimate                    |                | BT           | WiiU / Switch Pro     | Default Gamepad                      | [7](#7---8bitdo-pairing-guide)                                                                                     |
| Atari VCS Classic                  | 1511233-01     | HID Generic  | Xbox One S / X\|S     | Default Gamepad                      | [17](#17---atari-vcs-pairing-guide)                                                                                |
| Atari VCS Modern                   | 1511232-01     | HID Generic  | Xbox One S / X\|S     | Default Gamepad                      | [17](#17---atari-vcs-pairing-guide)                                                                                |
| Google Stadia                      | H2B            | HID Generic  | Default               | Default Gamepad                      | [14](#14---google-stadia-pairing-guide)                                                                            |
| Exlene GameCube                    |                | Switch       | WiiU / Switch Pro     | Default Gamepad                      | [12](#12---exlene-gamecube-pairing-guide)                                                                          |
| Hyperkin Admiral N64               | MO7389-AP      | Switch       | N64                   | Default Gamepad                      | [13](#13---hyperkin-admiral-pairing-guide)                                                                         |
| Microsoft Xbox Adaptive            | 1836           | BT           | Xbox One S / X\|S     | Default Gamepad                      | [4](#4---xbox-pairing-guide)                                                                                       |
| Microsoft Xbox One S               | 1708           | BT           | Xbox One S / X\|S     | Default Gamepad                      | [4](#4---xbox-pairing-guide)                                                                                       |
| Microsoft Xbox Series X\|S         | 1954           | BT           | Xbox One S / X\|S     | Default Gamepad                      | [4](#4---xbox-pairing-guide)                                                                                       |
| Nintendo Switch Famicom & NES      | HAC-033-036    | Switch       | Switch NES            | Default Gamepad                      | [6](#6---switch-pro--joycon-pairing-guide)                                                                         |
| Nintendo Switch Joycon (Dual)      | HAC-015-016    | Switch       | Switch Joycon         | **Switch Left/Right Joycon Upright** | [6.3](#63---dual-joycon-pairing-guide)                                                                             |
| Nintendo Switch Joycon (Single)    | HAC-015-016    | Switch       | Switch Joycon         | Default Gamepad                      | [6](#6---switch-pro--joycon-pairing-guide)                                                                         |
| Nintendo Switch MD & Genesis 3btns | HAC-045        | Switch       | Switch MD / Genesis   | Default Gamepad                      | [6](#6---switch-pro--joycon-pairing-guide)                                                                         |
| Nintendo Switch Mega Drive 6btns   | HAC-046        | Switch       | Switch MD / Genesis   | Default Gamepad                      | [6](#6---switch-pro--joycon-pairing-guide)                                                                         |
| Nintendo Switch N64                | HAC-043        | Switch       | Switch N64            | Default Gamepad                      | [6](#6---switch-pro--joycon-pairing-guide)                                                                         |
| Nintendo Switch Pro                | HAC-013        | Switch       | WiiU / Switch Pro     | Default Gamepad                      | [6](#6---switch-pro--joycon-pairing-guide)                                                                         |
| Nintendo Switch SFC & SNES         | HAC-042        | Switch       | Switch SNES           | Default Gamepad                      | [6](#6---switch-pro--joycon-pairing-guide)                                                                         |
| Nintendo Wiimote                   | RVL-036        | Wii          | Wiimote               | Default Gamepad                      | [5](#5---wii--wiiu-pro-pairing-guide)                                                                              |
| Nintendo Wiimote + Classic         | RVL-005        | Wii          | Wiimote + Classic     | Default Gamepad                      | [5](#5---wii--wiiu-pro-pairing-guide)                                                                              |
| Nintendo Wiimote + Classic Pro     | RVL-005 (-02)  | Wii          | Wiimote + Classic Pro | Default Gamepad                      | [5](#5---wii--wiiu-pro-pairing-guide)                                                                              |
| Nintendo Wiimote + Nunchuck        | RVL-004        | Wii          | Wiimote + Nunchuck    | Default Gamepad                      | [5](#5---wii--wiiu-pro-pairing-guide)                                                                              |
| Nintendo WiiU Pro                  | WUP-005        | Wii          | WiiU / Switch Pro     | Default Gamepad                      | [5](#5---wii--wiiu-pro-pairing-guide) [Press -](BlueRetro-System-Specific-User-Manual#special-buttons-functions-8) |
| PowerA GameCube                    | 1511638-01     | Switch       | WiiU / Switch Pro     | Default Gamepad                      | [6](#6---switch-pro--joycon-pairing-guide)                                                                         |
| Retro-Bit SEGA Saturn Bluetooth    |                | Xinput       | Saturn                | Default Gamepad                      | [8](#8---retro-bit-pairing-guide)                                                                                  |
| Retro Fighters Brawler64 Bluetooth |                | Switch       | Switch N64            | Default Gamepad                      | [11](#11---retrofighters-brawler64-bluetooth-pairing-guide)                                                        |
| Retro Fighters Warrior Adapter     |                | Xinput       | Game Cube             | Default Gamepad                      | [10](#10---retrofighters-warrior-adapter-pairing-guide)                                                            |
| Sony PS3 DualShock 3               |                | PS3          | PS3                   | Default Gamepad                      | [2](#2---ps3-pairing-guide)                                                                                        |
| Sony PS3 Sixaxis                   |                | PS3          | PS3                   | Default Gamepad                      | [2](#2---ps3-pairing-guide)                                                                                        |
| Sony PS4 DualShock 4               |                | PS4          | PS4 / PS5             | Default Gamepad                      | [3](#3---ps4--ps5-pairing-guide)                                                                                   |
| Sony PS5 DualSense                 | CFI-ZCT1W      | PS5          | PS4 / PS5             | Default Gamepad                      | [3](#3---ps4--ps5-pairing-guide)                                                                                   |
| Valve Steam Controller             | 1001           | Lizard (BLE) | KB & Mouse            | **DC FPS for Steam ctrl lizard**     | [9](#9---steam-controller-pairing-guide)                                                                           |

## 1.2 - List of tested Bluetooth Keyboards
If your keyboard prompt for a pin on Windows you may have to do the same with BlueRetro.
Simply put 0000 and press Enter (BlueRetro have no way to ask you to do so).
This is only needed for older BT keyboard, BT 4.0+ (LE) will not ask for a pin.

* Logitech MX5000 (Enter pin 0000 when prompted by KB screen)
* Logitech K600
* 8BitDo Retro Mechanical Keyboard

## 1.3 - List of tested Bluetooth Mouses
* Logitech MX Master 2S
* Logitech M585
* Logitech M720
* Rapoo MT550
* Rapoo 7200M

# 2 - PS3 Pairing Guide

* Note: only official PS3 controllers are supported.

## 2.1 - First pairing

### 2.1.1 - Windows

1. Download and install [Sixaxis Pair Tool](https://sixaxispairtool.en.lo4d.com/windows#:~:text=The%20Sixaxis%20Pair%20Tool%20is,games%20with%20your%20PS3%20controller.)
2. Determine BlueRetro MAC address

- Open https://blueretro.io/ in a chrome web browser (desktop/android).
- Navigate to "BlueRetro System Manager".
- Click on "Connect BlueRetro".
- Pair your device.

    On connection the MAC address of the device will be shown: write it down.

    ```
    Connected to:BlueRetro_XX_XXXX
    (XX:XX:XX:XX:XX:XX)[v.x.x.x]
    ```
3. Connect your PS3 controller to PC using USB cable.
4. Launch Sixaxis pair tool and type in the address found in step #2.\
![](img/SixaxisPairTool_v0FDiegEiq.png)
5. Click update, once done disconnect the controller from PC.
6. Boot up BlueRetro and press the PS button, the controller should connect to BlueRetro.

### 2.1.2 - OSX

1. Install Prerequisites (macOS)

- Install Homebrew https://brew.sh
- Install required libs & packages

    ```brew install wget libusb libusb-compat```

2. Compile sixpair binary

    ```
    mkdir ~/Documents/sixpair
    cd ~/Documents/sixpair
    wget -O sixpair.c https://gist.github.com/wouterds/4ab5715966812009d634e3d034abc7fc/raw
    gcc -o sixpair sixpair.c -lusb
    ```

    If everything went well you should now have a sixpair executable at `~/Documents/sixpair`.

3. Determine BlueRetro MAC address

- Open https://blueretro.io/ in a chrome web browser (desktop/android)
- Navigate to "BlueRetro System Manager"
- Click on "Connect BlueRetro"
- Pair your device

    On connection the MAC address of the device will be shown. Write it down.

    ```
    Connected to:BlueRetro_XX_XXXX
    (XX:XX:XX:XX:XX:XX)[v.x.x.x]
    ```

- Open a shell terminal and set the master PS3 address to BlueRetro MAC address

    ```
    .~/Documents/sixpair/sixpair XX:XX:XX:XX:XX:XX
    ```

## 2.2 - Reconnect

1. Simply press PS button to reconnect to BlueRetro.

# 3 - PS4 & PS5 Pairing Guide

## 3.1 - First pairing

1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing).
2. Press & hold simultaneously Share & PS buttons until the LED blink white.
3. Color on controller will change once pairing is complete.

## 3.2 - Reconnect

1. Simply press PS button to reconnect to BlueRetro.

# 4 - Xbox Pairing Guide

Update firmware via the [Xbox accessories Win10 app](https://apps.microsoft.com/store/detail/xbox-accessories/9NBLGGH30XJ3).

## 4.1 - First pairing

1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing).
2. Power on controller via Xbox button and then hold the black sync button until the logo blink.
3. Logo will stop blinking on controller once pairing is complete.
4. Press A buttons a few times to make sure joystick center value is properly init.

## 4.2 - Reconnect

1. Simply hold Xbox button for a small moment to power on controller and it will reconnect to BlueRetro.
2. Press A buttons a few times to make sure joystick center value is properly init.

# 5 - Wii & WiiU Pro Pairing Guide
* 1+2 pairing is not supported.

## 5.1 - First pairing

1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing).
2. Press red Sync button.
3. LEDs will stop blinking on controller once pairing is complete.

## 5.2 - Reconnect

1. Simply press any button on controller and it will reconnect to BlueRetro.

# 6 - Switch Pairing Guide

## 6.1 - First pairing

1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing).
2. Press and hold sync button until LEDs move in a left/right pattern.
3. LEDs will stop pattern on controller once pairing is complete.

## 6.2 - Reconnect
1. Simply press any button twice on controller and it will reconnect to BlueRetro.

## 6.3 - Dual Joycon Pairing Guide

1. Go to https://blueretro.io/presets.html and connect to your BlueRetro.
2. First select output 1 and select "Switch Left Joycon Upright" click save, wait for green text to appear.\
   <img width="281" alt="chrome_CosPbgOsVu" src="https://user-images.githubusercontent.com/3744056/180513746-d27d6cda-9b59-4c58-8875-885ec6b73f68.png">
3. Then select output 2 and select "Switch Right Joycon Upright" click save, wait for green text to appear.\
   <img width="295" alt="chrome_lYNgsZs9ih" src="https://user-images.githubusercontent.com/3744056/180513770-75222de2-fb66-4cef-8e2a-9237ab5b020d.png">
4. Then pair the joycon with blueretro separately using the sync button hidden on the sliding side.\
   It's important to connect the left joycon first, then connect the right joycon.
5. After that you can clip them on the middle support and they should function as one controller.

# 7 - 8bitdo Pairing Guide
Update firmware via the [8bitdo Upgrade tool Win10 app](https://support.8bitdo.com/firmware-updater.html).

## 7.1 - First pairing

1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing).
2. Power up 8bitdo controller in Xinput mode (Start + X or set switch to X) (Only Xinput mode supported!!).
2. Press and hold sync button until LEDs flash.
3. LEDs will stop pattern on controller once pairing is complete.
4. Press A buttons a few times to make sure joystick center value is properly init.

## 7.2 - Reconnect
1. Simply press Start on controller and it will reconnect to BlueRetro.
2. Press A buttons a few times to make sure joystick center value is properly init.

## 7.3 - D-pad as Joystick or D-pad configuration
Most 8bitdo controllers are configured to have the D-pad emulate a joystick by default.
In most case for BlueRetro you will want to configure it as a d-pad.

See [8bitdo support page FAQs for each controller](https://support.8bitdo.com/) for more info.

* 8bitdo S30 Modkit: Hold Up + L + R for 5 seconds
* 8bitdo N30 Modkit: Hold Up + Select for 5 seconds
* 8bitdo M30 Bluetooth: Hold Up + Select for 5 seconds

# 8 - Retro-Bit Pairing Guide

## 8.1 - First pairing

1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing).
2. Power up Retro-Bit controller in Xinput mode (Home + X) (Only Xinput mode supported!!).
2. If done properly 2 LEDs will flash.
3. LEDs will stop flashing on controller once pairing is complete and rumble will trigger.

## 8.2 - Reconnect
1. Simply press Homeon controller and it will reconnect to BlueRetro.

# 9 - Steam controller Pairing Guide

You need to first install the BLE firmware update:\
https://help.steampowered.com/en/faqs/view/1796-5FC3-88B3-C85F

## 9.1 - First pairing

1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing).
2. Power on controller by holding Y and then pressing the Steam button.
3. Logo will stop blinking on controller once pairing is complete.

## 9.2 - Reconnect

1. Simply press Steam button to power on controller and it will reconnect to BlueRetro.

# 10 - RetroFighters Warrior Adapter Pairing Guide

## 10.1 - First pairing

1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing).
2. Power on adapter by holding Home + Minus simultaneously until LED start blinking fast.
3. LED will stop blinking once pairing is complete.

## 10.2 - Reconnect

1. Simply press Home button to power on adapter and it will reconnect to BlueRetro.

# 11 - RetroFighters Brawler64 Bluetooth Pairing Guide

## 11.1 - First pairing
1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing).
2. Power up Brawler64 by holding sync button until LEDs move in a up/down pattern.
3. LED will stop blinking once pairing is complete.

## 11.2 - Reconnect

1. Simply press any button a few time to power it on and it will reconnect to BlueRetro.

# 12 - Exlene GameCube Pairing Guide

The controller will mock an Switch Pro controller and can't be uniquely identified.
As such you need to press (-) to toggle on the [**Rotated name based mapping**](BlueRetro-System-Specific-User-Manual#special-buttons-functions-8).

## 12.1 - First pairing

1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing).
2. Power up the Exlene controller by holding Home until LED start blinking fast.
3. LED will stop blinking once pairing is complete.

## 12.2 - Reconnect

1. Simply press Home button to power on Exlene controller and it will reconnect to BlueRetro.

# 13 - Hyperkin Admiral Pairing Guide

## 13.1 - First pairing

1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing).
2. Power up the controller by holding the Sync button until LED start blinking fast.
3. LED will stop blinking once pairing is complete.

## 13.2 - Reconnect

1. It's important to press the A button to power on the Admiral controller as it's select the default internal mapping of the controller.\
   It will reconnect to BlueRetro after doing so.

# 14 - Google Stadia Pairing Guide

## 14.1 - First pairing

1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing).
2. Power up the Stadia controller by holding Stadia button + the Y button simultaneously until LED start blinking orange.
3. LED will blink white once pairing is complete.

## 14.2 - Reconnect

1. Simply press Stadia button to power on Stadia controller and it will reconnect to BlueRetro.

# 15 - 8BitDo N64 Modkit Pairing Guide

## 15.1 - First pairing

1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing).
2. Set switch at bottom of 8BitDo rumble to **S**.
3. Power up the 8BitDo N64 Modkit controller by holding start.
4. Hold sync button until LED start blinking fast.
5. LED will stop blinking once pairing is complete.
6. Press A buttons a few times to make sure joystick center value is properly init.

## 15.2 - Reconnect

1. Set switch at bottom of 8BitDo rumble to **S**.
2. Power up the 8BitDo N64 Modkit controller by holding start.
3. LED will stop blinking once pairing is complete.
4. Press A buttons a few times to make sure joystick center value is properly init.

# 16 - 8BitDo NGC Modkit Pairing Guide
8bitdo Switch mode will not work properly with BlueRetro.

Make sure to use either the **Default Gamepad only** or the **Default Gamepad/Keyboard** presets to make
the triggers end button active. (Merge preset simulate the end button base on analog position.)

## 16.1 - First pairing

1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing).
2. Power up 8BitDo NGC Modkit in Android mode (Start + B) (Only Android mode supported!!).
3. LEDs on controller will stop flashing once pairing is complete.
4. Press A buttons a few times to make sure joystick center value is properly init.

## 16.2 - Reconnect

1. Power up the 8BitDo NGC Modkit controller by holding start.
2. LED will stop blinking once pairing is complete.
3. Press A buttons a few times to make sure joystick center value is properly init.

# 17 - Atari VCS Pairing Guide

## 17.1 - First pairing

1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing).
2. Press and hold the Atari button until the button LED start flashing quickly.
3. LEDs on controller will stop flashing once pairing is complete.
4. Press A buttons a few times to make sure joystick center value is properly init.

## 17.2 - Reconnect

1. Press and release the Atari button.
2. LED will stop blinking once pairing is complete.
3. Press A buttons a few times to make sure joystick center value is properly init.
