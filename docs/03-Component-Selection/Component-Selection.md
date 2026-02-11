---
title: Module's Selected Major Components
---

## Module's Selected Major Components

The following sections are the selected major components necessary for the Human-Machine Interface module to function. According to the project requirements, this subsystem must have a 3.3 volt switching regulator, a sensor for users to input commands into the interface, and an OLED screen to display data.

### Power Management

**Voltage Regulator**

1. Custom Circuit

    ![](image1.png)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Components provided by course             | Cannot change voltage setting after it has been soldered         |
    | Can be deconstructed if needed            | Requires more traces on PCB                                      |
    |                                           | Components provided need pliers to meet surface mount constraint |

2. LM2575 Regulator Circuit

    ![](image1.png)

    * $2.16/each
    * [link to product](https://www.digikey.com/en/products/detail/onsemi/LM2575D2T-3-3R4G/1476688)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Provided by course                        | Unable to replace parts of circuit if needed                     |         | Meets surface mount constraint of project | Takes up space on PCB                                            |
    | Can change voltage settings after it has been soldered if needed (0V/3.3V/5V) |                              |

3. LM2575 Regulator Circuit

    ![](image1.png)

    * $2.16/each
    * [link to product](https://www.digikey.com/en/products/detail/onsemi/LM2575D2T-3-3R4G/1476688)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Provided by course                        | Unable to replace parts of circuit if needed                     |         | Meets surface mount constraint of project | Takes up space on PCB                                            |
    | Can change voltage settings after it has been soldered if needed (0V/3.3V/5V) |                              |
   
**Rationale:** The course-provided LM2575 regulator circuit is the best fit for this module because it is the easiest to use for debugging and testing due to it being already prepared for use, it has multiple rails and power settings, and it has a switch to turn power on and off.

### Sensor

**Interface Inputs**

1. Pushbutton Switches

    ![](image1.png)

    * $1/each
    * [link to product](http://www.digikey.com/product-detail/en/ECS-40.3-S-5PX-TR/XC1259TR-ND/827366)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Provided by course                        | Might require de-bounce circuit                                  |
    | Requires few traces in PCB                | Needs pliers to meet surface mount constraint                    |
    |                                           | May wear down easily                                             |

2. Potentiometers

    ![](image1.png)

    * $1/each
    * [link to product](http://www.digikey.com/product-detail/en/ECS-40.3-S-5PX-TR/XC1259TR-ND/827366)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Provided by course                        | Requires external components and support circuitry for interface |
    | Allows for analog input                   | Needs pliers to meet surface mount constraint                    |

3. Joystick Potentiometer

    ![](MFG_FJ05K-S1B5KB0.jpg)

    * $5.73/each
    * [link to product](https://www.digikey.com/en/products/detail/favor-electronics/FJ05K-S1B5KB0/16893757?s=N4IgjCBcoExgbFUBjKAzAhgGwM4FMAaEAeygG0QAWABgGYBWAThAF0iAHAFyhAGVOATgEsAdgHMQAX2lA)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Meets surface mount consraint of project  | Needs several traces and pins                                    |
    | Allows for multiple analog inputs         | Expensive                                                        |

**Rationale:** Potentiometers seem to be the best fit for operating the HMI. Using two or more potentiometers will require a few more traces than a pushbutton would but would avoid issues such as debouncing. If needed, however, we can add pushbuttons to the module for minor functions.

### Actuator

**HMI OLED Screen**

1. SSD1306 0.96"

    ![](image1.png)

    * $1/each
    * [link to product](https://www.amazon.com/Songhe-0-96-inch-I2C-Raspberry/dp/B085WCRS7C/)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Provided by course                        | Requires external components and support circuitry for interface |
    | Compatible with ESP32                     | Small Screen                                                     |
    | Meets surface mount constraint of project |                                                                  |

2. XC1259TR-ND surface mount crystal

    ![](image1.png)

    * $1/each
    * [link to product](http://www.digikey.com/product-detail/en/ECS-40.3-S-5PX-TR/XC1259TR-ND/827366)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Inexpensive                               | Requires external components and support circuitry for interface |
    | Compatible with PSoC                      | Needs special PCB layout.                                        |
    | Meets surface mount constraint of project |

3. XC1259TR-ND surface mount crystal

    ![](image1.png)

    * $1/each
    * [link to product](http://www.digikey.com/product-detail/en/ECS-40.3-S-5PX-TR/XC1259TR-ND/827366)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Inexpensive                               | Requires external components and support circuitry for interface |
    | Compatible with PSoC                      | Needs special PCB layout.                                        |
    | Meets surface mount constraint of project |

**Rationale:** The OLED screen . If needed, multiple OLED screens can be used with each displaying different data for the user.
