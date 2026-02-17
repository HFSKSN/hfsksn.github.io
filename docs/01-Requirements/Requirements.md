---
title: Module's Requirements
---

## Module Requirements
The following sections document the requirements that the Gyroscope module in the Camera Arm Subgroup needs to fulfill in order to stabilize the camera during data collection. As a stretch goal, the subsystem may also be able to track the speed of the boat and the location of the boat using the speed data with additional sensors.

| **Requirement Description** | **Measure of<br> Threshold** | **Target<br>Measure** |**Stretch<br>Requirement<br>(Y-N)**|
|-----------------------------| ----------------- | ----------------- | :-----: |
| Surface-mounted 3.3V switching power regulator | 3.2 Volts | 3.3 Volts | No |
| Surface-mounted microcontroller | 1 PIC or ESP | ESP32 | No |
| Wireless Communication | Able to send or receive bluetooth data | Send and receive bluetooh data to other modules | Yes |
| Gyroscope Sensor | Able to detect angular movement of boat | Send motion data to stabilize camera instruments | No |
| Accelerometer Sensor | Able to detect speed of boat | Send speed data to user interface | Yes |
| UART Communication | Able to send or receive data | Send and receive data to other modules | No |
| Distance Calculation | Able to record location from accelerometer data | Store sensor data, calculate distance, and send data to user interface | Yes |
