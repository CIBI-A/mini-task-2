### Robot control

### Problem statement:
 To control a Robot to move in any direction.
### Ideation:
In the actual project they have used DTMF, that is

Phone >> DTMF decoder >> motor driver >> motor


| Method | Feasibility | Advantages | Disadvantages |
|-----------|-------------|------------|---------------|
|DTMF |easy to implement|Simple circuit and microcontroller is not necessary | It cannot be implemented without a phone. It can be made wireless only by using two phones|
|IR |knowledge about IR receiver circuit|Robot can be controlled wirelessly and circuit is easy to implement|IR light should fall on receiver and coverage range is small(approx 10m)|
|RF |Need to know about RF transmitter and receiver module|Robot can be controlled wirelessly. RF doesn't require line of sight, it can be operated from any where within coverage range(approx 50m)| Hardware is little bit complex|

##### Choosing a pipeline:
The best way depends on the neccessity, However we can eliminate DTMF because we need 2 phones to make it wireless.

Therefore we can choose IR or RF method

###### IR: 
IR remote >> IR receiver ic >> Microcontroller >> motor driver >> motor

Find the IR signals of the remote and code according to the neccessity. Receiver ic is connected to arduino as input and motor driver is connected as output.We can upgrade to gesture control also.
 

###### RF:
Push button >> encoder >> RF transmitter >>RF receiver >> decoder >> Microcontroller >> motor driver >> motor

Microcontrolled can be removed. Use push buttons as which direction to move. This can also be upgraded to gesture control.


[DTMF method](https://www.electronicshub.org/dtmf-mobile-controlled-robot-without-microcontroller/),
[IR method](https://www.electronicsforu.com/electronics-projects/hardware-diy/arduino-based-rf-controlled-robot),
[RF method](https://www.instructables.com/id/ARDUINO-based-IR-remote-control-robot/)

[IR vs RF](https://www.bronsondesign.com/blog/ir-vs-rf-remote-control/)
