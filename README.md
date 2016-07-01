###GRBL_LCD
*grbl version 0.9j

###IMPORTANT NOTE:
This version of GRBL is made to run with a larger amount of RAM and is made for use with the Arduino mega2560.

This version utilizes a modified version of the Arduino LiquidCrystal library added to the final build, this causes
an increase in the total size of the final build. A heavily modified version may be made for use with the Arduino UNO
but there is no plan to do as at the moment.

The LCD is connected to the Arduino mega2560's pins like such
* Pin 44 - LCD RS
* Pin 45 - LCD reset
* Pin 46 - LCD D4
* Pin 47 - LCD D5
* Pin 48 - LCD D6
* Pin 49 - LCD D7
The LCD power, contrast and backlight has to be controlled by seperate circuitry

The main change is within the following files (Compared to the main version)
* report.c
* main.c

Further changes will be made to other files because this version is being made with intent to be used with a 2 axis CNC laser cutter.
These changes are in the general configuration files, and may be easily reverted later on for use with other projects.