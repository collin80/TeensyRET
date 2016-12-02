Teensy-RET
=======

Reverse Engineering Tool based around a custom board with a socket for Teensy 3.6. The board also has SN65HVD234
transceivers, an I2C to OneWire interface chip, and an Adafruit BLE module. Only the transceivers are relevant to this
project but the project is setup to use pin 2 for enabling CAN0 and pin 35 for CAN1 enable. Set this as appropriate for your
designs or to 255 to disable if no enable pin is needed.

The project builds with the Arduino IDE with the TeensyDuino add-on

WARNING: This is currently an early port of GVRET. Some things won't work, some things will crash. But, initial testing shows
compatibility with SavvyCAN, ability to read frames to the console, and stability at high bus loads.

#### Requirements:

1.6.x Arduino IDE

TeensyDuino 1.31 or newer

FlexCAN library from me (https://github.com/collin80/FlexCAN_Library)

SDCard-Beta library  (https://github.com/greiman/SdFat-beta)

The canbus is supposed to be terminated on both ends of the bus. This should not be a problem as this firmware will be used to reverse engineer existing buses.

#### License:

This software is MIT licensed:

Copyright (c) 2014-2017 Collin Kidder, Michael Neuweiler, Charles Galpin

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be included
in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

