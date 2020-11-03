# Table of contents
* [FC / NES adapter cable](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-Cables-Build-Instructions#fc--nes-adapter-cable)
* [SFC / SNES adapter cable](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-Cables-Build-Instructions#sfc--snes-adapter-cable)
* [Saturn adapter cable](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-Cables-Build-Instructions#saturn-adapter-cable)
* [Nintendo 64 adapter cable](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-Cables-Build-Instructions#nintendo-64-adapter-cable)
* [Dreamcast adapter cable](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-Cables-Build-Instructions#dreamcast-adapter-cable)
* [GameCube adapter cable](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-Cables-Build-Instructions#gamecube-adapter-cable)
# FC / NES adapter cable
## Bill of materials
* DB25 Male solder cup (x1) (DKPN: AE10984-ND PN: A-DS 25 LL/Z)
* 74AHCT1G125 SC70-5 (x7) (DKPN: 296-4709-1-ND PN: SN74AHCT1G125DCKR)
* 3.6K resistors (x3) (DKPN: ‎S3.6KCACT-ND‎ PN: RNMF14FTC3K60‎) (Required for PAL system only)
* DB25 Backshell (x1) (DKPN: 970-25BPE-ND PN: 970-025-010R011)
* Level shifter PCB (x1)
* NES controller plug (x2)
* Famicom controller plug (x1) (Optional)
## Cable schematic
 [https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/NES.pdf](https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/NES.pdf)
## Pinout reference
![](img/cables/nes_pinout.png)
## Cable PCB build instruction
![](img/cables/nes.png)
* Solder 74AHCT1G125 to footprint highlighted in red.
* Bridge HI side of jumper I39.
* Connect pad DIR3 & DIR1 to GND.
* For using PAL system, add 3.6K pull-ups to NES 5V (pin 5) on pads IO18, IO5 & IO32.
* Connect cords according to table below and pinout reference.

PCB PAD | Cord | Pin | Name | Required?
------- | ---- | --- | ---- | ---------
VIN | NES P1 | 5 | 5V | Yes
GND | NES P1 | 1 | GND | Yes
IO32 | NES P1 | 3 | OUT0 | Yes
IO19 | NES P1 | 4 | P1_D0 | Yes
IO5 | NES P1 | 2 | P1_CUP | Yes
VIN | NES P2 | 5 | 5V | No
GND | NES P2 | 1 | GND | No
IO22 | NES P2 | 4 | P2_D0 | No
IO18 | NES P2 | 2 | P2_CUP | No
IO21 | FC_DB15 | 13 | P1_D1 | No
IO25 | FC_DB15 | 7 | P2_D1 | No
# SFC / SNES adapter cable
## Pinout reference
![](img/cables/snes_pinout.png)
## Bill of materials
* DB25 Male solder cup (x1) (DKPN: AE10984-ND PN: A-DS 25 LL/Z)
* 74AHCT1G125 SC70-5 (x9) (DKPN: 296-4709-1-ND PN: SN74AHCT1G125DCKR)
* DB25 Backshell (x1) (DKPN: 970-25BPE-ND PN: 970-025-010R011)
* Level shifter PCB (x1)
* SNES controller plug (x2)
## Cable schematic
 [https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/SNES.pdf](https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/SNES.pdf)
## Cable PCB build instruction
![](img/cables/snes.png)
* Solder 74AHCT1G125 to footprint highlighted in red.
* Connect cords according to schematic.
* Bridge LO side of jumper I39.
# Saturn adapter cable
## Pinout reference
![](img/cables/saturn_pinout.png)
## Bill of materials
* DB25 Male solder cup (x1) (DKPN: AE10984-ND PN: A-DS 25 LL/Z)
* 74AHCT1G125 SC70-5 (x14) (DKPN: 296-4709-1-ND PN: SN74AHCT1G125DCKR)
* DB25 Backshell (x1) (DKPN: 970-25BPE-ND PN: 970-025-010R011)
* Level shifter PCB (x1)
* Saturn controller plug (x2)
## Cable schematic
 [https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/Saturn.pdf](https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/Saturn.pdf)
## Cable PCB build instruction
![](img/cables/saturn.png)
* Solder 74AHCT1G125 to footprint highlighted in red.
* Connect cords according to schematic.
* Bridge LO side of jumper I39.
# Nintendo 64 adapter cable
## Pinout reference
![](img/cables/n64_pinout.png)
## Bill of materials
* DB25 Male solder cup (x1) (DKPN: AE10984-ND PN: A-DS 25 LL/Z)
* DB25 Backshell (x1) (DKPN: 970-25BPE-ND PN: 970-025-010R011)
* Passthrough PCB (x1)
* N64 controller plug (x4)
## Cable schematic
 [https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/N64.pdf](https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/N64.pdf)
## Cable PCB build instruction
![](img/cables/n64.png)
* Connect cords according to schematic.
* Bridge HI side of jumper I39.
# Dreamcast adapter cable
## Pinout reference
![](img/cables/dreamcast_pinout.png)
## Bill of materials
* DB25 Male solder cup (x1) (DKPN: AE10984-ND PN: A-DS 25 LL/Z)
* DB25 Backshell (x1) (DKPN: 970-25BPE-ND PN: 970-025-010R011)
* Passthrough PCB (x1)
* Dreamcast controller plug (x4)
## Cable schematic
 [https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/Dreamcast.pdf](https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/Dreamcast.pdf)
## Cable PCB build instruction
![](img/cables/dc.png)
* Connect cords according to schematic.
* Bridge HI side of jumper I39.
# GameCube adapter cable
## Pinout reference
![](img/cables/gamecube_pinout.png)
## Bill of materials
* DB25 Male solder cup (x1) (DKPN: AE10984-ND PN: A-DS 25 LL/Z)
* DB25 Backshell (x1) (DKPN: 970-25BPE-ND PN: 970-025-010R011)
* Passthrough PCB (x1)
* GameCube controller plug (x4)
## Cable schematic
 [https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/GameCube.pdf](https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/GameCube.pdf)
## Cable PCB build instruction
![](img/cables/gc.png)
* Connect cords according to schematic.
* Bridge LO side of jumper I39.
# JVS adapter cable
## Bill of materials
* DB25 Male solder cup (x1) (DKPN: AE10984-ND PN: A-DS 25 LL/Z)
* DB25 Backshell (x1) (DKPN: 970-25BPE-ND PN: 970-025-010R011)
* 74AHCT1G125 SC70-5 (x1) (DKPN: 296-4709-1-ND PN: SN74AHCT1G125DCKR)
* Step Up 5V (x1) (DKPN: 296-24519-1-ND PN: TPS61240DRVT)
* Inductor (x1) (DKPN: 490-4026-1-ND PN: LQM21FN1R0N00D)
* RS485 PHY (x1) (DKPN: 296-50395-1-ND PN: THVD1450DR)
* Resistor 10K (x2) (DKPN: 311-10.0KLRCT-ND PN: RC0402FR-0710KL)
* Capacitor 0.1u (x1) (DKPN: 490-6328-1-ND PN: GRM155R71C104KA88J)
* Capacitor 2.2u (x1) (DKPN: 1276-1085-1-ND PN: CL10A225KP8NNNC)
* Capacitor 4.7u (x1) (DKPN: 1276-1044-1-ND PN: CL10A475KP8NNNC)
* JVS PCB (x1)
* USB-A plug (x1)
## Cable schematic
[https://github.com/darthcloud/BlueRetroHW/blob/master/Cables/jvs/jvs.pdf](https://github.com/darthcloud/BlueRetroHW/blob/master/Cables/jvs/jvs.pdf)
## Cable PCB build instruction
![](img/cables/jvs_f.png)
* Connect cords according to schematic.
* PCB jumper are already set nothing to do.
* Do not install R4, R3 & D1.