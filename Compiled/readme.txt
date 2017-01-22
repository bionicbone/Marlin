Usage:

1. Power off printer.
2. Press center button on panel.
3. Power up printer, please keep center button pressed.
4. Release center button.
5. Connect USB
6. Look up COM port from windows device manager. 

execute 
 
BiLinear 3x3 - RC8 BugFix (Jan 2017) Under Test
===============================================
avrdude.exe -v -p atmega1284p -c arduino -P com6 -b 57600 -V -U flash:w:MarlinRC8_IncJan17Fixes_ABL_BiLinearMesh3x3_HooyHoo_Mount.hex

3 Point - RC8 BugFix (Jan 2017) Under Test
==========================================
avrdude.exe -v -p atmega1284p -c arduino -P com6 -b 57600 -V -U flash:w:MarlinRC8_IncJan17Fixes_ABL_3Point_HooyHoo_Mount.hex

Mesh 7x7 - RC8 BugFix (Jan 2017) Under Test
==========================================
avrdude.exe -v -p atmega1284p -c arduino -P com6 -b 57600 -V -U flash:w:MarlinRC8_IncJan17Fixes_ABL_Mesh7x7_HooyHoo_Mount.hex


RC8 by Ghostface - RC 8 Only - No Fixes
=======================================
claims to have good results but is 100+ commits behind the latest bugfixes
avrdude.exe -v -p atmega1284p -c arduino -P com6 -b 57600 -V -U flash:w:Marlin_M150_RC8_v2_Ghostface.hex
M150 config RC8

-control
-- 
temperature

Autotemp: off
..

PID-P: 25.2
PID-I: 0.98
PID-D: 114
PID-C: 1.0

note: run PID tune to get correct values
.. 
your PLA and ABS pref here

pre-heat PLA
: fan: 0 - nozzle: 190 - 
bed: 55


pre-heat ABS
: fan: 0
 - nozzle: 240 - bed: 95


motion
accel: 800 - 
wx-jerk: 7 - 
wy-jerk: 6
 - vz-jerk: 0.40
 - ve-jerk: 5 - 
Vmax X: 300 - 
Vmax Y: 300 - 
Vmax Z: 5 - 
Vmax E: 25
             
Vmin: 0
 - VTrav min: 0 - 
Amax X: 1100 - 
Amax y: 1000 - 
Amax Z: 100 - 
Amax E: 10000 - 
A-retract: 3000
 - A-Travel: 3000
             
Xsteps/mm: 92.63 - 
Ysteps/mm: 92.63 - 
note: X and Y steps are for the default 17T plastic gears 16T is 100
             
Zsteps/mm: 1600.0 - 
Esteps/mm: 104 

-- filament 
E in mm³: off




RC7 Reliable with OverHeat protection and ABL with HoolyHoo mount
================================================================= 
avrdude.exe -v -p atmega1284p -c arduino -P com6 -b 57600 -V -U flash:w:MarlinRC7_ABL_HoolyHoo_Mount.hex

Original
========
avrdude.exe -v -p atmega1284p -c arduino -P com6 -b 57600 -V -U flash:w:Marlin_Original.hex