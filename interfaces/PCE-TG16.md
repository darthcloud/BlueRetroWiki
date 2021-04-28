# PCE & TG16 controllers interface

The PCE interface is similar to how the Genesis work but a little bit simpler as it didn't need to be backward comaptible with anything else.
Eight inputs are multiplexed on four data lines (URDL) with a select line (SEL). An output enable line (/OE) disable the peripheral output and is used
as a latch or toggle to controller special peripheral like the multitap or the 6 buttons controller.

![](img/cables/pce_pinout.png)
