
# Functional parts build notes (to get the Printer up and running)
Start with the [Stock Voron 2.4 Manual](https://github.com/VoronDesign/Voron-2/tree/Voron2.4/Manual).
Be aware that the v2.4 Manual uses a 250mm Version of the v2, so some dimensions may seem wrong if you build a 300mm/350mm Version.

## P. 25 v2.4 manual: 
If you build a bigger Version than a 250mm, you need more screws / m3-T-Nuts. Start from the outer holes in the rail and work your way towards the middle screwing the rail down every second hole.
The carriages are designed to slide along the rail easily. This unfortunately also includes sliding off the rails. Dropping the carriage likely irreparably damages it. ALWAYS put the little black rubber Carriage stoppers back on the rail (into the holes without screws) until your printer ist up and runnning!

## P. 29 v2.4 manual:
The DIN-Rails need to be rotated 90 Degrees so the cables are long enough later. They should run parallel to the bed extrusions (from front to back).

## P. 84 v2.4 manual: 
Skip this step, this part is not used and therefore probably not included in your printed parts.

## P. 88 v2.4 manual: 
If you are building a 300mm machine you will need to start you screws from the second screw hole in the rails leaving the end holes open to allow space for T-nuts at later steps.
Small reminder: The carriages are designed to slide along the rail easily. This unfortunately also includes sliding off the rails. Dropping the carriage likely irreparably damages it. ALWAYS put the little black rubber Carriage stoppers back on the rail (into the holes without screws) until your printer ist up and runnning!

## P. 101 v2.4 manual: 
Again, if you are building a bigger printer than the 250mm version, start at the outer holes and screw the rail down every second hole.
Small reminder (again): The carriages are designed to slide along the rail easily. This unfortunately also includes sliding off the rails. Dropping the carriage likely irreparably damages it. ALWAYS put the little black rubber Carriage stoppers back on the rail (into the holes without screws) until your printer ist up and runnning!

## P. 104 v2.4 manual: 
As said before, the part on top of the right XY-Joint is not used with this kit. Use m5x10 BHCS like on the left XY-Joint to secure the X Axis to the XY-Joints.

## P. 122 v2.4 manual: 
After you installed the Z-belts and squared the Gantry, make sure your AB belts are exactly the same length and have the exact same amount of teeth! Proceed with routing the AB-Belts, but be Aware that you will use a different X carriage as in the Voron 2.4 Manual.

## P. 129-131 v2.4 manual: 
Skip these pages. Put the AB belts to the MGN12 Carriage with some tape, they dont have to be tight.

## P. 143 v2.4 manual: 
X Carriage: After finishing the AB-Belts Routing, switch to the [TAP Manual](https://github.com/VoronDesign/Voron-Tap/tree/main/Manual). Optotap is used as the sensor.
Be sure to take a look into the R8_errata.md document, it Highlights some important changes from the Manual and install the X Endstop switch.

## P. 33 Tap Manual: 
After you have installed Tap successfully and have the AB belts fixed in the tap carriage, switch to page 146 of the Voron 2.4 manual or to the [Stealthburner manual](https://github.com/VoronDesign/Voron-Stealthburner/tree/main/Manual).
We will come back to install the Toolhead later.

## P. 13 Stealthburner manual: 
You use a Toolhead PCB, so install these two heat inserts.

## P. 14 Stealthburner manual: 
Skip

## P. 30 Stealthburner manual: 
Follow [this Video Guide](https://github.com/VoronDesign/Voron-Stealthburner/tree/main/Manual) on how to set the gear mesh on your CW2.
Follow [this video Guide](https://www.youtube.com/watch?v=L1gxBCiE0pk) on how to set the Anti-Squish as well.

## P. 31 Stealthburner manual: 
Skip for now, we will install our Version of the Anchor later.

## P. 34 Stealthburner manual: 
You dont need to fix the Cable Cover down with the m3x6 BHCS now, you will need to access this later.

## P. 36-43 Stealthburner manual: 
All Hotends are mounted in a similar pattern and pretty self-explaining, your hotend mount and hotend will look different.

## P. 46-51 Stealthburner manual: 
Be very careful with the cables, you can easily rip them off the LED PCB which leads to this LED and the following ones not working.

## P. 53 Stealthburner manual: 
Be sure that your fan blows in the right Direction. Look at the arrows on the fan. Additionally, the Sticker on the fan is on the back pointing towards the Hotend. You want the fan to blow air into the hotend, not trying to pull the air out. This destroys your fan and your whole hotend mount because of heatcreep.

## P. 56 Stealthburner manual: 
You dont need to screw the 5015 fan into the SB Face, you will install the SB0000 Fan PCB there later.

## P. 58 Stealthburner manual: 
All parts of the Stealthburner are now pretty much finished. Now you will need to install the Can-Board on there and do some basic wiring. Switch to the [SB2209 RP2040 Manual](https://github.com/bigtreetech/EBB/tree/master/EBB%20SB2209%20CAN%20(RP2040)/Build%20Guide).

## P. 02 SB2209 manual: 
Now you need to screw down the 5015 fan with the SB0000 PCB :)

## P. 03/04 SB2209 manual: 
You need to select Vin (24V) for all fans. Be sure to wire Gnd to Gnd and 24V to 24V! Otherwise you will experience magic smoke later.

## P. 05 SB2209 manual: 
Skip

## P. 06 SB2209 manual: 
Be sure to wire Gnd to Gnd, Signal to Signal and 24V to 24V! Otherwise you will experience magic smoke later.

## P. 13 SB2209 manual: 
You Need to set the switch to 1: on; 2: on; 3: off; 4: on

## P. 15 SB2209 manual: 
Skip

## P. 16 SB2209 manual:
Be sure to use the endstop labeled "To CAN_Endstop" which is the one with the short wires.

## P. 18 SB2209 manual: 
Skip

## P. 19 SB2209 manual: 
Skip, Stealthburner will be assembled later.

## P. 24 SB2209 manual: 
You will need to Strip down the Isolation a bit so you have enough cable length to connect the cable to the PSU and to the Can port. Go back to the Tap Manual page 34 now, flashing the toolhead will be done later.
Use the tight cable sleeve around the cable.

## P. 36 Tap manual: 
Stealthburner and Tap are now completed and installed. Switch back to p. 148 of the original V2.4 manual.

## P. 149 v2.4 manual:
Rotate the din rails 90° compared to the original layout.

## P. 150-152 v2.4 manual: 
Skip; Raspberry Pi mounting and 5v PSU mounting is not needed. Instead, mount the CB1 / CM4 on the Manta.

## P.158-164 v2.4 manual:
Skip; TAP is your Z-Endstop, your X Endstop sits on Tap and your Y endstop will be mounted on the A Motor mount later.

## P. 165 v2.4 manual: 
You use the 3in6 Power Distributor instead.

## P. 170 v2.4 manual:
small reminder, you dont use a Raspberry Pi.

## P. 172 v2.4 manual:
another small reminder, you don't use a 5v PSU.

## P. 175-178 v2.4 manual:
Skip these steps, instead configure your Manta like this:
![M8P_v2 Jumper / Driver marking](https://github.com/FORMBOT/Voron-2.4/blob/main/Diagrams/M8P_config.pdf)
Place a Jumper on all yellow marked pins and place the TMC2209s with attached heatsink on all driver ports with a blue circle after installing the jumpers.

## P. 183 v2.4 manual: 
Leave the cables to the 5v PSU out.

## P. 184 v2.4 manual:
The Z-Endstop cables are not needed.

## P. 185 v2.4 manual: 
Be **100%** sure that the SSR cables are connected correctly, **otherwise your printer is _not_ safe to be powered on**.

## P. 186-189 v2.4 manual:
This kit doesn't use Wagos to distribute the High Voltage cables.

## P. 190-193 v2.4 manual: 
These steps are for an octopus Mainboard. Use this wiring diagram instead: ![v2.4 M8P wiring diagram](https://github.com/FORMBOT/Voron-2.4/blob/main/Diagrams/Wiring%20Diagram%20of%20V2.4%20R2%20Pro%2B.pdf)
For now, only connect z0-z3, the bed heater, 24V from the 24V PSU and the bed thermistor.

## P. 194-199 v2.4 manual:
Skip these steps, you use Umbilical on X and Y.

## P. 204 v2.4 manual:
You use a bit different Wire guide where you have to screw in a pg7 cable gland. From here you route the Can cable down through the z chain, together with the A and B Motor cables. 
![v2.4 M8P wiring diagram](https://github.com/FORMBOT/Voron-2.4/blob/main/Diagrams/Wiring%20Diagram%20of%20V2.4%20R2%20Pro%2B.pdf) 
Connect the B motor (left motor) to X Motor, connect the A motor (right motor) to Y Motor.
Connect the CAN-Cable to the right CAN-Port on the M8P and 24V / GND to the 24V PSU. If you think the cables are not Long enough, you haven't done [this step](https://github.com/FORMBOT/Voron-2.4/tree/main/Build%20Notes#p-24-sb2209-manual).

# Cosmetic parts build notes (not needed to get the pinter running)

## P. 206-209 v2.4 manual:
You can skip these steps.

## P. 211 & 214-216 & 220-221 v2.4 manual:
Skip; you don't need these parts because you use the touchscreen.

## P. 231 v2.4 manual:
Use the ![v2.4 M8P wiring diagram](https://github.com/FORMBOT/Voron-2.4/blob/main/Diagrams/Wiring%20Diagram%20of%20V2.4%20R2%20Pro%2B.pdf) to wire the electronics fans.

## P. 233 v2.4 manual: 
Don't close the electronics compartment yet, you will need to acces this while flashing the boards.

## P. 256 v2.4 manual:
Use the big cable sleeve around the exhaust fan cable (if you use the stock exhaust).