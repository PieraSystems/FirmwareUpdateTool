# FirmwareUpdateTool
Python-based Firmware Update tool for Piera IPS and A-Series Canaree sensors
Updated 12/17/2021 - Version 1.9.12 

This software is used to update firmware on Piera IPS-Series Sensors currently running v1.9.9 or older -  It is designed to be used with Piera Evaluation Kit (PEK) USB Cables or other compatable SiLab CP2102-based USB to UART Adapters. This update is not for prior versions of Piera IPS Sensors running Version 1.8.x or below.

When running the program, it will detect Piera devices connected to your computers USB Port and prompt you to select a device to update.
Once selected, the program will detect the version of firmware currently running on your device, and if needed update it to v1.9.12
Once the update is successfull, it may also load new sensor calibration settings if that is required for your sensor.

The software is designed to run and has been tested on Windows 10 (x86/x64-based) platforms. 
- To run the software, extract the [ZIP file](https://github.com/PieraSystems/FirmwareUpdateTool/releases/download/v1.9.12/flasher-1.9.12.zip) and launch flasher.exe application.
- Follow instruction on screen, DO NOT Disconnect your Piera device while upgrade is in progress.
- If you run into any issues, disconnect Piera device, Reconnect it, and run flasher.exe again.


Please run Flasher once for each IPS Sensor you wish to update. 
After the upgrade the IPS-Sensor will reboot with the factory configuration.


The following shows the typical output when running Flasher successfully
--------

D:\Piera-Dev\flasher>flasher.exe
IPS Update Tool v1.1
 Exit - Ctrl-C

 1: COM7

Selection: 1

Version found:
v1.9.9 (COM11)

Press Enter to update device or Ctrl-C to exit...

Entering boot loader...
Sending file, please wait...
File sent.
Updating settings for IPS7100-21H000085

...........................................

Update complete. Press Enter key to exit.

--------

If "No Sensor found" Message is seen, ensure the Piera IPS-Sensor or Canaree A-Series is properly connected to your PC and recognised as a USB Device.  On some systems is maybe necissary to install a driver from SiLabs.  Follow the instructions below 


D:\Piera-Dev\flasher>flasher.exe
IPS Update Tool v1.1
 Exit - Ctrl-C
No sensor found, press any key to exit...

Download the Universal Windows Driver from SiLabs.com.
 https://www.silabs.com/documents/public/software/CP210x_Universal_Windows_Driver.zip
Right-click on CP210x_Universal_Windows_Driver.zip, choose "Extract All..." and then "Extract".
Enter the CP210x_Universal_Windows_Driver folder and run CP210xVCPInstaller_x64.exe.
Follow instructions in Installation Wizard to complete installation.
Re-Run flasher.exe to update your device. 

For more information visit us at www.pierasystems.com/support 
