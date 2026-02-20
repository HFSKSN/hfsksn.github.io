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
  P->>P: Adjust Motor Speed to 80%,<br/> Trash Message

  U-->>I: Turn Camera
  I->>M: Isaac to Austin<br/>Camera to 24 degrees
  M->>N: Isaac to Austin<br/>Camera to 24 degrees
  N->>J: Isaac to Austin<br/>Camera to 24 degrees
  J->>P: Isaac to Austin<br/>Camera to 24 degrees
  P->>H: Isaac to Austin<br/>Camera to 24 degrees
  H->>A: Isaac to Austin<br/>Camera to 24 degrees
  A->>A: Adjust Camera Servo to<br/>24 degrees, Trash Message

  U-->>I: Take Picture
  I->>M: Isaac to Levi<br/>Take Photo
  M->>N: Isaac to Levi<br/>Take Photo
  N->>J: Isaac to Levi<br/>Take Photo
  J->>P: Isaac to Levi<br/>Take Photo
  P->>H: Isaac to Levi<br/>Take Photo
  H->>A: Isaac to Levi<br/>Take Photo
  A->>L: Isaac to Levi<br/>Take Photo
  L->>L: Take and Save Image,<br/>Trash Message

  loop
    I->>M: Isaac to Hafsa<br/>Get Speed
    M->>N: Isaac to Hafsa<br/>Get Speed
    N->>J: Isaac to Hafsa<br/>Get Speed
    J->>P: Isaac to Hafsa<br/>Get Speed
    P->>H: Isaac to Hafsa<br/>Get Speed
    H->>H: Collect Acceleration Data,<br/>Calculate, Trash Message
    H->>A: Hafsa to Isaac<br/>Speed is 3m/s
    A->>L: Hafsa to Isaac<br/>Speed is 3m/s
    L->>S: Hafsa to Isaac<br/>Speed is 3m/s
    S->>K: Hafsa to Isaac<br/>Speed is 3m/s
    K->>N: Hafsa to Isaac<br/>Speed is 3m/s
    N->>M: Hafsa to Isaac<br/>Speed is 3m/s
    M->>I: Hafsa to Isaac<br/>Speed is 3m/s
    I->>I: Display "Speed = 3m/s"<br/>on OLED screen

    I->>M: Isaac to Seth<br/>Get Distance
    M->>N: Isaac to Seth<br/>Get Distance
    N->>J: Isaac to Seth<br/>Get Distance
    J->>P: Isaac to Seth<br/>Get Distance
    P->>H: Isaac to Seth<br/>Get Distance
    H->>A: Isaac to Seth<br/>Get Distance
    A->>L: Isaac to Seth<br/>Get Distance
    L->>S: Isaac to Seth<br/>Get Distance
    S->>S: Collect Distance Data,<br/>Trash Message
    S->>K: Seth to Isaac<br/>Distance is 4.54m
    K->>N: Seth to Isaac<br/>Distance is 4.54m
    N->>M: Seth to Isaac<br/>Distance is 4.54m
    M->>I: Seth to Isaac<br/>Distance is 4.54m
    I->>I: Display "Distance = 4.54m"<br/>on OLED screen

    I->>M: Isaac to Kelton<br/>Get Temperature
    M->>N: Isaac to Kelton<br/>Get Temperature
    N->>J: Isaac to Kelton<br/>Get Temperature
    J->>P: Isaac to Kelton<br/>Get Temperature
    P->>H: Isaac to Kelton<br/>Get Temperature
    H->>A: Isaac to Kelton<br/>Get Temperature
    A->>L: Isaac to Kelton<br/>Get Temperature
    L->>S: Isaac to Kelton<br/>Get Temperature
    S->>K: Isaac to Kelton<br/>Get Temperature
    K->>K: Collect Temperature Data,<br/>Trash Message
    K->>N: Kelton to Isaac<br/>Temperature is 23C
    N->>M: Kelton to Isaac<br/>Temperature is 23C
    M->>I: Kelton to Isaac<br/>Temperature is 23C
    I->>I: Display "Temperature = 23C"<br/>on OLED screen

    H->>H: Collect Angular Momentum data, Calculate
    H->>A: Stabilize Arm<br>Camera to 3 degrees
    A->>A: Adjust Camera Servo to<br/>3 degrees, Trash Message
  end
```
