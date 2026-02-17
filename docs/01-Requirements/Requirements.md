---
title: Module's Requirements
---

## Module Requirements
The following sections document the requirements that the D3 Sensor module needs to fulfill in order to allow the user to recieve data on the boat's speed. As stretch goals, the subsystem may also be able to track the location of the boat using the speed data or help stabilize the on-board instruments with additional sensors.

| **Requirement Description** | **Measure of<br> Threshold** | **Target<br>Measure** |**Stretch<br>Requirement<br>(Y-N)**|
|-----------------------------| ----------------- | ----------------- | :-----: |
| Surface-mounted 3.3V switching power regulator | 3.2 Volts | 3.3 Volts | No |
| Surface-mounted microcontroller | 1 PIC or ESP | ESP32 | No |
| Wireless Communication | Able to send or receive bluetooth data | Send and receive bluetooh data to other modules | Yes |
| Accelerometer Sensor | Able to detect speed of boat | Send speed data to user interface | No |
| Gyroscope Sensor | Able to detect angular movement of boat | Send motion data to stabilize camera instruments | Yes |
| UART Communication | Able to send or receive data | Send and receive data to other modules | No |
| Distance Calculation | Able to record location from accelerometer data | Store sensor data, calculate distance, and send data to user interface | Yes |
