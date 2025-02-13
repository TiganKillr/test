## Introduction
Welcome to my page about the **Arm Manipulated Camera** Robot (AMC).

The AMC is a 5-Axis robot arm designed to hold a smartphone for video recording.\
It offers a built in recorder and player for camera movements, or precision controls via Wi-Fi.

&nbsp;
## Table of contents
> [Features](#features)\
[Hardware Overview](#hardware)\
[Software Overview](#software)\
[Mechanical Design](#mechanical)

&nbsp;
<a name="features"/>

## Features
The specifics of this project are as follows:
- Constrained to 5 degrees of freedom and a length of 40cm.
- Equipped with a built-in position saver for repeatable camera movements.
- Includes a web-based interface for precise and external control.
- Made using 3D printed parts in PLA.

&nbsp;
<a name="hardware"/>

## Hardware Overview
### Electronics
- <ins>**ESP32-C3**</ins>\
   The development board for this robot arm will be the ESP32-C3 Super Mini.\
   It has:
   - Built-in antenna for transceiving WiFi / Bluetooth signals.
   - 160 MHz clock speed.
   - Small size and power consumption.
   - Runs on 5V or 3v3

- <ins>**AS5600**</ins>\
   To capture the position of each link, I will be using AS5600 rotary magnetic encoders.
   - 12-bit resolution
   - I²C Controlled, so SDA and SCL pins.
   - Runs on 3v3
### Actuators
- <ins>**MG996R Servo**</ins>\
  This servo has been modified by me to act like a geared DC motor.\
  By disconnecting the potentiometer and grinding the output gear notch, I loose out on position control.

&nbsp;
<a name="software"/>

## Software Overview

&nbsp;
<a name="mechanical"/>

## Mechanical Design



&nbsp;

.

&nbsp;

.

&nbsp;

.

&nbsp;

Rewrite:

The armature lengths are as follows:
| Lower Link | Upper Link | Wrist Link Rear | Wrist Link Front | 
| -- | -- | -- | -- |
| 17.5cm | 12.5cm | 5cm | 5cm |

And the corresponding torque values.

**Note:** These are estimated values.

| Shoulder Joint | Elbow Joint | Wrist Joint | 
| -- | -- | -- |
| 24.33kgf/cm | 10.5kgf/cm | 3.56kgf/cm |
| 2.39Nm | 1.03Nm | 0.35Nm |

&nbsp;
## Electronics details

I will be using 5v and 3v3 power throughout the circuit.

Here are the active components I will be using:

| Component | Voltage | Description |
| -- | -- | -- |
| ESP32-C3 Super Mini | Both | Development board to control the device. |
| MG966R Servo | 5V | Hobby servo that will drive the gearboxes. |
| Logic Level Shifter | Both | Increases/decreases voltage for communication interfaces. |
| AS5600 Encoder | 5V | Magnetic encoder to measure joint travel |


&nbsp;
<details>
<summary>Tips for collapsed sections</summary>

You can add a header
---
Some test things

```ruby
   puts "Hello World"
```
</details>
