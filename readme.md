# DosBox for OPL2 Audio Board
This repository contains a version of DosBox SVN 0.74 that supports OPL2 passthrough to the OPL2 Audio Board over serial port. Install the accompanying Arduino sketch on your Arduino and enjoy real OPL2 audio from DosBox!

* For build instructions see [https://www.dosbox.com/wiki/BuildingDOSBox](https://www.dosbox.com/wiki/BuildingDOSBox)
* To get the OPL2 Audio Board library go to [https://github.com/DhrBaksteen/ArduinoOPL2](https://github.com/DhrBaksteen/ArduinoOPL2)
* More info on the OPL2 Audio Board can be found here: [https://www.tindie.com/products/DhrBaksteen/opl2-audio-board/](https://www.tindie.com/products/DhrBaksteen/opl2-audio-board/)

## Configuration
After compiling the source run DosBox to create a default config file `dosbox-OPL2 Audio Board.conf`.
The configuration for the OPL2 Audio Board is part of the `[sblaster]` section. Set `oplemu` to `opl2board` and `oplport` to the port where your Arduino + OPL2 board is connected. For example `COM4`. By setting `oplemu=opl2board` the `oplmode` will automatically be set to `opl2` no matter what value you set.
