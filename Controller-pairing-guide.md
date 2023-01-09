# Table of contents

* [1 - List of tested Bluetooth devices](#1---list-of-tested-bluetooth-devices)
* [2 - PS3 Pairing Guide](#2---ps3-pairing-guide)
* [3 - PS4 & PS5 Pairing Guide](#3---ps4--ps5-pairing-guide)
* [4 - Xbox Pairing Guide](#4---xbox-pairing-guide)
* [5 - Wii & WiiU Pro Pairing Guide](#5---wii--wiiu-pro-pairing-guide)
* [6 - Switch Pro & Joycon Pairing Guide](#6---switch-pro--joycon-pairing-guide)
* [7 - 8bitdo Pairing Guide](#7---8bitdo-pairing-guide)
* [8 - Retro-Bit Pairing Guide](#8---retro-bit-pairing-guide)

# 1 - List of tested Bluetooth devices

| Name | Product Number | Firmware | Mode | Mapping Src Label | Mapping preset | Pairing Guide | Known issues | Unconfirm issues |
| ---- | -------------- | -------- | ---- | ----------------- | -------------- | ------------- | ------------ | ---------------- |
| 8bitdo GBros. Adapter | 83GA | v2.26 | Xinput | GameCube | Default Gamepad |   |   |   |
| 8bitdo M30 Bluetooth | 80HA | v1.15 | Xinput | Saturn | Default Gamepad |   |   |   |
| 8bitdo N30 Arcade Stick | NS30 | v5.10 | Xinput | Xbox One S / X\|S | Default Gamepad |   |   |   |
| 8bitdo N64 | RB8-N64 | v2.00 | HID Generic | N64 | Default Gamepad |   |   |   |
| 8bitdo SF30 Pro | 80DB | v2.00 | Xinput | 8bitdo SN30/SF30 | Default Gamepad |   |   |   |
| Exlene GameCube |   | 2021-11 | Xinput (but they call it IOS) | Exlene GameCube | Exlene GameCube |   |   |   |
| Hyperkin Admiral N64 | MO7389-AP | v1.5.010722 | Switch | N64 | Default Gamepad |   |   |   |
| Microsoft Xbox Adaptive | 1836 | 5.15.3168.0 | Bluetooth | Xbox One S / X\|S | Default Gamepad |   |   |   |
| Microsoft Xbox One S | 1708 | 5.15.3168.0 | Bluetooth | Xbox One S / X\|S | Default Gamepad |   |   |   |
| Microsoft Xbox Series X\|S | 1954 | 5.15.3168.0 | Bluetooth | Xbox One S / X\|S | Default Gamepad |   |   |   |
| Nintendo Switch Famicom & NES | HAC-033, 034, 035, 036 |   | Switch | Switch NES | Default Gamepad |   |   |   |
| Nintendo Switch Joycon (Dual) | HAC-015, 016 |   | Switch | Switch Joycon | Default Gamepad |   |   |   |
| Nintendo Switch Joycon (Single) | HAC-015, 016 |   | Switch | Switch Joycon | Default Gamepad |   |   |   |
| Nintendo Switch MD & Genesis 3btns | HAC-045 |   | Switch | Switch MD / Genesis | Default Gamepad |   |   |   |
| Nintendo Switch MegaDrive 6btns | HAC-046 |   | Switch | Switch MD / Genesis | Default Gamepad |   |   |   |
| Nintendo Switch N64 | HAC-043 |   | Switch | Switch N64 | Default Gamepad |   |   |   |
| Nintendo Switch Pro | HAC-013 |   | Switch | WiiU / Switch Pro | Default Gamepad |   |   |   |
| Nintendo Switch SFC & SNES | HAC-042 |   | Switch | Switch SNES | Default Gamepad |   |   |   |
| Nintendo Wiimote | RVL-036 |   | Wii | Wiimote | Default Gamepad |   |   |   |
| Nintendo Wiimote + Classic | RVL-005 |   | Wii | Wiimote + Classic | Default Gamepad |   |   |   |
| Nintendo Wiimote + Classic Pro | RVL-005 (-02) |   | Wii | Wiimote + Classic Pro | Default Gamepad |   |   |   |
| Nintendo Wiimote + Nunchuck | RVL-004 |   | Wii | Wiimote + Nunchuck | Default Gamepad |   |   |   |
| Nintendo WiiU Pro | WUP-005 |   | Wii | WiiU / Switch Pro | Default Gamepad |   |   |   |
| PowerA GameCube | 1511638-01 |   | Switch | GameCube | Default Gamepad |   |   |   |
| Retro-Bit SEGA Saturn Bluetooth |   |   | Xinput | Saturn | Default Gamepad |   |   |   |
| RetroFighter Brawler64 Bluetooth |   |   | Xinput | N64 | Default Gamepad |   |   |   |
| RetroFighter Warrior Adapter |   |   | Switch | GameCube | Default Gamepad |   |   |   |
| Sony PS3 DualShock 3 |   |   | PS3 | PS3 | Default Gamepad |   |   |   |
| Sony PS3 Sixaxis |   |   | PS3 | PS3 | Default Gamepad |   |   |   |
| Sony PS4 DualShock 4 |   |   | PS4 | PS4 / PS5 | Default Gamepad |   |   |   |
| Sony PS5 DualSense | CFI-ZCT1W |   | PS5 | PS4 / PS5 | Default Gamepad |   |   |   |
| Valve Steam Controller |   |   | Lizard | KB & Mouse | DC FPS for Steam ctrl lizard |   |   |   |

# 2 - PS3 Pairing Guide

* Note only official PS3 controller are supported.

## 2.1 - First pairing

### 2.1.1 - Windows

1. Download and install [Sixaxis Pair Tool](https://sixaxispairtool.en.lo4d.com/windows#:~:text=The%20Sixaxis%20Pair%20Tool%20is,games%20with%20your%20PS3%20controller.)
2. Determine BlueRetro MAC address

- Open https://blueretro.io/ in a chrome web browser (desktop/android)
- Navigate to "BlueRetro System Manager"
- Click on "Connect BlueRetro"
- Pair your device

    On connection the MAC address of the device will be shown. Write it down.

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

1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing)
2. Press & hold simultaneously Share & PS buttons until the LED blink white.
3. Color on controller will change once pairing is complete.

## 3.2 - Reconnect

1. Simply press PS button to reconnect to BlueRetro.

# 4 - Xbox Pairing Guide
As of v1.2.1 the minimum required Xbox FW for controller are:\
Xbox One S: 4.8.1923.0\
Adaptive: 4.5.1680.0\
Series X|S: 5.9.2709.0

Update via the [Xbox accessories Win10 app](https://apps.microsoft.com/store/detail/xbox-accessories/9NBLGGH30XJ3).

## 4.1 - First pairing

1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing)
2. Power on controller via Xbox button and then hold the black sync button until the logo blink.
3. Logo will stop blinking on controller once pairing is complete.

## 4.2 - Reconnect

1. Simply hold Xbox button for a small moment to power on controller and it will reconnect to BlueRetro.

# 5 - Wii & WiiU Pro Pairing Guide
* 1+2 pairing is not supported.

## 5.1 - First pairing

1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing)
2. Press red Sync button
3. LEDs will stop blinking on controller once pairing is complete.

## 5.2 - Reconnect

1. Simply press any button on controller and it will reconnect to BlueRetro.

# 6 - Switch Pro & Joycon Pairing Guide

## 6.1 - First pairing

1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing)
2. Press and hold sync button until LEDs move in a left/right pattern.
3. LEDs will stop pattern on controller once pairing is complete.

## 6.2 - Reconnect
1. Simply press any button twice on controller and it will reconnect to BlueRetro.

# 7 - 8bitdo Pairing Guide
Update firmware via the [8bitdo Upgrade tool Win10 app](https://support.8bitdo.com/firmware-updater.html).

## 7.1 - First pairing

1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing)
2. Power up 8bitdo controller in Xinput mode (Start + X or set switch to X) (Only Xinput mode supported!!)
2. Press and hold sync button until LEDs flash.
3. LEDs will stop pattern on controller once pairing is complete.

## 7.2 - Reconnect
1. Simply press Start on controller and it will reconnect to BlueRetro.

# 8 - Retro-Bit Pairing Guide

## 8.2 - First pairing

1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing)
2. Power up Retro-Bit controller in Xinput mode (Home + X) (Only Xinput mode supported!!)
2. If done properly 2 LEDs will flash.
3. LEDs will stop flashing on controller once pairing is complete and rumble will trigger.

## 8.3 - Reconnect
1. Simply press Homeon controller and it will reconnect to BlueRetro.
