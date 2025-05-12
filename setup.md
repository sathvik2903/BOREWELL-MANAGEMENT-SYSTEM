Setup Instructions

Wiring :

| Component        | ESP8266 Pin |
|------------------|-------------|
| Ultrasonic TRIG  | D1          |
| Ultrasonic ECHO  | D2          |
| Relay IN         | D5          |
| Manual Button    | D6          |
| Mode Button      | D0          |

- Both buttons use `INPUT_PULLUP`
- Relay is active HIGH

Ultrasonic Notes :
- Ensure max distance set to 200cm in code
- Position sensor above tank opening

Blynk App :
- Add one Button widget (V1) – Relay
- Add another Button (V2) – Mode toggle
- Add two Labels (V3, V4) – Status display
- Add a Gauge widget (V5) – Water level display

Upload : 
1. Connect ESP to USB
2. Use Arduino IDE or PlatformIO
3. Install required libraries:
   - ESP8266WiFi
   - Blynk
   - NewPing
