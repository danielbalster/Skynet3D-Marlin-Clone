# Skynet3D-Marlin-Clone

Purpose:
Add automatic bed measuring as a feature. idea is to use the ABL feature to detect the end of the heated bed in XY direction.

- you have a metallic/aluminium hotbed 
- you have an inductive z endstop sensor
- first it will home to the somewhat center
- then it will crawl into -X direction until the Z-endstop sensor is triggered (because it's floating without hotbend below)
- repeat for +X, -Y and +Y direction
- gather all absolute positions
- now we can calculate the somewhat exact extends of the hotbed and the correct center/origin/etc from it

FEATURE IS STILL WIP - DON'T USE


1. download Skynet3D from facebook.com/Skynet3Dfirmwaredevelopment
2. unzip
3. open contained arduino IDE
4. clone this repository into that folder
5. open the sketch from this repository (Skynet3D-Marlin-Clone.ino)
6. export compiled binary firmware (Skynet3D-Marlin-Clone.ino.sanguino.hex)
7. copy to target system connected with your printer
8. avrdude -v -p atmega1284p -c arduino -P /dev/ttyUSB0 -b 57600 -D -Uflash:w:Skynet3D-Marlin-Clone.ino.sanguino.hex:i

done.
