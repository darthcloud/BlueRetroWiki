# Table of contents
* [FC / NES adapter cable](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-Cables-Build-Instructions#fc--nes-adapter-cable)
* [SFC / SNES adapter cable](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-Cables-Build-Instructions#sfc--snes-adapter-cable)
* [Saturn adapter cable](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-Cables-Build-Instructions#saturn-adapter-cable)
* [Nintendo 64 adapter cable](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-Cables-Build-Instructions#nintendo-64-adapter-cable)
* [Dreamcast adapter cable](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-Cables-Build-Instructions#dreamcast-adapter-cable)
* [GameCube adapter cable](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-Cables-Build-Instructions#gamecube-adapter-cable)
* [JVS adapter cable](https://github.com/darthcloud/BlueRetro/wiki/BlueRetro-Cables-Build-Instructions#jvs-adapter-cable)
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
![](img/cables/fc_pinout.png)
## Cable PCB build instruction
![](img/cables/nes.png)
* Solder 74AHCT1G125 to footprint highlighted in red.
* Bridge HI side of jumper I39.
* Connect pad DIR3 & DIR1 to GND.
* For using PAL system, add 3.6K pull-ups to NES 5V (pin 5) on pads IO18, IO5 & IO32.
* Connect cords according to table below and pinout reference.

PCB PAD | Cord | Pin | Name | Use | Required?
------- | ---- | --- | ---- | --- | ---------
VIN | NES P1 | 5 | 5V | BlueRetro Power | Yes
GND | NES P1 | 1 | GND | BlueRetro Power | Yes
IO32 | NES P1 | 3 | OUT0 | Latch for all accessories | Yes
IO19 | NES P1 | 4 | P1_D0 | Player 1 / Four Score DATA | Yes
IO5 | NES P1 | 2 | P1_CUP | Player 1 / Four Score CLK | Yes
VIN | NES P2 | 5 | 5V | BlueRetro Power | No
GND | NES P2 | 1 | GND | BlueRetro Power | No
IO22 | NES P2 | 4 | P2_D0 | Player 2 / Four Score DATA | No
IO18 | NES P2 | 2 | P2_CUP | Player 2 / Four Score CLK | No
IO21 | FC_DB15 | 13 | P1_D1 | FC 4P adapter P3 DATA | No
IO25 | FC_DB15 | 7 | P2_D1 | FC 4P adapter P4 DATA | No
# SFC / SNES adapter cable
## Bill of materials
* DB25 Male solder cup (x1) (DKPN: AE10984-ND PN: A-DS 25 LL/Z)
* 74AHCT1G125 SC70-5 (x9) (DKPN: 296-4709-1-ND PN: SN74AHCT1G125DCKR)
* 3.6K resistors (x5) (DKPN: ‎S3.6KCACT-ND‎ PN: RNMF14FTC3K60‎) (Required for PAL system only)
* DB25 Backshell (x1) (DKPN: 970-25BPE-ND PN: 970-025-010R011)
* Level shifter PCB (x1)
* SNES controller plug (x2)
## Cable schematic
 [https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/SNES.pdf](https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/SNES.pdf)
## Pinout reference
![](img/cables/snes_pinout.png)
## Cable PCB build instruction
![](img/cables/snes.png)
* Solder 74AHCT1G125 to footprint highlighted in red.
* Bridge LO side of jumper I39.
* Connect pad DIR3 & DIR1 to GND.
* For using PAL system, add 3.6K pull-ups to SNES 5V (pin 1) on pads IO23, IO18, IO5, IO32 & IO26.
* Connect cords according to table below and pinout reference.

PCB PAD | Cord | Pin | Name | Use | Required?
------- | ---- | --- | ---- | --- | ---------
VIN | SNES P1 | 1 | 5V | BlueRetro Power | Yes
GND | SNES P1 | 7 | GND | BlueRetro Power | Yes
IO5 | SNES P1 | 2 | P1_CLK | Player 1 / Multitap 1 CLK | Yes
IO32 | SNES P1 | 3 | LATCH | Latch for all accessories | Yes
IO19 | SNES P1 | 4 | P1_D0 | Player 1 / Multitap 1 DATA | Yes
IO21 | SNES P1 | 5 | P1_D1 | Multitap 1 DATA | No
IO23 | SNES P1 | 6 | P1_SEL | Multitap 1 CTRL | No
VIN | SNES P2 | 1 | 5V | BlueRetro Power | No
GND | SNES P2 | 7 | GND | BlueRetro Power | No
IO18 | SNES P2 | 2 | P2_CLK | Player 2 / Multitap 2 CLK | No
IO22 | SNES P2 | 4 | P2_D0 | Player 2 / Multitap 2 DATA | No
IO25 | SNES P2 | 5 | P2_D1 | Multitap 2 DATA | No
IO26 | SNES P2 | 6 | P2_SEL | Multitap 2 CTRL | No
# Saturn adapter cable
## Bill of materials
* DB25 Male solder cup (x1) (DKPN: AE10984-ND PN: A-DS 25 LL/Z)
* 74AHCT1G125 SC70-5 (x14) (DKPN: 296-4709-1-ND PN: SN74AHCT1G125DCKR)
* DB25 Backshell (x1) (DKPN: 970-25BPE-ND PN: 970-025-010R011)
* Level shifter PCB (x1)
* Saturn controller plug (x2)
## Cable schematic
 [https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/Saturn.pdf](https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/Saturn.pdf)
## Pinout reference
![](img/cables/saturn_pinout.png)
## Cable PCB build instruction
![](img/cables/saturn.png)
* Solder 74AHCT1G125 to footprint highlighted in red.
* Bridge LO side of jumper I39.
* Connect pad DIR0, DIR2, DIR1 & DIR4 to GND.
* Connect cords according to table below and pinout reference.

PCB PAD | Cord | Pin | Name | Use | Required?
------- | ---- | --- | ---- | --- | ---------
VIN | SATURN P1 | 1 | 5V | BlueRetro Power | Yes
GND | SATURN P1 | 9 | GND | BlueRetro Power | Yes
IO5 | SATURN P1 | 2 | P1_D | Player 1 D1 | Yes
IO3 | SATURN P1 | 3 | P1_U | Player 1 D0 | Yes
I35 | SATURN P1 | 4 | P1_TH | Player 1 CTRL | Yes
IO27 | SATURN P1 | 5 | P1_TR | Player 1 CTRL | Yes
IO26 | SATURN P1 | 6 | P1_TL | Player 1 CTRL | Yes
IO23 | SATURN P1 | 7 | P1_R | Player 1 D3 | Yes
IO18 | SATURN P1 | 8 | P1_L | Player 1 D2 | Yes
VIN | SATURN P2 | 1 | 5V | BlueRetro Power | No
GND | SATURN P2 | 9 | GND | BlueRetro Power | No
IO21 | SATURN P2 | 2 | P2_D | Player 2 D1 | No
IO19 | SATURN P2 | 3 | P2_U | Player 2 D0 | No
I36 | SATURN P2 | 4 | P2_TH | Player 2 CTRL | No
IO16 | SATURN P2 | 5 | P2_TR | Player 2 CTRL | No
IO33 | SATURN P2 | 6 | P2_TL | Player 2 CTRL | No
IO25 | SATURN P2 | 7 | P2_R | Player 2 D3 | No
IO22 | SATURN P2 | 8 | P2_L | Player 2 D2 | No
# Nintendo 64 adapter cable
## Bill of materials
* DB25 Male solder cup (x1) (DKPN: AE10984-ND PN: A-DS 25 LL/Z)
* DB25 Backshell (x1) (DKPN: 970-25BPE-ND PN: 970-025-010R011)
* Passthrough PCB (x1)
* N64 controller plug (x4)
## Cable schematic
 [https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/N64.pdf](https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/N64.pdf)
## Pinout reference
![](img/cables/n64_pinout.png)
## Cable PCB build instruction
![](img/cables/n64.png)
* Bridge HI side of jumper I39.
* Connect cords according to table below and pinout reference.
# Dreamcast adapter cable
## Bill of materials
* DB25 Male solder cup (x1) (DKPN: AE10984-ND PN: A-DS 25 LL/Z)
* DB25 Backshell (x1) (DKPN: 970-25BPE-ND PN: 970-025-010R011)
* Passthrough PCB (x1)
* Dreamcast controller plug (x4)
## Cable schematic
 [https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/Dreamcast.pdf](https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/Dreamcast.pdf)
## Pinout reference
![](img/cables/dreamcast_pinout.png)
## Cable PCB build instruction
![](img/cables/dc.png)
* Bridge HI side of jumper I39.
* Connect cords according to table below and pinout reference.
# GameCube adapter cable
## Bill of materials
* DB25 Male solder cup (x1) (DKPN: AE10984-ND PN: A-DS 25 LL/Z)
* DB25 Backshell (x1) (DKPN: 970-25BPE-ND PN: 970-025-010R011)
* Passthrough PCB (x1)
* GameCube controller plug (x4)
## Cable schematic
 [https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/GameCube.pdf](https://github.com/darthcloud/BlueRetroHW/blob/master/DIY/GameCube.pdf)
## Pinout reference
![](img/cables/gamecube_pinout.png)
## Cable PCB build instruction
![](img/cables/gc.png)
* Bridge LO side of jumper I39.
* Connect cords according to table below and pinout reference.
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
* PCB jumper are already set nothing to do.
* Do not install R4, R3 & D1.
* Connect cords according to table below and pinout reference.