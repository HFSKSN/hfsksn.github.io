---
title: Module's Requirements
---

## Module Requirements
The following sections document the requirements that the User Interface module needs to fulfill in order to allow the user to directly interact with the automated telescope, input commands, and view the data collected by the other modules.

| **Requirement Description** | **Measure of<br> Threshold** | **Target<br>Measure** |**Stretch<br>Requirement<br>(Y-N)**|
|-----------------------------| ----------------- | ----------------- | :-----: |
| Surface-mounted 3.3V switching power regulator | 3.2 Volts | 3.3 Volts | No |
| Surface-mounted microcontroller | 1 PIC or ESP | ESP32 | No |
| Wireless Communication | Able to send or receive a Wi-Fi data | Send and receive Wi-Fi Data to MQTT | Yes |
| Surface-mounted Display | Able to display data | Displays data received from sensor modules | No |
| Surface-mounted Controls | Able to process user inputs | Send user inputs to microcontroller and device reacts to commands | No |
| UART Communication | Able to send or receive data | Send and receive data as main hub for modules | No |
| Surface-mounted Storage Device | Able to store data | Stores sensor data and can be ejected from housing | Yes |
