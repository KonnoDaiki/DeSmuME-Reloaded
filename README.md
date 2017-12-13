# DeSmuME-Reloaded

DS emulator with WiFi support

# SETUP

- cd desmume/src/frontend/posix
- ./autogen.sh
- ./configure --enable-glx --enable-openal --enable-glade --enable-wifi
- make
- cd gtk

After compilation of the project, run the following command to use the libpcap functions in standard user mode :
- sudo setcap cap_net_raw,cap_net_admin=eip ./desmume

Example for using DeSmuME after all these steps :
- desmume --bios-arm9 "/home/test/Documents/MyBios/biosnds9.bin" --bios-arm7 "/home/test/Documents/MyBios/biosnds7.bin" --firmware-path "/home/test/Documents/MyBios/firmware.bin" --firmware-boot 1

# TODO

- See for useful ameliorations to add on my DeSmuME version ( bug fixes and suggestions are welcome)
- Collaboration with StapleButter (MelonDS developper) and other people to add WiFi local support

# History

13-Dec-2017 : Third version with WiFi support working with DWC project
- Desmume version 0.9.12 svn
- Firmware can be set via command-line

13-Dec-2017 : Second version with WiFi support working with DWC project
- Desmume version 0.9.11 svn
- Firmware can be set via command-line and GTK mode

12-Dec-2017 : First version with WiFi support working with DWC project
- Desmume version 0.9.7 svn r3947
- Firmware can be set via command-line and GTK mode
- Bug fixes on loading and saving .dfc files
