# Marlin-2.1.2.5-SKR-V1.3-UM2Go

Marlin 2.1.2.5 Settings for BIGTREE SKR 1.3, TMC2130 to drive Ultimaker UM2GO 3D Printer.

Repo contains updated files to reflect changes in
- configuration.h
- configuration_adv.h
- pins_BT_SKR_c ommon.h
- pins_BTT_SKR_V1_3

Search for "rudy" to find all modifications in code.

Hardware:
- Ultimaker 2 Go frame
- Heated bed
- Aftermarket UM2+ Olsson Block hotend for 1.75mm filament
- 1.75mm extruder
- 24v ultimaker OEM PSU
- 2x Thermistor NTC100K in PT100 casing (head and bed)
- Ultimaker 2 + fan bracket
- Blue teflon tube
- SKR 1.3
- TMC2130
- Um2 Oled with SR reader
- Custom expansion PCB for Power, USB, Swith to fit case slots (UM board layout)
- Sliders With Copper Sleeve + Slider Block Spring
- Print head carriage with Igus Drylin polymer busings + Igus 6mm rods
- Left physical endstop switches

Software:

- Enabled TMC2130 in SPI mode
- Stealthcop enabled
- 16 microstepping for X/Y/Z axis
- 32 microstepping for E
- Hotend auto fan (5v) is enabled via servo connector
- Print fan is enabled via heater 1 connector (he1)
- Hotend temp sensor is moved to temp2 port (hardware issue on my board)
- Enabled heated bed
- Enabled ulticontroller display and Clickwheel+LEDs as published by Anthrix https://community.ultimaker.com/topic/30786-ultimaker-with-skr-14/
- Enabled bed callibration submenu
- Enabled bed taming option
- Enabled PID callibration submenu
- Enabled Eeprom
- Enabled Z babysteps submenu
- Motors Current set at around 500mah
- Decreased Acceleration and jerk values
- Enabled Lights submenu
- Case lights are enabled via Fan connector
- Added more preheat profiles
- Enabled pint counter
- Enabled print fail recovery

Hotend PID values in config are left stock Marlin ones (callibrated via lcd)

ToDo:

- Add motherboard cooling fan
- Add bed leveling sensor
- Switch from glass to magnetic PEI build plate (ordered from aliexpress)
- Filament sensor
- Add WiFi
- Maybe Octoprint + camera

_____________________________________________________________________________________________________________________________

Marlin 2.1.2.5

This is a minor release bringing over some changes from the latest development branch. Configurations have been patched up to allow for a more complete binary deployment.

Example Configurations for many machines are posted at:
https://github.com/MarlinFirmware/Configurations/tree/release-2.1.2.5

Binaries of this release can be found at:
https://github.com/MarlinFirmware/MarlinBuilds/tree/release-2.1.2.5


Changes
🩹 Fix STM32 CPU serial UUID (#26715, #26727, #26737)
🐛 Fix skipping of G2/G3 E-only moves
🐛 Update and patch some pins files
📝 Update some config links and defaults
🔨 Update build and other supporting scripts
🔨 Add mega1281 specific build environment
🔨 Update to the newest Simulator
🧑‍💻 Update to the newest Pins Debugging
