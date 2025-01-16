# Marlin-2.1.2.5-SKR-V1.3-UM2Go

Marlin 2.1.2.5 Settings for BIGTREE SKR 1.3, TMC2130 to drive Ultimaker UM2GO 3D Printer.

Repo contains updated files to reflect changes in
- configuration.h
- configuration_adv.h
- pins_BT_SKR_c ommon.h

Search for "rudy" to find all modifications

Changelog:

Enabled TMC2130 in SPI mode 
Stealthcop
32 microstepping
Sensorless homing on X/Y axis
Hotend fan is enabled via fan connector
Print fan is enabled via heater 1 connector (he1)
Hotend temp sensor is moved to temp2 port (hardware issue of my board)	
Enabled hot bed heating 
Enabled ulticontroller display and Clickwheel+LEDs as published by Anthrix https://community.ultimaker.com/topic/30786-ultimaker-with-skr-14/
Enabled bed callibration 


To do:

Add caselight 24v leds feature using spare signal pin and transistor / or extruder 1 output
Hotend PWM callibration (temp is overshooted)
Callibrate fans PWM values (hotend fan is jittering)
