# SafeRing

A women's safety system: a BLE smart ring plus a Flutter companion app that sends an SOS with live location in one tap.

> Source code is private. This repository is a showcase of the project.

## What it does

When the user presses SOS (on the app, or via the ring), SafeRing:

1. Fetches the current GPS location
2. Sends an SMS with a Google Maps live-location link to emergency contacts
3. Places an automatic call to a trusted contact
4. Shows an honest result screen, so a failed SMS or call is shown as failed

## Features

| Area | Features |
|------|----------|
| Emergency | One-tap SOS, Voice SOS, Shake SOS, Flash SOS, Fake Call |
| Location | Live Location sharing (SMS, Google Maps, copy link), Safe Walk, Walk History, Safe Zone, Night Alert |
| Hardware | BLE Ring Connect with battery status (ESP32-C3 based ring) |
| Evidence | Photo and video Evidence Capture |
| Help | Safety Tips, Helplines, nearby police stations on Maps |
| General | Multilingual UI, onboarding with emergency contacts |

## Tech stack

- **App:** Flutter (Dart)
- **Android native:** Kotlin (SMS sending through a platform channel)
- **Location:** Geolocator
- **Hardware:** ESP32-C3 Super Mini, LiPo battery, BLE
- **Release:** signed Android APK (v1.0.0)

## Known limitations

- SMS to the national emergency number 112 is not reliably received, so police alerts need a verified SMS-capable number (planned feature)
- Emergency contacts are currently set during onboarding; an in-app contacts editor is in progress

## Roadmap

- In-app contacts editor
- Nearest police station lookup
- Backend alert service

## Author

Toushif Ansari
Diploma in Computer Engineering, University Polytechnic, BIT Mesra
GitHub: [toushif-ansari22](https://github.com/toushif-ansari22)

Copyright (c) 2026 Toushif Ansari. All rights reserved.
