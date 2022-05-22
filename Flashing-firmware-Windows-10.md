# Flashing firmware Windows 10

1. Download the [Flash Download Tools](https://www.espressif.com/en/support/download/other-tools) and unzip.
2. Execute flash_download_tool_x.y.z.exe\
   ![](img/flash_tool.png)
3. Select develop Mode\
   Select ESP32 DownloadTool\
   ![](img/flash_mode.png)
4. Select and check the 3 binary file in the first 3 field and match the option as in screenshot.\
   An universal version with system auto detection is provided in addition to system hard-coded versions.\
   In order each bin offset are: 0x1000, 0x8000, & 0x10000.\
   ![](img/flash_config.png)
5. Select proper COM port for your machine.
6. Press START
7. Wait for status to change to FINISH.
