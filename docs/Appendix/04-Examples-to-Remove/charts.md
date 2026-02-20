---
title: Appendix - Charts Example
---


``` mermaid
graph LR
  A[Start] --> B{Error?};
  B -->|Yes| C[Hmm...];
  C --> D[Debug];
  D --> B;
  B ---->|No| E[Yay!];
```

``` mermaid
sequenceDiagram
  autonumber
  Alice->>John: Hello John, how are you?
  loop Healthcheck
      John->>John: Fight against hypochondria
  end
  Note right of John: Rational thoughts!
  John-->>Alice: Great!
  John->>Bob: How about you?
  Bob-->>John: Jolly good!
```


``` mermaid
stateDiagram-v2
  state fork_state <<fork>>
    [*] --> fork_state
    fork_state --> State2
    fork_state --> State3

    state join_state <<join>>
    State2 --> join_state
    State3 --> join_state
    join_state --> State4
    State4 --> [*]
```

``` mermaid
sequenceDiagram
  autonumber
  actor U as InPersonUser
  participant I as Isaac<br/>Controller
  box Blue
  participant M as Michael<br/>Controller Transceiver
  participant N as Neel<br/>Drone Transceiver
  end
  participant J as Jacob<br/>Steering
  participant P as K Phang<br/>Throttle
  participant H as Hafsa<br/>Gyroscope & Accelerometer
  participant A as Austin<br/>Camera Arm
  participant L as Levi<br/>Camera
  participant S as Seth<br/>Distance Sensor
  participant K as Kelton<br/>Temperature Sensor

  Note over M,N: Bluetooth Low Energy Communication

  U-->>I: Steer Drone
  I->>M: Isaac to Jacob<br/>Steer Drone to 45 degrees
  M->>N: Isaac to Jacob<br/>Steer Drone to 45 degrees
  N->>J: Isaac to Jacob<br/>Steer Drone to 45 degrees
  J->>J: Adjust Steering Servo to<br>45 degrees, Trash Message
  U-->>I: Throttle Drone
  I->>M: Isaac to K<br/>Throttle Drone to 80%
  M->>N: Isaac to K<br/>Throttle Drone to 80%
  N->>J: Isaac to K<br/>Throttle Drone to 80%
  J->>P: Isaac to K<br/>Throttle Drone to 80%
  P->>P: Adjust Motor Speed to 80%, Trash Message
  U-->>I: Turn Camera
  I->>M: Isaac to Austin<br/>Camera to 24 degrees
  M->>N: Isaac to Austin<br/>Camera to 24 degrees
  N->>J: Isaac to Austin<br/>Camera to 24 degrees
  J->>P: Isaac to Austin<br/>Camera to 24 degrees
  P->>A: Isaac to Austin<br/>Camera to 24 degrees
  A->>A: Adjust Camera Servo to<br>24 degrees, Trash Message
```
