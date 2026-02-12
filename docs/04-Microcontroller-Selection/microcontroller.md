---
title: Module's Selected Microcontroller
---

## Module's Selected Microcontroller

The following section details relevant information on the selected microcontroller for the HMI module, the ESP32. Official datasheets, online resources, load specifications, are listed below in Table 1. Table 2 and Figure 1 display the pins and modules available for the functionality required for the subsystem, which requires UART communication between subsystems, I2C for the OLED screen to function, GPIO inputs for pushbuttons, ADC inputs for potentiometers, LED PWM outputs for LEDs, and a USB programmer for coding. The ESP32 was chosen for this project over the PIC 18 because of the additional UART slots provided (there is a pinout conflict if attempting to use two UART moduless and I2C in the PIC 18 DIP) as well as the fact that there are more resources on programming the OLED screen with the ESP32.


**Table 1:** Microcontroller Info

| ESP Info                                      | Answer                                                                                              |
| --------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| Model                                         | ESP32 S3 WROOM 1 N4                                                                                 | 
| Product Page URL                              | [link](https://www.espressif.com/en/products/modules)                                               |
| ESP32-S3-WROOM-1-N4 Datasheet URL             | [link](https://documentation.espressif.com/esp32-s3-wroom-1_wroom-1u_datasheet_en.pdf)              | 
| ESP32 S3 Datasheet URL                        | [link](https://documentation.espressif.com/esp32-s3_datasheet_en.pdf)                               | 
| ESP32 S3 Technical Reference Manual URL       | [link](https://documentation.espressif.com/esp32-s3_technical_reference_manual_en.pdf)              | 
| Vendor link                                   | [link](https://www.digikey.com/en/products/detail/espressif-systems/ESP32-S3-WROOM-1-N4/16162639)   | 
| Code Examples                                 | [link](https://github.com/embedded-systems-design/code_esp32_oled)                                  | 
| External Resources URL(s)                     | [link](https://embedded-systems-design.github.io/tutorials/esp32/)                                  | 
| Unit cost                                     | $5.06                                                                                               | 
| Supply Voltage Range                          | Min: 3.0V <br> Typ: 3.3V <br> Max: 3.6V <br> Abs Max: 3.6V                                          | 
| Absolute Maximum current <br> (for entire IC) | 355mA                                                                                               | 
| Maximum GPIO current <br> (per pin)           | 40mA                                                                                                | 
| Supports External Interrupts?                 | Yes                                                                                                 | 
| Required Programming Hardware, Cost, URL      | VScode Pymakr <br> $0 <br> [link](https://marketplace.visualstudio.com/items?itemName=pycom.Pymakr) | 


**Table 2:** Pin Allocation

| Module         | # Available | Needed | Associated Pins (or * for any) |
| -------------- | ----------- | ------ | ------------------------------ |
| UART           | 3           | 2      | *GPIO                          |
| External SPI   | 2           | 0      | *GPIO                          |
| I2C            | 2           | 1      | *GPIO                          |
| GPIO           | 36          | 4      | *GPIO                          |
| ADC            | 20          | 2      | IO1-20                         |
| LED PWM        | 36          | 2      | *GPIO                          |
| Motor PWM      | 36          | 0      | *GPIO                          |
| USB Programmer | 1           | 1      | IO19-20                        |


## Microcontroller Diagram

![Pinout Diagram](pinout.png)

**Figure 1:** ESP32-S3-WROOM-1 Pinout Diagram
