# Firmware Flashing

First of all, be sure that your wiring is **100% correct** before you first power on your Printer. You should **disconnect* the bed heater and the SB2209 RP2040 completely, otherwise they may heat which could destroy your printed parts, hotend, bed heater, magnet sheet or thermal fuse.

## CB1/CB2 Setup
*this guide translates 1:1 to BTT Pi v1.1 / v2*
1. Get the [latest release of the cb1 firmware](https://github.com/bigtreetech/CB1/releases) (for cb2 get the [latest cb2 firmware release](https://github.com/bigtreetech/CB2/releases)). You want to download the XXX...XXX.img.xy file. This may take some time.
2. While you are waiting for the file to download, install the [Raspberry Pi Imager](https://www.raspberrypi.com/software/).
3. Unpack the firmware so you have a .img file.
4. Open the Raspberry Pi Imager, click on Choose OS, scroll down to the very end, klick on "Use Custom" and select the .img file you just unpacked.
5. Select the MicroSD card with the "Choose Storage" function.
6. Click on "WRITE" and accept that all previous data on the SD card will be deleted.
7. If the imager didn't already eject the SD-Card, eject it, pull it out from your Computer and plug it back in.
8. The Card will now show up as "BOOT".
9. Open the system.cfg file.
10. Remove the `#` in front of hostname and change it to whatever name you want your printer to show up in your network. E.g. `hostname="Voron"`
11. Remove the `#` in front of TimeZone and change it to your local time zone, E.g. `Europe/Munich`, `America/New_York` or `Asia/Shenzen`.
12. Go to WIFI_SSID and change it to your Wifi Name (`WIFI_SSID="YOURWIFINAME"`).
13. Go to WIFI_PASSWD and change it to your Wifi Password (`WIFI_PASSWD="YOURWIFIPASSWORD"`).
14. **DONT EDIT ANYTHING ELSE UNLESS YOU KNOW EXACTLY WHAT YOU ARE DOING!**

## CM4/5 Setup
*this guide translates 1:1 to Raspberry Pi 4 / 5*
1. Download and install [Raspberry Pi Imager](https://www.raspberrypi.com/software/).
2. Click “Choose OS” and scroll down to “Other specific-purpose OS”.
3. Select “3D Printing” and choose “Mainsail OS”.
4. Choose your SD Card.
5. If you will be using Wi-Fi, click on the GEAR icon in the bottom right corner and enter your Wi-Fi information.
6. Click on “SAVE” and on “WRITE”. and accept that all previous data on the SD card will be deleted.
7. Make sure that your MCU(s) is connected to your pi. If you will be using wired networking, also make sure your ethernet cable is connected.
8. Insert the microSD card into your Pi, and power on the Pi.
9. Find your Pi on the network, and ssh into it (using PuTTY on Windows or the terminal on MacOS). The default username is pi and the password is raspberry.
	* If your network supports bonjour, the pi should show up as mainsailos.local
	* If your network automatically assigns DNS hostnames, it may simply show up as mainsailos
	* Failing these two options, you may need to check your router’s DHCP server, and find out what IP address as been assigned to the device.

## CANBUS Setup
1. First of all, take a look at the [CANbus basics](https://canbus.esoterical.online).
2. Now [set up the CANbus Network](https://canbus.esoterical.online/Getting_Started.html).
3. [Flash your Mainboard](https://canbus.esoterical.online/mainboard_flashing.html). You need to flash it in USB-CAN-Bridge. You can find the needed Mainboard settings / hardware [here](https://canbus.esoterical.online/mainboard_flashing/common_hardware/BigTreeTech%20Manta%20M8P%20v2.0/README.html).
4.Now [flash your SB2209 RP2040](https://canbus.esoterical.online/toolhead_flashing.html). You can find the needed settings / hardware [here](https://canbus.esoterical.online/toolhead_flashing/common_hardware/BigTreeTech%20SB2209%20(RP2040)/README.html).
4. Note your UUIDs and note which one is the one of the Mainboard and which belongs to the toolhead.