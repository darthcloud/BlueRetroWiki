# Introduction
BlueRetro aim to support as much device as possible by trying to follow what the HID descriptor
of unknown device report. You would expect this to be quite standard but device manufacturers
are quite good at making weird descriptor. BlueRetro HID parser got tested with only a few devices.
So quite often a device won't work because it's descriptor goes around the assumption I made in the
parser code.

To help me improve support sent me a Bluetooth HCI trace done on Windows 10!

# Software to install
* Download and install latest version of Wireshark:\
  You don't need to install any of the optional drivers when prompted\
  https://www.wireshark.org/#download
* Download and install latest version of Microsoft Bluetooth Test Platform:\
  https://learn.microsoft.com/en-us/windows-hardware/drivers/bluetooth/testing-btp-setup-package

# Trace examples
1. Always start the trace from a fresh state:\
  1.1. Remove the device from Windows if it had been paired previously:\
       ![](img/remove_paired.png)\
  1.2. Close all existing Wireshark opened window if any.\
  1.3. Close all existing Virtual Sniffer window if any.\
2. Open a windows cmd prompt and execute:
  ```
  C:\BTP\v1.14.0\x86\btvs.exe -Mode Wireshark
  ```
3. In the virtual sniffer window enable "Full Packet Logging"
4. Pair the device to Windows using the Bluetooth devices manager.
5. Press all the buttons on the controller one at a time taking note of the order you pressed them.
6. Stop the trace in Wireshark and save the trace.
7. Send me the .pcapng trace and your notes.

![](img/win10_bt_hci_trace.gif)