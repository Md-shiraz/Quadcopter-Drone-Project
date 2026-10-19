# Quadcopter Drone Project

A Pixhawk-based quadcopter build covering airframe assembly, electrical wiring, flight-controller setup, calibration, and flight testing. The project report contains the detailed build procedure, wiring summary, safety guidance, and troubleshooting notes.

## Hardware

- Pixhawk 2.4.8 flight controller with GPS and external compass
- Four A2212/13T 1000 KV brushless motors and four Cyclone 35 A ESCs
- FlySky FS-i6S transmitter and FS-iA10B receiver, connected using PPM
- 10-inch propellers
- Reported battery: 3-cell, 5200 mAh; verify the battery label and configuration before use

The documented flight modes are Stabilize, Loiter, and Return to Launch (RTL). Mission Planner is used for firmware setup, calibration, battery monitoring, and flight-mode configuration.

## Project photo

![Assembled quadcopter showing its frame, motors, Pixhawk flight controller, GPS module, and receiver](WhatsApp%20Image%202026-10-19%20at%2018.17.42.jpeg)

![Quadcopter in flight during an outdoor test](quadcopter-flight-test.png)

## Repository contents

- `src/Main.java` — IntelliJ IDEA Java starter/demo program. It is not flight-control firmware.
- [`Drone_Project_Report_Improved (1).docx`](./Drone_Project_Report_Improved%20%281%29.docx) — detailed project report.

The Pixhawk firmware and aircraft configuration are handled through Mission Planner; this repository does not contain custom drone-control software.

## Running the Java demo

Open the project in IntelliJ IDEA, configure a JDK that supports the compact source-file syntax used in `src/Main.java`, and run `Main.java`. The demo prints a greeting and the numbers 1 through 5; running it does not control the quadcopter.

## Safety

Remove all propellers before ESC calibration and motor testing. Before flight, verify motor order and rotation, radio and battery failsafes, sensor health, GPS/compass operation, and RTL settings. Perform initial flight tests in a clear, suitable outdoor area, keep people away, and follow applicable drone operating requirements. Always verify settings against the installed hardware and firmware.
