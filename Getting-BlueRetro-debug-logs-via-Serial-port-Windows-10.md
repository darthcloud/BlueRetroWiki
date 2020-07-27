# **When using DevKitC USB port for serial debug DO NOT CONNECT the 5V pin coming from game system. Power will be provided from USB**

## Getting BlueRetro debug logs via Serial port Windows 10
1. Download & install [PuTTY](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html) or use your favorite terminal emulator.
2. Select serial and set right COM port and set speed to 921600\
![](img/putty_lRphcbP80S.png)
3. In "Terminal" check "Implicit CR in every LF"\
![](img/putty_rU4TrkHm7S.png)
4. Back in session you may save those setting for later.
5. Click "Open"
6. Reproduce issue and copy the whole log to a .txt file.
7. Open issue in GitHub and attach file with write step for reproduction.