---
title: Module's API
---

# Overview



## Messages

Set Camera Angle

|               | Byte 1-2     |
|---------------|--------------|
| Variable Name | message_type |
| Variable Type | uint8_t      |
| Min Value     | 3            |
| Max Value     | 3            |
| Example       | 3            |

Take Photo

|               | Byte 1-2     |
|---------------|--------------|
| Variable Name | message_type |
| Variable Type | uint8_t      |
| Min Value     | 4            |
| Max Value     | 4            |
| Example       | 4            |

Get Speed

|               | Byte 1-2     |
|---------------|--------------|
| Variable Name | message_type |
| Variable Type | uint8_t      |
| Min Value     | 5            |
| Max Value     | 5            |
| Example       | 5            |

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

|               | Byte 1-2 | Byte 3   | Byte 4   |
|---------------|----------|----------|----------|
| Variable Name | uint8_t  | uint16_t | uint16_t |
| Variable Type | uint8_t  | uint16_t | uint16_t |
| Min Value     | 8        | 0        | 0        |
| Max Value     | 8        | 360      | 360      |
| Example       | 8        | 350      | 25       |

Display Speed

|               | Byte 1-2 | Byte 3  |
|---------------|----------|---------|
| Variable Name | uint8_t  | uint8_t |
| Variable Type | uint8_t  | uint8_t |
| Min Value     | 11       | 0       |
| Max Value     | 11       | 20      |
| Example       | 11       | 3       |
