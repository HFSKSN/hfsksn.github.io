---
title: Module's API
---

## Overview

In the daisy chain, the Gyroscope module will be receiving, acting upon, and discarding message 5, Get Speed, from the Controller module. It will also be sending message 8, Adjust Angle, to the Camera Arm module and message 11, Display Speed, to the Controller Module. All other message types will be passed through the chain, and invalid message types will be discarded.

## Messages

Set Camera Angle

|               | Byte 1    | Byte 2      | Byte 3       |
|---------------|-----------|-------------|--------------|
| Variable Name | sender_id | receiver_id | message_type |
| Variable Type | char      | char        | uint8_t      |
| Min Value     | A         | G           | 3            |
| Max Value     | A         | G           | 3            |
| Example       | A         | G           | 3            |

Take Photo

|               | Byte 1    | Byte 2      | Byte 3       |
|---------------|-----------|-------------|--------------|
| Variable Name | sender_id | receiver_id | message_type |
| Variable Type | char      | char        | uint8_t      |
| Min Value     | A         | F           | 4            |
| Max Value     | A         | F           | 4            |
| Example       | A         | F           | 4            |

Get Speed

|               | Byte 1    | Byte 2      | Byte 3       |
|---------------|-----------|-------------|--------------|
| Variable Name | sender_id | receiver_id | message_type |
| Variable Type | char      | char        | uint8_t      |
| Min Value     | A         | H           | 5            |
| Max Value     | A         | H           | 5            |
| Example       | A         | H           | 5            |

Get Temperature

|               | Byte 1-2     |
|---------------|--------------|
| Variable Name | message_type |
| Variable Type | uint8_t      |
| Min Value     | 6            |
| Max Value     | 6            |
| Example       | 6            |

Get Distance

|               | Byte 1-2     |
|---------------|--------------|
| Variable Name | message_type |
| Variable Type | uint8_t      |
| Min Value     | 7            |
| Max Value     | 7            |
| Example       | 7            |

Adjust Angle

|               | Byte 1-2     | Byte 3   | Byte 4   |
|---------------|--------------|----------|----------|
| Variable Name | message_type | x_value  | y-value  |
| Variable Type | uint8_t      | int8_t   | int8_t   |
| Min Value     | 8            | -127     | -127     |
| Max Value     | 8            | 127      | 127      |
| Example       | 8            | 120      | -25      |
