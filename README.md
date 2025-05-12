# Borewell Management System 

It's an **IoT-based motor management borewell system** via ESP8266 and Blynk. One can toggle **Manual** or **Automatic** mode with controlling the motor upon **ultrasonic water sensing**.

Features:
- Automatic/Manual relay switch
- Water sensing through ultrasonic sensor
- Realtime monitoring and control using Blynk
- Physical debounced button for manual and mode selection
- Augmented gauge logic to track the levels better

Hardware Used:
- ESP8266 (NodeMCU)
- Ultrasonic sensor (HC-SR04)
- Relay Module (6HP)
- Push buttons × 2
- 10kΩ resistors (if not using INPUT_PULLUP)
- Wires and breadboard

Blynk Setup:
- Virtual Pin `V1` – Relay Control
- Virtual Pin `V2` – Mode Control (Auto/Manual)
- Virtual Pin `V3` – Relay Status (Display)
- Virtual Pin `V4` – Mode Status (Display)
- Virtual Pin `V5` – Water Level Gauge

Logic:
- **Manual Mode**: Button or Blynk toggles relay
- **Auto Mode**: Relay turns ON below 30%, OFF above 85%
- **Relay Logic**: `HIGH` = ON, `LOW` = OFF (inverted)

Getting Started
1. Flash `code/borewell_management.ino` to ESP8266.
2. Replace your `WiFi` and `Blynk` credentials.
3. Connect components as per circuit.
4. Use Blynk app for control & monitoring.

License:
MIT License © CH SATHVIK KUMAR
