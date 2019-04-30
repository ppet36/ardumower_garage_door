# ArduMower electric garage door

This repository contains resources for my electric garage door for ArduMower. I created them because cats and other animals went to the garage and left the products of their digestive tract in it :)

Used motor is UXCELL 30RPM 24V motor (https://www.ebay.com/itm/DC-24V-30RPM-8mmx15mm-Dual-D-Shape-Shaft-Electric-Power-Turbo-Worm-Geared-Motor/362278845277).

![alt](/eagle/door_sch.png?raw=true)

Pad between two 100n capacitors is connected directly to the chassis of motor to avoid interference. PCB is mounted on motor with four M4 screws.

![alt](/eagle/door_brd.png?raw=true)

Extra space (top/left) around motor is used for mounting micro-switches at desired position.

Door in the action can be seen on YouTube https://youtu.be/0yKCrzkIeTo

Signal pin is connected to perimeter sender. When sender is ON (mower is mowing) door is open. If mower is in garage eq. charging and perimeter sender is OFF, door is closed. Signal is connected on pin D10 a firmware of perimeter sender slightly modified to control pin.
