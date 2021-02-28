# Flashing firmware Windows 10
1. Download the [Flash Download Tools](https://www.espressif.com/en/support/download/other-tools) and unzip.
2. Execute flash_download_tool_3.8.5.exe\
![](img/explorer_iaheNf1C24.png)
3. Select Developer Mode\
![](img/flash_download_tool_3.8.5_TlqnyxB9Ji.png)
4. Select ESP32 DownloadTool\
![](img/flash_download_tool_3.8.5_WXhPGbf8md.png)
5. Select and check the 3 binary file in the first 3 field and match the option as in screenshot.\
\
Two types of build are now available: the SD card version as before (now named BlueRetro_universal_sd.bin) and also internal flash (SPIFFS). For each type I also provide the regular universal version with system auto detection. But in addition system hard-coded versions are available. A total of 24 variants are available.\
\
![](img/flash_download_tool_3.8.5_lBiiCrN3Gd.png)
6. Select proper COM port for your machine. (BlueRetro DevKit will show 2 COM, select 2nd one)\
   ([See this guide](https://github.com/darthcloud/BlueRetro/wiki/Missing-2nd-COM-port-Win10-BlueRetro-DevKit-fix) if only one show up)
7. Press START
8. Wait for status to change to FINISH.\
![](img/flash_download_tool_3.8.5_BDyWW8n9Wb.png)