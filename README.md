# FirmwareUpdateTool
Python-based Firmware Update tool for Piera IPS and A-Series Canaree sensors
Updated 11/2/2021

This software is used to update firmware on Piera IPS-Series Sensors currently running v1.9.9 to version v1.9.10.  It is designed to be used with Piera Evaluation Kit (PEK) USB Cables or other compatable SiLab CP2102-based USB to UART Adapters. 
This update is not for prior versions of Piera IPS Sensors running Version 1.8.x or below.

When running the program, it will detect Piera devices connected to your computers USB Port and prompt you to select a device to update.
Once selected, the program will detect the version of firmware currently running on your device, and if necissary update it to v1.9.10
Once the update is successfull, it may also load new sensor calibration settings if that is required for your sensor.

Please run Flasher once for each IPS Sensor you wish to update. 
After the upgrade the IPS-Sensor will reboot with the factory configuration.

The software is designed to run and has been tested on Windows 10 (x86/x64-based) platforms. 
