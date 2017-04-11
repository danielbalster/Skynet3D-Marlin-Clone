# Skynet3D-Marlin-Clone


# 1. download Skynet3D from facebook.com/Skynet3Dfirmwaredevelopment
# 2. unzip
# 3. open contained arduino IDE
# 4. clone this repository into that folder
# 5. open the sketch from this repository (Skynet3D-Marlin-Clone.ino)
# 6. export compiled binary firmware (Skynet3D-Marlin-Clone.ino.sanguino.hex)
# 7. copy to target system connected with your printer
# 8. avrdude -v -p atmega1284p -c arduino -P /dev/ttyUSB0 -b 57600 -D -Uflash:w:Skynet3D-Marlin-Clone.ino.sanguino.hex:i

done.
