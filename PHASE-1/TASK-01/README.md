# Zelbytes Arduino Internship


Objective

Set up Arduino IDE, connect the Arduino Uno board, and verify basic board operation.

Hardware Used

- Arduino Uno R3 Compatible
- USB Type-B Cable
- Windows Laptop

Software Used

- Arduino IDE 2.3.9

Tasks Performed

1. Installed Arduino IDE.
2. Connected Arduino Uno board.
3. Verified board selection.
4. Uploaded BlinkSerial sketch.
5. Tested Serial Monitor communication.
6. Uploaded PinMapInfo sketch.

Files

BlinkSerial.ino

- Blinks onboard LED on pin 13.
- Prints board initialization messages.

PinMapInfo.ino

- Displays Arduino pin mapping information.
- Provides serial communication guidelines.

Expected Output

BlinkSerial

- LED blinks every 500 ms.

Serial Monitor

Zelbytes Arduino Foundations — Day 1

Board: check Tools > Board matches hardware

Analog pins A0-A5 map to digital 14-19

Avoid pins 0/1 when using USB Serial

Repository Structure

- BlinkSerial.ino
- PinMapInfo.ino
- README.md

Learning Outcomes

- Arduino IDE installation and setup
- Arduino board programming
- Serial communication basics
- Understanding Arduino pin mapping

Status

Completed