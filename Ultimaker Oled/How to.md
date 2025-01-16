According to 
https://community.ultimaker.com/topic/30786-ultimaker-with-skr-14/?do=findComment&comment=260276

Slice cable to extend 3 wires and make connection to different location.

that will be 3.3v - power, (SCL, SDA - this is your i2c communication for screen). 



Connectors  J2 - pins 6 and connector J3 - pin 4 this is where your i2c going.

J3 - pin 8 ,3.3v which is missing on skr side is exp 2 pin 8 you need to split and supply 3.3v from any pin on board, i did use from wi-fi interface. (i do use wi-fi connector (rx,tx) for octoprint. so 3.3v is free to use for screen if you planing to use esp3d then is couple other pins with 3.3v you could use one of them.)

i2c wire is very simple EXP1 port wire 6, 4.


After that just in marlin to enable ultimaker 2 controller.

Also PCA9632 led controller is supported by marlin so led also will be working. just enable in marlin.

