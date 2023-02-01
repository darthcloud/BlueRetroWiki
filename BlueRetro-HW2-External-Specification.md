# This is not a modding guide. While all the information is listed, you need to be experienced in electronic to make use of this information.

# Table of contents
* [1 - External mode detection](#1---external-mode-detection)
* [2 - I39 pin usage](#2---i39-pin-usage)
* [3 - Controller plug-in detection](#3---controller-plug-in-detection)
* [4 - Port status LED](#4---port-status-led)
* [5 - Global status LED](#5---global-status-led)
* [6 - Reset button](#6---reset-button)
* [7 - Universal interface pinout](#7---universal-interface-pinout)
* [8 - Wired interface pinout](#8---wired-interface-pinout)
* [9 - Example schematic base on spec](#9---example-schematic-base-on-spec)

# 1 - External mode detection

HW2 base design allow to use the same firmware for internal and external BlueRetro device.

External mode is detected via the otherwise unused pin for power (IO13) and reset (IO14).
The adapter is deemed to be external if both pins state is "active" base on the polarity of those pins for each system.
See table below on how to wire both pins for each system.

System | IO13 | IO14
------ | ---- | ----
Universal | HI | HI
GameCube | HI | HI
(S)NES Mini (Wii ext.) | LO | HI
TODO | Others | System

# 2 - I39 pin usage

### System specific firmware

Connected directly to the ESP32 3V3 rail.

### Universal firmware

This pin is used by the detacheable cable to select between which detection system bank is used by the firmware.

System | I39
------ | ---
Famicom / NES | LO
PC Engine / TG16 | LO
Mega Drive / Genesis | LO
SFC / SNES | HI
CD-i | HI
3DO | HI
PlayStation | LO
Saturn | HI
PC-FX | HI
JVS (Arcade) | LO
Nintendo 64 | LO
Dreamcast | LO
GameCube | HI
(S)NES Mini (Wii ext.) | LO

# 3 - Controller plug-in detection
ESP32 IO | Direction | Function | Note
---------- | ---------- | --------- | ------
35* | Input | Controller port 1 detect | 3.3v level, low: plug disconnect, high: pluged in
36** | Input | Controller port 2 detect | 3.3v level, low: plug disconnect, high: pluged in
32 | Input | Controller port 3 detect | 3.3v level, low: plug disconnect, high: pluged in
33 | Input | Controller port 4 detect | 3.3v level, low: plug disconnect, high: pluged in

```
* P1 pin # for Mega Drive / Genesis / Saturn / Jaguar is IO15 due to conficts
** P2 pin # for Mega Drive / Genesis / Saturn / Jaguar is I34 due to conficts
```

To avoid spurious interrupt from disconnected plug cable, the detection pins are used to detect disconnection and disable that port on BlueRetro.

### Option 1: System with dual supply
``` PlayStation & GameCube ```

Use the higher supply rail (5V or 8V) to power BlueRetro, connect each plug cable of that rail together to all supply from any port.

Put a 47K pull-down resitor on each detection pins to GND. Wire the lower supply rail (3V3) to the detection pin.

### Option 2: System with only 3V3 supply
``` Nintendo 64 ```\
``` The first plug is always required to be used. ```

Use the first port plug 3V3 to power the adapter and wire the first detection pin to the first port 3V3 as well.

Put a 47K pull-down resitor on P2, P3 & P4 detection pins to GND. Wire the 3V3 of cable P2, P3 & P4 to the detection pin.

### Option 3: System with only 5V supply
``` All others system ```\
``` The first plug is always required to be used. ```

Use the first port plug 5V to power the adapter and wire the first detection pin to ESP32 3V3 supply.

Put a 20K pull-down resitor on P2 (and P3 & P4 for Dreamcast) detection pins to GND. Wire the 5V of cable P2 (and P3 & P4 for Dreamcast) to the detection pin through a series 10K resistor.

# 4 - Port status LED
ESP32 IO | Direction | Function | Note
---------- | ---------- | --------- | ------
2 | Output | Controller port 1 LED | 3.3v level
4 | Output | Controller port 2 LED | 3.3v level
12 | Output | Controller port 3 LED | 3.3v level
15 | Output | Controller port 4 LED | 3.3v level

All those pin are ESP32 strapping pin. Interface via MOSFET to avoid problem at boot.

![](img/port_led.png)

### Behavior while in pairing mode
* The first available port LED will be pulsing.

### Behavior when BT controller connected
* Port which got an active BT connection will have it's corresponding LED solid.

### Behavior while system reset is pressed (Boot button)
* All port LED are used to indicate current switch function (See [6](#6---reset-button))

# 5 - Global status LED
ESP32 IO | Direction | Function | Note
---------- | ---------- | --------- | ------
17 | Output | BlueRetro status LED | 3.3v level

![](img/sts_led.png)

### Behavior while in pairing mode
* LED will be pulsing.

### Behavior while system reset is pressed (Boot button)
* LED indicate current switch function (See [6](#6---reset-button))

### Behavior when an unrecoverable error occur
* LED will be solid.

# 6 - Reset button
ESP32 IO | Direction | Function | Note
---------- | ---------- | --------- | ------
0 | Input | ESP32 boot button | Idle high

* Button press under < 3 sec (All LEDs solid):
  If in pairing mode: Stop pairing mode otherwise all BT devices are disconnect.
* Button press between > 3 sec and < 6 sec (All LEDs blink slowly):
  Start pairing mode.
* Button press between > 6 sec and < 10 sec (All LEDs blink fast):
  Factory reset ESP32 to original BlueRetro firmware the device shipped with & reset configuration.

# 7 - Universal interface pinout
``` In HW2 pin 20 of the DB25 was change from IO0 to IO15 ```

The universal firmware is design to use a DB25 interface wired as follow.

DB25 pin | ESP32 IO
-------- | --------
1 | IO23
14 | IO22
2 | IO1 (TXD)
15 | IO3 (RXD)
3 | IO21
16 | IO19
4 | IO18
17 | IO5
5 | GND
18 | IO17
6 | 3V3
19 | IO16
7 | 5V-8V
20 | IO15
8 | GND
21 | I36
9 | GND
22 | I39
10 | I34
23 | I35
11 | IO32
24 | IO33
12 | IO25
25 | IO26
13 | IO27

# 8 - Wired interface pinout
See [BlueRetro Core Pinout Specification](BlueRetro-Core-Pinout-Specification)

# 9 - Example schematic base on spec
* GameCube: [gamecube_hw2_external.pdf](pdf/gamecube_hw2_external.pdf)
