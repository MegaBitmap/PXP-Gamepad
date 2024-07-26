# PXP-Gamepad
 DIY universal controller pocket gamepad.

This is a open source wired controller/gamepad designed to be ultra portable.  
It uses a RP2040-Zero MCU soldered onto a custom PCB (see files).  
For firmware it uses GP2040-CE which can be downloaded from here:  
https://github.com/MegaBitmap/GP2040-CE/releases  

![gamepad](https://raw.githubusercontent.com/MegaBitmap/PXP-Gamepad/master/Images/gamepad.png)  
![render](https://raw.githubusercontent.com/MegaBitmap/PXP-Gamepad/master/Images/render.png)  
![pcb-front](https://raw.githubusercontent.com/MegaBitmap/PXP-Gamepad/master/Images/pcb-front.png)  
![pcb-back](https://raw.githubusercontent.com/MegaBitmap/PXP-Gamepad/master/Images/pcb-back.png)  
![schematic](https://raw.githubusercontent.com/MegaBitmap/PXP-Gamepad/master/Images/schematic.png)  


# 3D Print Settings

3MF Print files ready to be sliced can be downloaded from here:  
https://github.com/MegaBitmap/PXP-Gamepad/tree/master/3D_Files/3MF_Mesh  

If you have good first layer adhesion, disable brim.  
~0.13mm layer height  
Z seam alignment -> random  
The faceplate must be printed facing up with generate support enabled.  
The shoulder buttons need generate support enabled.  

The D-pad is split into two pieces to allow it to print without support.  
Use a dab of glue to attach the "D-pad-pin" with the pointy side facing out towards the PCB.  
The "D-pad-pin" prevents left and right or up and down from being pressed at the same time.  

After printing the faceplate and shoulder buttons, thoroughly remove all support material.  


# Parts List

1 x 3D Printed case and set of buttons (see files)  
https://github.com/MegaBitmap/PXP-Gamepad/tree/master/3D_Files/3MF_Mesh  

1 x PXP-GAMEPAD PCB (use Gerber files to order PCBs)  
https://jlcpcb.com/  

1 x RP2040-Zero Microcontroller  
https://www.waveshare.com/rp2040-zero.htm  

2 x PSP 3000 Joysticks (Alps Alpine RKJXU1210006)  
https://www.adafruit.com/product/3103  

7 x Screws (M2 x 8mm countersunk)  
https://www.ebay.com/itm/174466999302  

2 x FFC connectors 0.5mm pitch 4 pin bottom contacts (Cvilux CF20041D0R0-NH)  
https://www.digikey.com/en/products/detail/cvilux-usa/CF20041D0R0-NH/15792974  

2 x Right angle tact button switches (Panasonic EVQ-PUL02K)  
https://www.digikey.com/en/products/detail/panasonic-electronic-components/EVQ-PUL02K/286340  

14 x Tact button switches (TE Connectivity MSLPT5252BG2MTR)  
https://www.digikey.com/en/products/detail/te-connectivity-alcoswitch-switches/MSLPT5252BG2MTR/9686572  

(Optional) 3M dual lock for easy universal phone mounting.  (SJ3550 1 inch)  
https://www.ebay.com/itm/401127190632  

Make sure to use a high quality shielded USB C cable. (A to C or C to C)  


# Video Build Guide

Coming soon...


# Firmware Settings

[Download firmware here](https://github.com/MegaBitmap/GP2040-CE/releases).  
[Install it using this guide](https://gp2040-ce.info/installation/).  

In the web configurator -> Configuration -> Add-Ons -> Analog
Use these settings:  

Analog Stick 1 X Pin    = 27  
Analog Stick 1 Y Pin    = 26  
Analog Stick 1 Mode     = Left Analog  
Analog Stick 1 Invert   = X Axis  
Analog Stick 2 X Pin    = 29  
Analog Stick 2 Y Pin    = 28  
Analog Stick 2 Mode     = Right Analog  
Analog Stick 2 Invert   = X Axis  
Inner Deadzone Size (%) = 5  
Outer Deadzone Size (%) = 50  
Auto Calibration        = Enabled  

Then scroll to bottom -> Save -> Reboot -> Controller  

# Credits

GP2040-CE Multi-Platform Gamepad Firmware for RP2040  
https://github.com/OpenStickCommunity/GP2040-CE  

Better PSP Thumb Stick Analog Replacement
by limoncello-mozzarella is licensed under the Creative Commons - Attribution license.  
https://www.thingiverse.com/thing:3048385



