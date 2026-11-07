# Plan

Goal: TILT balancing on its own by early December, before finals (last final is Dec 16). About 10 to 12 hours a week.

## Where I am (Nov 7)

- [x] Every part tested (motors, encoders, buck converter set to 5.0 V)
- [x] Every part measured with calipers ([design/measurements.md](design/measurements.md))
- [x] Design locked in ([design/](design/))
- [x] Learned Onshape on the real parts: motor fit-test plate and middle plate, both printed
- [x] Designed every frame part: top plate, bottom plate, motor mount, wheel. All printing, pick up Monday ([log](log/2026-11-07.md))

## Next up

**Frame (Onshape and printing)**
- [x] Bottom plate: IMU, buck converter, motor mount holes, wire slots, front arrow
- [x] Motor mounts: same hole pattern as the fit-test plate, plus a tab that screws to the bottom plate
- [x] Wheels: 84 mm with a tire groove, 5 rim holes, D-shaped hole
- [x] Top plate: battery strap slots, wire hole, TILT logo and light bar
- [ ] Pick up the prints and test the fits (motor in mount, wheel on shaft)
- [ ] Tires: TPU if Thinkbox has it, otherwise bike inner tube
- [ ] Get hardware: 8 M3 standoffs (80 mm, or stack shorter ones), M3 x 6 screws, foam tape or mini breadboard, velcro strap
- [ ] Assemble the frame

**Firmware (VS Code and PlatformIO)**
- [ ] Install VS Code and PlatformIO, upload Blink
- [ ] Work through the 8 test steps in [firmware/](firmware/)
- [ ] Wire everything on the bench, then in the frame
- [ ] Tune the PID until it stays up

**PCB (KiCad)**
- [ ] Schematic, then layout, then order it. Boards take 1 to 2 weeks, so order by about Nov 20.
- [ ] If the PCB is late, the robot still balances with jumper wires on the printed frame.

## Weekly lessons

| Week | Lesson |
| --- | --- |
| 1 | I2C and UART |
| 2 | PWM, H-bridges, and encoders |
| 3 | IMU, accelerometer and gyro, and filtering |
| 4 | Control and PID |
| 5 | Reading schematics and PCB basics |
| 6 | PCB layout: traces, ground, decoupling |

## Risks

- **Finals:** keep December light.
- **PCB lead time:** order early, and don't depend on it to balance.
- **LiPo safety:** only charge while I'm watching, on a hard surface, and don't run it below about 6.6 V.
