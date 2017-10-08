# Creality-CR-10
Stuff for my Creality CR-10 3D Printer.


## Flashing

*bootloader*:

    avrdude -p m1284p -c usbasp-clone -P usb -U flash:w:optiboot_atmega1284p.hex:i
   
*Marlin* via Arduino:

    avrdude -p m1284p -c arduino -P /dev/ttyUSB2 -U flash:w:Marlin.hex:i
    
*Marlin* via USBasp:

    avrdude -p m1284p -c usbasp-clone -P usb -U flash:w:Marlin.hex:i
