# TapIn

A classroom attendance dashboard. A teacher starts a session, students tap an RFID card or scan a QR code, and TapIn marks each student present, late or absent automatically.

## Features
- Late rule based on class start time and a grace period, editable at any time
- Reader-friendly input: RFID and QR readers type the number and press Enter, so the same box works with real hardware (Raspberry Pi, ESP32 or a USB reader)
- Live roster, tap log, today's counts and an attendance-rate chart across sessions
- CSV export and one-click delete of all data
- Privacy by design: only student number, name and time are stored; no photos or biometrics; data stays in the browser

## Run
Open `index.html`. Click a student card or type a number such as `2023-0101` to simulate a tap. The roster and history are fictional sample data.

## Thesis angles
- Compare reader methods (RFID, QR, face recognition) on speed, error rate and cost
- Measure time saved per class versus paper attendance
- Add a back end so tap events from an ESP32 reach the dashboard over Wi-Fi
