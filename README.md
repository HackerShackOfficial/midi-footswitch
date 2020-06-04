# midi-footswitch
MIDI footswitch for software instruments

This is an extremely simple script that shows how to configure buttons connected to a Teensy controller for a MIDI footswitch. The code has a lot of boilerplate that should be cleaned up with loops, but I kept it as-is for clarity.

## Setup Instructions

1. Download teensyarduino (installer)[https://www.pjrc.com/teensy/td_download.html]
2. Plug in your device
3. When using Arduino, be sure to select Teensy in the `Tools` > `Boards menu (Teensy 4.0)`
4. You must select`MIDI` from the `Tools` > `USB Type` menu
5. Select the correct port (you should see "Teensy" in the port name)
6. Upload the script
