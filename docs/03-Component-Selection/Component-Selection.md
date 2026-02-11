---
title: Module's Selected Major Components
---

## Module's Selected Major Components

The following sections are the selected major components necessary for the Human-Machine Interface module to function. According to the project requirements, this subsystem must have a 3.3 volt switching regulator, a sensor for users to input commands into the interface, and an OLED screen to display data.

### Power Management

**Voltage Regulator**

1. Custom Circuit

    ![](image1.png)

    * $1/each
    * [link to product](http://www.digikey.com/product-detail/en/ECS-40.3-S-5PX-TR/XC1259TR-ND/827366)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Components provided by course             | Cannot change voltage setting after it has been soldered         |
    | Can be deconstructed if needed            | Requires more space on PCB                                       |
    |                                           | Components provided need pliers to meet surface mount constraint |

2. Regulator Circuit

    ![](image1.png)

    * $1/each
    * [link to product](http://www.digikey.com/product-detail/en/ECS-40.3-S-5PX-TR/XC1259TR-ND/827366)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Provided by course                        | Unable to replace parts of circuit if needed                     |
    | Requires few traces in PCB                | Needs pliers to meet surface mount constraint                    |
    | Can change voltage settings after it has been soldered if needed (0V/3.3V/5V) |                              |

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
    |                                           | |

3. Joystick Potentiometer

    ![](image1.png)

    * $5.73/each
    * [link to product](https://www.digikey.com/en/products/detail/favor-electronics/FJ05K-S1B5KB0/16893757?s=N4IgjCBcoExgbFUBjKAzAhgGwM4FMAaEAeygG0QAWABgGYBWAThAF0iAHAFyhAGVOATgEsAdgHMQAX2lA)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    |                         | Expensive |
    | Meets surface mount consraint of project  | Needs several traces and pinouts                                 |
    | Allows for analog input                   |                                                                  |

**Rationale:** A clock oscillator is easier ...

### Actuator

**HMI OLED Screen**

1. XC1259TR-ND surface mount crystal

    ![](image1.png)

    * $1/each
    * [link to product](http://www.digikey.com/product-detail/en/ECS-40.3-S-5PX-TR/XC1259TR-ND/827366)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Provided by course                        | Requires external components and support circuitry for interface |
    | Compatible with PSoC                      | Needs special PCB layout.                                        |
    | Meets surface mount constraint of project |

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

**Rationale:** A clock oscillator is easier ...
