# Voron V2.4 Formbot Kit Building Instructions / Tipps
https://www.formbot3d.com/products/voron-24-r2-pro-corexy-3d-printer-kit-with-m8p-cb1-board-and-canbus-wiring-system?VariantsId=10457

## Building instructions
Start with the stock Voron 2.4 Manual https://github.com/VoronDesign/Voron-2/tree/Voron2.4/Manual
Be aware that the v2.4 Manual uses a 250mm Version of the v2, so some dimensions may seem wrong if you build a 300mm/350mm Version.

P. 25 v2.4 manual: If you build a bigger Version than a 250mm, you need more screws / m3-T-Nuts. Start from the outer holes in the rail and work your way towards the middle screwing the rail down every second hole.
The carriages are designed to slide along the rail easily. This unfortunately also includes sliding off the rails. Dropping the carriage likely irreparably damages it. ALWAYS put the little black rubber Carriage stoppers back on the rail (into the holes without screws) until your printer ist up and runnning!

P. 84 v2.4 manual: Skip this step, this part is not used and therefore probably not included in your printed parts.

P. 88 v2.4 manual: If you are building a 300mm machine you will need to start you screws from the second screw hole in the rails leaving the end holes open to allow space for T-nuts at later steps.
Small reminder: The carriages are designed to slide along the rail easily. This unfortunately also includes sliding off the rails. Dropping the carriage likely irreparably damages it. ALWAYS put the little black rubber Carriage stoppers back on the rail (into the holes without screws) until your printer ist up and runnning!

P. 101 v2.4 manual: Again, if you are building a bigger printer than the 250mm version, start at the outer holes and screw the rail down every second hole.
Small reminder (again): The carriages are designed to slide along the rail easily. This unfortunately also includes sliding off the rails. Dropping the carriage likely irreparably damages it. ALWAYS put the little black rubber Carriage stoppers back on the rail (into the holes without screws) until your printer ist up and runnning!

P. 104 v2.4 manual: As said before, the part on top of the right XY-Joint is not used with this kit. Use m5x10 BHCS like on the left XY-Joint to secure the X Axis to the XY-Joints.

P. 122 v2.4 manual: After you installed the Z-belts and squared the Gantry, make sure your AB belts are exactly the same length and have the exact same amount of teeth! Proceed with routing the AB-Belts, but be Aware that you will use a different X carriage as in the Voron 2.4 Manual.

P. 129-131 v2.4 manual: Skip these pages. Put the AB belts to the MGN12 Carriage with some tape, they dont have to be tight.

P. 143 v2.4 manual: X Carriage: After finishing the AB-Belts Routing, switch to the tap Manual. Optotap is used as the sensor. https://github.com/VoronDesign/Voron-Tap/tree/main/Manual
Be sure to take a look into the R8_errata.md document, it Highlights some important changes from the Manual and install the X Endstop switch.

P. 33 Tap Manual: After you have installed Tap successfully and have the AB belts fixed in the tap carriage, switch to page 146 of the Voron 2.4 manual or to https://github.com/VoronDesign/Voron-Stealthburner/tree/main/Manual
We will come back to install the Toolhead later.

P. 13 Stealthburner manual: You use a Toolhead PCB, so install these two heat inserts.

P. 14 Stealthburner manual: Skip

P. 30 Stealthburner manual: Follow this Video Guide on how to set the gear mesh on your CW2: https://github.com/VoronDesign/Voron-Stealthburner/tree/main/Manual
Follow this video on how to set the Anti-Squish as well: https://www.youtube.com/watch?v=L1gxBCiE0pk

P. 31 Stealthburner manual: Skip for now, we will install our Version of the Anchor later.

P. 34 Stealthburner manual: You dont need to fix the Cable Cover down with the m3x6 BHCS now, you will need to access this later.

P. 36-43 Stealthburner manual: All Hotends are mounted in a similar pattern and pretty self-explaining, your hotend mount and hotend will look different.

P. 46-51 Stealthburner manual: Be very careful with the cables, you can easily rip them off the LED PCB which leads to this LED and the following ones not working.

P. 53 Stealthburner manual: Be sure that your fan blows in the right Direction. Look at the arrows on the fan. Additionally, the Sticker on the fan is on the back pointing towards the Hotend. You want the fan to blow air into the hotend, not trying to pull the air out. This destroys your fan and your whole hotend mount because of heatcreep.

P. 56 Stealthburner manual: You dont need to screw the 5015 fan into the SB Face, you will install the SB0000 Fan PCB there later.

P. 58 Stealthburner manual: All parts of the Stealthburner are now pretty much finished. Now you will need to install the Can-Board on there and do some basic wiring. Switch to this manual: https://github.com/bigtreetech/EBB/tree/master/EBB%20SB2209%20CAN%20(RP2040)/Build%20Guide

P. 02 SB2209 manual: Now you need to screw down the 5015 fan with the SB0000 PCB :)

P. 03/04 SB2209 manual: You need to select Vin (24V) for all fans. Be sure to wire Gnd to Gnd and 24V to 24V! Otherwise you will experience magic smoke later.

P. 05 SB2209 manual: Skip

P. 06 SB2209 manual: Be sure to wire Gnd to Gnd, Signal to Signal and 24V to 24V! Otherwise you will experience magic smoke later.

P. 13 SB2209 manual: Skip, unless you use a PT1000 Thermistor

P. 15 SB2209 manual: Skip

P. 18 SB2209 manual: Skip

P. 19 SB2209 manual: Skip, Stealthburner will be assembled later.

P. 24 SB2209 manual: You will need to Strip down the Isolation a bit so you have enough cable length to connect the cable to the PSU and to the Can port. Go back to the Tap Manual page 34 now, flashing the toolhead will be done later.

P. 36 Tap manual: Stealthburner and Tap are now completed and installed. Switch back to p. 148 of the original V2.4 manual.

P. 150-152 v2.4 manual: Skip; Raspberry Pi mounting and 5v PSU mounting is not needed. Instead, mount the CB1 / CM4 on the Manta.

--- to be continued ---

