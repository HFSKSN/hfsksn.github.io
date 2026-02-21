---
title: Module's Selected Major Components
---

## Module's Selected Major Components

The following sections are the selected major components necessary for the Gyroscope module to function. According to the project requirements, this subsystem must have a surface-mounted 3.3 volt switching regulator as well as a sensor which is capable of sending gyroscopic data to the camera arm of the boat and is compatible with either the PIC18 or ESP32.

### Power Management

**Voltage Regulator**

1. LM7805 Regulator

    ![](lm7805.png)

    * 1.43/each
    * [link to product](https://www.digikey.com/en/products/detail/texas-instruments/LM7805MPX-NOPB/6110583)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Meets surface mount constraint of project | Requires external components                                     |
    |                                           | Not standard for PIC or ESP32                                    |

3. LM2575 Regulator

    ![](lm2575.png)

    * $2.16/each
    * [link to product](https://www.digikey.com/en/products/detail/onsemi/LM2575D2T-3-3R4G/1476688)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Provided by course                        | Requires external components                                     |
    | Meets surface mount constraint of project |                                                                  |

4. BU33UV7NUX-E2 Regulator

    ![](BU33UV7NUX-E2.png)

    * $1.13/each
    * [link to product](https://www.digikey.com/en/products/detail/rohm-semiconductor/BU33UV7NUX-E2/8125892)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Meets surface mount constraint of project | Requires external components                                     |
    | Inexpensive                               | 11 solder points                                                 |
   
**Rationale:** The course-provided LM2575 regulator circuit is the best fit for this module because it is the easiest since it is already available for testing and development, provides the correct voltage, and only has five solder points.

### Sensor

**Gyroscope**

1. MPU-6050

    ![](.png)

    * $3.69/each
    * [link to product](https://www.digikey.com/en/products/detail/universal-solder-electronics-ltd/26098/26606388)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Gyroscope and accelerometer               | Not surface mounted                                              |
    | Many resources on how to use with ESP32   |                                                                  |
    | Component already owned by team           |                                                                  |

2. BMI323

    ![](BMI323.png)

    * $3.27/each
    * [link to product](https://www.digikey.com/en/products/detail/bosch-sensortec/BMI323/16719593)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Accelerometer, Gyroscope, Magnetometer    | Requires external components                                     |
    | Surface mounted                           |                                                                  |

4. LSM9DS0TR 

    ![](LSM9DS0TR.png)

    * $13.47/each
    * [link to product](https://octopart.com/part/stmicroelectronics/LSM9DS0TR)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Accelerometer, Gyroscope, Magnetometer, Temperature Sensor | Requires external components                    |
    | Surface mounted                           | Expensive                                                        |
    |                                           | Not available on Digikey                                         |

**Rationale:** The MPU-6050 is the best fit for this project because it is designed to be used with the ESP32 and is already able to be tested by our team. Despite the fact that it uses a daughtboard with through-hole pins, the sensor is still able to be used in this project with approval from the professor. It also can be used to meet our stretch goal of calculating speed using the accelerometer.
