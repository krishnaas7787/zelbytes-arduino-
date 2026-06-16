# Task 8 - IoT Lab Telemetry Integration

## Overview
This task implements posting of bench sensor telemetry data
(temperature, humidity, soil moisture, CO2) from an Arduino Uno
to the Zelbytes IoT Learning Lab cloud dashboard, using a Python
script running on the host machine to bridge Serial CSV data to
the cloud API.

## Files
- `telemetry.py` — Python script reading Serial CSV from Arduino and posting to IoT Lab
- `secrets.h.example` — Template for required API key and device ID (real values excluded from repo)
- `docs/IOT_LAB.md` — Full documentation of API integration and field mapping
- `images/` — Proof of successful data transmission and dashboard visibility

## How to Run
1. Copy `secrets.h.example` to `secrets.h` and fill in your real API key and device ID
2. Connect Arduino Uno via USB and confirm the correct COM port in `telemetry.py`
3. Run the script:4. Verify successful POST responses (status 202) in the terminal
5. Check **IoT Lab → API Explorer** to confirm new data points

## Result
- 10 telemetry samples were successfully posted under device_id `krishnaas_bench01`
- Each request returned HTTP status **202**
- Data was confirmed visible in the IoT Lab API Explorer, with the temperature_c series showing 36 total recorded data points

## Security Note
Never commit `secret.h` (or `secrets.h`) or any file containing real API keys.
This is enforced via `.gitignore`.

## Verification
- 10 sample readings were successfully posted under device_id `krishnaas_bench01`, each returning HTTP status **202**.
- Data was confirmed visible via **IoT Lab → API Explorer**, with the `temperature_c` series showing multiple recorded data points across all samples sent.

## Notes
- ESP8266 WiFi bridge integration is planned for Day 17, removing the need for a host Python relay script.
