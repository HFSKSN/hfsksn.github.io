---
title: Module's Block Diagram
tags:
- tag1
- tag2
---

## Overview
The purpose of this block diagram is to display what is necessary for the subsystem to function and to properly allocate resources such as pins and power according to the previously stated requirements and concept. In order to power the subsystem, a power source over 7V, such as 9V 2A wall supply, is needed to pass through a 3.3V 1.5A regulator which powers the module's major components. The primary sensor is the Gyroscope and Accelerometer Sensor, which will detect both the angular movement and speed of the boat. A simple digital switch and LED is also included for testing and debugging. Communication between modules will be facilitated through headers connecting UART pins. Bluetooth in the ESP32 may be used to provide additional functionality if needed.

## Block Diagram 
![Individual Block diagram](EGR314_BlockDiagram.drawio.png)

**Figure 1:** Individual Block Diagram for Gyroscope module with sensor, pinouts, debugging elements, and UART connectors. PDF version [*here*](EGR314_BlockDiagram.drawio.pdf)
