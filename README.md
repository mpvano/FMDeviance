## FMDeviance
A simple GnuRadio and RTL-SDR based NBFM Deviation meter

The only prerequisits are that you have a recent version of GnuRadio installed that includes the OsmoSDR support for SDR radios, and that you have a properly installed RTL-SDR.com Version 3 or 4 library.

This may work with other radios that OsmoSDR supports, but I've only tested it with the official RTL-SDR.com version 3 and 4 dongles.

The only problem I've encountered in moving it between different platforms is that the Low Pass filter module may report that it can't find it's windowing options because sometimes they have different suffixes on different platforms. To fix this, open the module and pop up the selector for the windowing option and select the one with the corresponding names. This is easier than it sounds - the names are obvious...

## Disclaimers

I designed this experimental NBFM Deviation meter as an aid to operation and experimentation. It is not designed to be highly accurate or foolproof. It works well when used as intended. Be careful not to destroy your receiver input by having the Radio antennas too close together!

This software was only made possible thanks to the excellent work done the Gnu Radio team and the rest of the community!

Mario Vano AE0GL

![Flow](Images/deviation.pdf)

![APRS](Images/deviation.pdf)

