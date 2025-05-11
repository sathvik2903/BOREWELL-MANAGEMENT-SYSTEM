# Borewell Management System

A simple,effective RF-based communication system using the RCSwitch library to wirelessly monitor borewell activity or water usage between a **transmitter** and a **receiver** ESP8266 module.

---
 Hardware Used
- 2 × ESP8266 (NodeMCU boards)
- RF Transmitter (433 MHz)
- RF Receiver (433 MHz)
- Breadboard, jumper wires
- LED for status indication

---
Transmitter:
- Sends a number (0–100) every second via RF.
- The number simulates sensor data or levels.
- LED blinks each time data is sent.

Receiver:
- Listens for RF signals.
- Displays the received number in the serial monitor.
- If no message is received in 2 seconds, a “Message NOT received!” warning is printed.
- LED toggles on successful reception.
