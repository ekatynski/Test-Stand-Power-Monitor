View this project on [CADLAB.io](https://cadlab.io/project/27045). 

# Test-Stand-Power-Monitor
A small board for cheaply and easily monitoring a motor test stand for a host of data types.

## Function
This board is capable of monitoring the following:
- 1x Voltage input
- 1x Hall Effect Sensor output (current measuring)
- 1x Displacement Sensor interface
- 1x UART (ESCs have UART telemetry output)
- 1x 1K RTD for temperature monitoring

In addition, this board is capable of operating a relay to control a contactor protecting the test stand power supply, as well as a CAN bus to interface with other sensory hardware in development utilizing CAN. In doing so, this board could monitor ESC power consumption, ESC temperature, ESC telemetry output, motor displacement, and eventually eRPM pending future hardware development. Prior test stand setups had used a Teensy 4.1 to monitor telemetry and perform no other function, so this board's development was to expand the amount of test stand monitoring that could be done cheaply while using a less costly and more available microcontroller in the event that it were damaged and required replacement.

## To-Do
Firmware to perform said monitoring has not yet been developed. This board utilizes an ESP32 microcontroller, chosen because it can be configured to communicate over WiFi out of the box, but I have not taken the time to write the C++ needed to make this board useful yet.
