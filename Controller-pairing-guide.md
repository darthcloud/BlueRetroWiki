# PS3
* Note only official PS3 controller are currently supported.
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
5. Click update once done disconnect controller from PC.
6. Boot up BlueRetro and press the PS button, the controller shall connect to BlueRetro.
## Reconnect
1. Simply press PS button to reconnect to BlueRetro.