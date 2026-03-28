---
title: Module's API
---

## Overview

In the daisy chain, the Gyroscope module will be sending message 8, Adjust Angle, to the Camera Arm module and message 5, Get Speed, to the Controller Module. All other message types will be passed through the chain, and invalid message types will be discarded.

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

|               | Byte 1    | Byte 2      | Byte 3       | Byte 4  |
|---------------|-----------|-------------|--------------|---------|
| Variable Name | sender_id | receiver_id | message_type | value   |
| Variable Type | char      | char        | uint8_t      | uint8_t |
| Min Value     | H         | A           | 5            | 0       |
| Max Value     | H         | A           | 5            | 30      |
| Example       | H         | A           | 5            | 2       |

Get Distance

|               | Byte 1    | Byte 2      | Byte 3       |
|---------------|-----------|-------------|--------------|
| Variable Name | sender_id | receiver_id | message_type |
| Variable Type | char      | char        | uint8_t      |
| Min Value     | J         | A           | 6            |
| Max Value     | J         | A           | 6            |
| Example       | J         | A           | 6            |

Get Temperature

|               | Byte 1    | Byte 2      | Byte 3       |
|---------------|-----------|-------------|--------------|
| Variable Name | sender_id | receiver_id | message_type |
| Variable Type | char      | char        | uint8_t      |
| Min Value     | I         | A           | 7            |
| Max Value     | I         | A           | 7            |
| Example       | I         | A           | 7            |

Stabilize Arm

|               | Byte 1    | Byte 2      | Byte 3       | Byte 4  | Byte 5  |
|---------------|-----------|-------------|--------------|---------|---------|
| Variable Name | sender_id | receiver_id | message_type | x_value | y_value |
| Variable Type | char      | char        | uint8_t      | uint8_t | uint8_t |
| Min Value     | H         | G           | 8            | -127    | -127    |
| Max Value     | H         | G           | 8            | 127     | 127     |
| Example       | H         | G           | 8            | 120     | -25     |

Roll Call

|               | Byte 1       |
|---------------|--------------|
| Variable Name | message_type |
| Variable Type | uint8_t      |
| Min Value     | 12           |
| Max Value     | 12           | 
| Example       | 12           |
