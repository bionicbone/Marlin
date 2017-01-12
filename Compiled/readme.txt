Usage:

1. Power off printer.
2. Press center button on panel.
3. Power up printer, please keep center button pressed.
4. Release center button.
5. Connect USB
6. Look up COM port from windows device manager. 

execute 
 
RC8 Under Test
==============
avrdude.exe -v -p atmega1284p -c arduino -P com6 -b 57600 -V -U flash:w:MarlinRC8_IncDec16Fixes_ABL_BiLinearMesh3x3_HooyHoo_Mount.hex


RC7 Reliable with OverHeat protection
===================================== 
avrdude.exe -v -p atmega1284p -c arduino -P com6 -b 57600 -V -U flash:w:MarlinRC7_ABL_HoolyHoo_Mount.hex