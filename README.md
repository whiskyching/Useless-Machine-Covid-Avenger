# Useless-Machine-Covid-Avenger
2020 was a challenging year due to the Corona Covid-19. It dramatically changes our lifestyle and human behaviors. We can't touch everything intuitively in public or before entering the shop. We subconsciously sanitize our hands before shaking hands with friends. Therefore, to contribute to this particular year, this idea comes out.

## Software Tool: 
- Python
- Arduino 
- Prusa 3D Print Slicer

## Hardware
- Solenoid Valve x1
- Arduino Uno x1
- Breadboard x1
- Powersupply 24V x1
- Adaptor 5V x1
- Button Sensor x3
- Servo Motor x3
- Relay x3
- 3D Printing Part


![image](https://user-images.githubusercontent.com/65818525/131314900-d4615d26-acfd-4686-8262-f84dd825f5f1.png)
---
![image](https://user-images.githubusercontent.com/65818525/131315070-cd2b3393-fcda-4abc-aaae-5270c74b59e0.png)
---
![image](https://user-images.githubusercontent.com/65818525/131315143-66cc6862-a089-4fed-8f52-aaf96993253a.png)
---
![image](https://user-images.githubusercontent.com/65818525/131315182-f0a29d55-1e32-49b0-a1ac-9cff369bed4e.png)

## 3D Print Parts
Here are all the components. Start from the hand, there are buttons on the palm as the trigger. And then the sprayer and the linkage mechanism on the former arm. On the upper arm, there is an actuator and the circuit. All of the customized parts are made by 3d printer, and tight by velcro on the arm.

![Explosion (1)](https://user-images.githubusercontent.com/65818525/131320547-bae617a5-193d-43ec-87a2-1bff1b13f673.gif) 
---
## Kinematic System - Linkage
This linkage mechanism is driven by two servo motors, which are installed on both sides. Through exploded view, you can see the main transmission consists of three links, two connectors, one anchor, and one rotating output. This will perfectly demonstrate the sloping curve, which you can see the motion trajectory on the right. The land gear of the plane inspires this idea by using the short link to drive the long link.

![image](https://user-images.githubusercontent.com/65818525/131320961-20c1891b-8fdb-4083-bd29-b4db70c0cb60.png) ![Kinematic](https://user-images.githubusercontent.com/65818525/131320986-a792b837-ec5c-44c3-a2bd-0a406b768647.gif)

## Trigger - Gestures
![Trigger](https://user-images.githubusercontent.com/65818525/131321188-47ec0b0d-a75e-410d-8f8b-4259bdee3cf4.png)
![upperGate](https://user-images.githubusercontent.com/65818525/131321663-258974a6-b89e-4883-bf35-52bb234dbbbe.gif) ![lowerGate](https://user-images.githubusercontent.com/65818525/131321673-6c6f6804-eebd-4322-b8bb-57f174951692.gif)

## Pneumatic System
- The spray system is driven by pneumatic. There are two metal cylinders. One is the high-pressure air CO2 cylinder. Another one is to contain sanitizer such as alcohol. Through 5 way 3 position solenoid power valves, the sanitizer will rush out to the designated port. 8mm PU pipes has been used for the connection. Besides, installing the regulating valve to adjusting the pressure for Sprayer A. And a Stop valve to control the CO2 cylinder.

![image](https://user-images.githubusercontent.com/65818525/131322014-86e7fb74-f5ca-4b3f-8761-4768e5cb9f12.png)

## Schematic Control System
![image](https://user-images.githubusercontent.com/65818525/131322093-b0723814-1820-4a71-82eb-c60d8524440a.png)

## Circuit Detail
- Two 5V relays are used to control the 24V solenoid valve to vent the pressurized air to the designated port through Arduino.
![image](https://user-images.githubusercontent.com/65818525/131322232-d7922812-617b-4d92-8cbb-7c4bddda6f9d.png)

## Arduino Code
- In Arduino code, the variables are defined first at the beginning, including servo motors, led pin(for testing), relays and button sensors. Then in the Setup function, Button ports are all input, and the rest are output. In the main function, there are two logics. One is for activating Sprayer A, another is for Sprayer B. One thing to note is the servo motor angle setting is opposite for each.

![image](https://user-images.githubusercontent.com/65818525/131322318-65b57411-d9b6-4f3e-90c2-915edddecabe.png)

## Fighting Modes
- To activate the weapon. There are three buttons on your palm. Through three two gestures, it will come out with different features. These buttons are hidden on the palm integrated with 3D printed components. 
## Gesture A: Lower Gate Activated
- Gesture A, which looks like a rocker, will trigger sprayer A, which is a soft and smooth spray.
![image](https://user-images.githubusercontent.com/65818525/131326159-4398c200-6d46-4da9-9da6-378e56e64f91.png) ![LowerGateFight (1)](https://user-images.githubusercontent.com/65818525/131325623-f2407050-f2a3-4e8c-be9e-587320b195bc.gif)

## Gesture B: Upper Gate Activated
- Gesture B, which is the badass one. You clench your fist. The sanitizer will come out with high-pressure air to clean everything you are targeting without mercy. And vent all the anger from Covid-19.

![image](https://user-images.githubusercontent.com/65818525/131326330-d69cf938-2254-4fa6-bda0-5052b878e248.png) ![UpperGateFight](https://user-images.githubusercontent.com/65818525/131326901-b8927cac-6608-4404-92fd-fc9f8b1fa8bf.gif)



## Development Process
![photo2](https://user-images.githubusercontent.com/65818525/131322851-cf6d9ba4-6b92-4486-92c8-91d576de0c20.png)
---
![image](https://user-images.githubusercontent.com/65818525/131326431-ce25abae-0717-4b24-bcc8-2f04ab90824b.png)
---
![image](https://user-images.githubusercontent.com/65818525/131326476-cd6b6b74-0373-485a-9983-3521f25bcd19.png)
---
![image](https://user-images.githubusercontent.com/65818525/131326538-78ea7308-4a41-458a-ac40-4a8a57d3e93e.png)
---
![photo](https://user-images.githubusercontent.com/65818525/131322829-ee808ec0-7b82-401d-92aa-7fa8ebc7909e.png)
---
![image](https://user-images.githubusercontent.com/65818525/131328197-1a8ec955-1856-4256-9cda-d3542d851de4.png)


