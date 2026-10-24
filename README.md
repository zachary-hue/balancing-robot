# balancing-robot

Building a self-balancing robot from scratch: ESP32, my own firmware, a 3D-printed frame designed in Onshape, and a custom PCB designed in KiCad. I am logging everything I learn along the way as well!

## Why I'm doing this

I don't want to just follow a tutorial. I want to understand every part of this robot and be able to build the next one on my own. So I'm learning each piece as I go:

- Onshape and 3D printing, so I can print parts to exact measurements (wheels and a frame)
- KiCad, so I can design a PCB and get it manufactured
- Soldering, wiring, and figuring out where everything should go
- Writing my own code for the robot, including I2C, UART, motor control, and PID

## The robot

| Part | What it does |
| --- | --- |
| ESP32 dev board (38-pin) | The brain. Runs the code. |
| MPU-9250/6500 IMU | Measures tilt (accelerometer and gyro) over I2C |
| TB6612FNG motor driver | Takes the ESP32's signals and drives the motors |
| 2x JGB37-520 motors (12 V, 110 RPM) with encoders | Move the wheels and measure how far they turn |
| LM2596 buck converter | Steps the battery's 7.4 V down to 5.0 V |
| 2S LiPo battery (7.4 V, 2200 mAh) | Power |

## Where things are

- `PLAN.md`: the full plan and timeline
- `log/`: one note for each work session, written as I go
- `firmware/`: my own code
- `cad/`: Onshape designs and exported files for 3D printing
- `pcb/`: my KiCad project

## Credit

I'm using [anwarminarso/ESP32-SelfBalancing](https://github.com/anwarminarso/ESP32-SelfBalancing) as a reference to learn from. My goal is to write my own code and compare it to theirs, not copy it.
