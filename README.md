## FMDeviance:

**_A Simple GnuRadio and RTL-SDR Based NBFM Deviation Meter_**

The only prerequisits are that you have a recent version of GnuRadio installed that includes the OsmoSDR support for SDR radios, and that you have a properly 
installed RTL-SDR.com Version 3 or 4 library.

### Display Controls

Hovering over the scope display will show the X and Y values at that point.

While hovering over a frozen scope display, the mouse wheel can be used to zoom the Y axis gain up or down. Of course, if you zoom out what you see will not display anything beyond the max_deviation setting.

You can also select a rectangular portion of the display with the left button. When you release the button, the display will zoom to the selection.

Clicking with the right button will restore the original zoom settings.

If you have a 3 button mouse, the middle button will pop up a menu of scope display parameters which can be modified. You can also save the scope display as a jpeg file. The "trigger" submenu allows switching to free running operation or altering the other triggering parameters.

Wayland based systems may output lengthy warnings to standard output that X windows features used by this popup menu may not be supported in the future. These are annoying, but they may safely be ignored and don't affect operation at this time.

### Compatibility

This may work with other radios that OsmoSDR supports, but I've only tested it with the official RTL-SDR.com version 3 and 4 dongles.

The only problem I've encountered in moving it between different platforms is that the Low Pass filter module may report that it can't find it's windowing options because sometimes they have different suffixes on different platforms. To fix this, open the module and pop up the selector for the windowing option and select the one with the corresponding names. This is easier than it sounds - the names are obvious...

### Disclaimers

I designed this experimental NBFM Deviation meter as an aid to operation and experimentation. It is not designed to be highly accurate or foolproof, or to be a high performance receiver. It works well when used as intended.

Be careful not to destroy your SDR receiver input by having the Radio and SDR antennas close together! HTs can produce quite high rf voltages in nearby equipment.

In some cases, you may need to use a power attenuator and/or sampling tap connecting the transmitter output and the SDR dongle to safely obtain a signal that is not leaking from earlier transmitter stages. 

This software was made possible thanks to the excellent work done by the Gnu Radio team and the rest of the community!

Mario Vano AE0GL

![Flow graph](Images/deviation.png)
![APRS](Images/APRSCapture.png)

