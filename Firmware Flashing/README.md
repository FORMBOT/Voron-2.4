# Firmware Flashing

First of all, be sure that your wiring is **100% correct** before you first power on your Printer. You should **disconnect* the bed heater and the SB2209 RP2040 completely, otherwise they may heat which could destroy your printed parts, hotend, bed heater, magnet sheet or thermal fuse.

## CB1/CB2 Setup
1. Get the [latest release of the cb1 firmware](https://github.com/bigtreetech/CB1/releases) (for cb2 get the [latest cb2 firmware release](https://github.com/bigtreetech/CB2/releases)). You want to download the XXX...XXX.img.xy file. This may take some time.
2. While you are waiting for the file to download, install the [Raspberry Pi Imager](https://www.raspberrypi.com/software/).
3. Unpack the firmware so you have a .img file.
4. Open the Raspberry Pi Imager, click on Choose OS, scroll down to the very end, klick on "Use Custom" and select the .img file you just unpacked.
5. Select the MicroSD card with the "Choose Storage" function.
6. Click on "write" and accept that all previous data on the SD card will be deleted.
7. If the imager didn't already eject the SD-Card, eject it, pull it out from your Computer and plug it back in.
8. The Card will now show up as "BOOT".
9. Open the system.cfg file.
10. Remove the `#` in front of hostname and change it to whatever name you want your printer to show up in your network. E.g. `hostname="Voron"`
11. Remove the `#` in front of TimeZone and change it to your local time zone, E.g. `Europe/Munich`, `America/New_York` or `Asia/Shenzen`.
12. Go to WIFI_SSID and change it to your Wifi Name (`WIFI_SSID="YOURWIFINAME"`).
13. Go to WIFI_PASSWD and change it to your Wifi Password (`WIFI_PASSWD="YOURWIFIPASSWORD"`).
14. **DONT EDIT ANYTHING ELSE UNLESS YOU KNOW EXACTLY WHAT YOU ARE DOING!**