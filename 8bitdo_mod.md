# 8BitDo GC ModKit No-Connect on Charge Mod

The 8BitDo GC ModKit has the annoying behavior of powering on and trying to connect to the last Bluetooth device when connected for charging.

If you use the GameCube internal mod, this is annoying because it will trigger the console to power on.

This page details how to modify the 8BitDo ModKit to disable the connect-on-charge feature.  
After this mod, the ModKit will only power on with the Start button.

## Disconnect USB VBUS from Power-On Logic Circuit

Cut the trace near the power-on circuitry as indicated by the red line:  
![](img/gc_modkit_pwr_on.png)

Simply performing this step is enough to remove the connect-on-charge behavior.

## Restoring the Charge LED (Optional)

The charge LED is controlled by the ModKit MCU. Since it won't power on anymore, the LED will no longer light up.  
(Actually, even unmodded, if you turn off the ModKit with Start while charging, the LED turns off!)

Unfortunately, the LEDs are configured as a current source rather than a current sink (as suggested by the TP4056 datasheet).  
So we need to use an inverter to reverse the logic of the charge pin.

### Parts Needed:
* TTL Inverter SN74AHCT1G04DBVR ([Digikey](https://www.digikey.ca/en/products/detail/texas-instruments/SN74AHCT1G04DBVR/276756))
* 2x 2KΩ resistors 1/8W ([Digikey](https://www.digikey.ca/en/products/detail/stackpole-electronics-inc/CF18JT2K00/1741658))

### Steps:
1. Remove the resistor pointed to by the red arrow near the TP4056 charge IC.  
   ![](img/gc_modkit_charger.png)
2. Cut the trace marked by the red line near the TP4056 charge IC.  
   ![](img/gc_modkit_charger.png)
3. Remove the resistor pointed to by the red arrow near the charge cable port.  
   ![](img/gc_modkit_led.png)
4. Scratch the solder mask where the red circle is. This will be the GND connection for inverter pin 3.  
   The VBUS connection for pin 5 will be the pad pointed to by the red arrow.  
   ![](img/gc_modkit_ic.png)
5. Solder the inverter onto the ModKit PCB as shown below.  
   ![](img/gc_modkit_mod.png)
6. Solder a resistor between pin 4 and pin 7 of the TP4056 charge IC.
7. Solder a wire between pin 7 of the TP4056 charge IC and pin 2 of the inverter.
8. Solder a resistor between pin 4 of the inverter and the pad near the charge connector port.  
   ![](img/gc_modkit_led_mod.png)

This completes the mod for restoring the charge LED.
