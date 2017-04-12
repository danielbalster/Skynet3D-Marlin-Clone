# Skynet3D-Marlin-Clone

This is my version of 
- Marlin firmware project (https://marlinfw.org)
- Modified by Skynet3D (https://facebook.com/Skynet3Dfirmwaredevelopment)
- Thingiverse LCD12864 modification (http://www.thingiverse.com/thing:2103748)

for my ANet A8 printer. Configuration is
- Automatic Bed Levelling
- LCD12864
- check configuration.h

# My contributions

## Automatic Bed Measure


# Installation

- copy anet folder into your hardware folder (in your Arduino installtion root, ie c:\programs\arduino\hardware\anet)
- open the sketch from the Skynet3D-Marlin-Clone folder
- export compiled binary firmware (Skynet3D-Marlin-Clone.ino.sanguino.hex)
- copy to target system connected with your printer
- avrdude -v -p atmega1284p -c arduino -P /dev/ttyUSB0 -b 57600 -D -Uflash:w:Skynet3D-Marlin-Clone.ino.sanguino.hex:i

done.
