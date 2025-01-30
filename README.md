## AMC Robot

Welcome to my page about the **Arm Manipulated Camera** Robot (AMC).

This is my first robotics project thats deals with electromechanical systems and software.

&nbsp;
## What is it?

The AMC is a robot arm designed to be used in video recording / photography.

In the future, the end effector will become swappable with other tools and provide other uses.

![alt text](https://github.com/TiganKillr/test/blob/main/placeholder.jpg?raw=true)

&nbsp;
## Armature details

The robot arm consists of 5 DOF starting with Roll, Yaw, Yaw, Yaw and Roll.

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

| Component | Voltage | Description |  |  |  |
| -- | -- | -- | -- | -- | -- |
| ESP32-C3 Super Mini | Both | Development board to control the device. |  |  |  |
| MG966R Servo | 5V | Hobby servo that will drive the gearboxes. |  |  |  |
| Logic Level Shifter | Both | Increases/decreases voltage for communication interfaces. |  |  |  |
| AS5600 Encoder | 5V |  |  |  |  |


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
