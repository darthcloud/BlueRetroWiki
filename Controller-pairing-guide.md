# Table of contents

* [PS3](#ps3)
* [PS4 & PS5](#ps4--ps5)
* [Xbox One S, Series X|S & Adaptive controller](#xbox-one-s--adaptive-controller)
* [Wii & WiiU Pro](#wii--wiiu-pro)
* [Switch Pro & Joycon](#switch-pro--joycon)
* [8bitdo](#8bitdo)

# PS3

* Note only official PS3 controller are supported.

## First pairing

### Windows

1. Download and install [Sixaxis Pair Tool](https://sixaxispairtool.en.lo4d.com/windows#:~:text=The%20Sixaxis%20Pair%20Tool%20is,games%20with%20your%20PS3%20controller.)
2. Get your BlueRetro/ESP32 BDADDR (MAC) from the serial log (See this [guide](https://github.com/darthcloud/BlueRetro/wiki/Getting-BlueRetro-debug-logs-via-Serial-port-Windows-10) to setup serial log)
```
# bt_hci_cmd_read_bd_addr
# BT_HCI_EVT_CMD_COMPLETE
# local_bdaddr: 84:0D:8E:E6:5A:56
```
3. Connect your PS3 controller to PC using USB cable.
4. Launch Sixaxis pair tool and type in the address found in step #2.\
![](img/SixaxisPairTool_v0FDiegEiq.png)
5. Click update, once done disconnect the controller from PC.
6. Boot up BlueRetro and press the PS button, the controller should connect to BlueRetro.

## Reconnect

1. Simply press PS button to reconnect to BlueRetro.
# PS4 & PS5

## First pairing

1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing)
2. Press & hold simultaneously Share & PS buttons until the LED blink white.
3. Color on controller will change once pairing is complete.

## Reconnect

1. Simply press PS button to reconnect to BlueRetro.

# Xbox One S, Series X|S & Adaptive controller
As of v1.2.1 the minimum required Xbox FW for controller are:\
Xbox One S: 4.8.1923.0\
Adaptive: 4.5.1680.0\
Series X|S: 5.9.2709.0

Update via the [Xbox accessories Win10 app](https://www.microsoft.com/en-us/p/xbox-accessories/9nblggh30xj3).

## First pairing

1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing)
2. Power on controller via Xbox button and then hold the black sync button until the logo blink.
3. Logo will stop blinking on controller once pairing is complete.

## Reconnect

1. Simply hold Xbox button for a small moment to power on controller and it will reconnect to BlueRetro.

# Wii & WiiU Pro
* 1+2 pairing is not supported.

## First pairing

1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing)
2. Press red Sync button
3. LEDs will stop blinking on controller once pairing is complete.

## Reconnect

1. Simply press any button on controller and it will reconnect to BlueRetro.

# Switch Pro & Joycon

## First pairing

1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing)
2. Press and hold sync button until LEDs move in a left/right pattern.
3. LEDs will stop pattern on controller once pairing is complete.

## Reconnect
1. Simply press any button twice on controller and it will reconnect to BlueRetro.

# 8bitdo
As of v1.2.1 the minimum required 8bitdo FW for controller are:\
SF30: v1.37\
Gbros adapter: v2.25

Update via the [8bitdo Win10 app](https://www.microsoft.com/en-us/p/xbox-accessories/9nblggh30xj3).

## First pairing

1. Boot up BlueRetro and make sure adapter is in inquiry mode (LED pulsing)
2. Power up 8bitdo controller in Xinput mode (Start + X or set switch to X) (Only Xinput mode supported!!)
2. Press and hold sync button until LEDs flash.
3. LEDs will stop pattern on controller once pairing is complete.

## Reconnect
1. Simply press Start on controller and it will reconnect to BlueRetro.