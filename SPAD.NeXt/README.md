
Special thanks to @1L2P (Discord ID: 1L2P#5598) for his excellent work!

Firmware tested with SPAD_v0.9.12.92 Full Release

MCP communicates with SPAD.neXt via SerialV2.
Baud Rate is 115200


Pre-config is available as Snippet #6477 or "Flight Core Technologies PMDG 737 MCP"

Internal device features:
- Turn on/off backlight by pressing C/O + CMDA and C/O + CWSA (MCP needs to be externaly powered)
- Set Backlight brightness level by pressing C/O and turning V/S encoder
- Turn on/off all display digits by pressing C/O + CMDB and C/O + CWSB
- Set Display brightness level by pressing C/O and turning RIGHT COURSE encoder
- The version is displayed on the led segments digits


![Screenshot](https://user-images.githubusercontent.com/53659578/193845938-f0ef2aed-1326-4257-a87d-9a4b7bee52e3.png)

R4:
Official VIP PID registration, State scan feature is now enabled, new VIRTUAL_POWER variable is available

R03d:
- clean some potential display overflow
- add negative values for displays if you need them in other aircraft
- fix decimal point missing in IAS/MACH display (just need to send a 0.00 format value)

R02:
- Fix for an overflow issue with the altitude display over 32768 feet
