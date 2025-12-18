## FMDeviance
_A simple GnuRadio and RTL-SDR based NBFM Deviation meter_

The only prerequisits are that you have a recent version of GnuRadio installed that includes the OsmoSDR support for SDR radios, and that you have a properly 
installed RTL-SDR.com Version 3 or 4 library.

## Display Controls

If you have a 3 button mouse, the middle button will pop up a menu of scope display parameters which can be modified. The "trigger" submenu allows switching to free running operation or altering the other triggering parameters.

Wayland based systems will output lengthy warnings to standard output that X windows features used by the popup may not be supported in the future. These may safely be ignored and don't affect the menu operation at this time.

## Compatibility

This may work with other radios that OsmoSDR supports, but I've only tested it with the official RTL-SDR.com version 3 and 4 dongles.

The only problem I've encountered in moving it between different platforms is that the Low Pass filter module may report that it can't find it's windowing options because sometimes they have different suffixes on different platforms. To fix this, open the module and pop up the selector for the windowing option and select the one with the corresponding names. This is easier than it sounds - the names are obvious...

## Disclaimers

I designed this experimental NBFM Deviation meter as an aid to operation and experimentation. It is not designed to be highly accurate or foolproof. It works well when used as intended. Be careful not to destroy your receiver input by having the Radio antennas too close together!

This software was made possible thanks to the excellent work done the Gnu Radio team and the rest of the community!

Mario Vano AE0GL

![Flow graph](Images/deviation.png)
![APRS](Images/APRSCapture.png)

