# mutliwii-quadrocopter
Custom Multiwii FW for quad &amp; how-to build steps 


Sources how-to build:
* https://www.instructables.com/id/The-Almost-Complete-Guide-to-Building-an-ArduCopte/
* 




Points:

## Soldering the Motor Wires to the ESC's
    
The motors run off of AC electricity. Which means there is no such thing as polarity when it comes to soldering the motor wires to the ESC. The MegaPirate configuration calls for the 6 motors to alternate between Clockwise and Counter Clockwise.

Decide which side of the hexacopter you want to be the "front" then mark each arm with its corresponding number. Start with number 8 then move CCW marking the rest of the arms (3, 5, 7, 2, 6).

On my Turnigy ESC, there are 3 wires that connect to the motor marked A-B-C. Use this setup to correctly wire the ESC's to the motors:

* (3,7,6) CCW:
  - A->Black
  - B->Red
  - C->Green
* (8,5,2) CW:
  - A->Black
  - B->Green
  - C->Red 

## Hooking Up the ESC Wires to the Controller

The D section is where you plug your ESC's into. You did put your numbers on the ESC's right?
8 -> D8
3 -> D3
5 -> D5
7 -> D7
2 -> D2

## MultiWii Pro Transmitter Wiring

The side that starts with "A" is where you plug in the transmitter wires.
 - A8 = Throttle
 - A9 = Aileron/Roll
 - A10 = Elevator/Pitch
 - A11 = Rudder/Yaw
 - A12 = Ch5/Radio 5
 - A13 = Ch6/Radio 6
 - A14 = Ch7/Radio 7
 - A15 = Ch8/Radio 8

That's the general input layout for the Multiwii pro 2.0. This is the layout you will use to connect the Turnigy 9x reciever to the Multiwii pro 2.0.
 - A8 = Channel 3
 - A9 = Channel 1
 - A10 = Channel 2
 - A11 = Channel 4
 - A12 = Channel 6
 - A13 = Channel 5
 - A14 = Ch7/Radio 7
 - A15 = Ch8/Radio 8

## MultiWii Pro GPS Wiring
he GPS provided with the Multiwii pro 2.0 comes with its own servo wires. Plug in the small connector to the GPS, then wire the other end in this configuration. The GPS is hooked up to the lower center pins on the board:
- GND -> GND
- RXA -> TX2
- TXA -> RX2
- VDD -> 5V

You'll notice on the ends of the connection there are "PPS and PEN". These are not used, simply peel them back and use tape/heat shrink to seal them in place.

## Propeller Installation

[TODO....]