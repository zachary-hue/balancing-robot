# Plan

Goal: TILT balancing on its own by early December, before finals (last final is Dec 16). About 10 to 12 hours a week.

## Where I am (Nov 6)

- [x] Every part tested (motors, encoders, buck converter set to 5.0 V)
- [x] Every part measured with calipers ([design/measurements.md](design/measurements.md))
- [x] Design locked in ([design/](design/))
- [x] Learned Onshape on the real parts: motor fit-test plate and middle plate, both printed

## Next up

**Frame (Onshape and printing)**
- [ ] Bottom plate: IMU, buck converter, driver clips, motor mount tabs, wire slots
- [ ] Motor mounts: same hole pattern as the fit-test plate, plus a tab that bolts to the bottom plate
- [ ] Wheels: 90 mm, D-shaped hole, set screw, find a tire or print one in TPU
- [ ] Top plate: battery strap slots, XT60, switch, TILT logo
- [ ] Get 8 M3 standoffs, 80 mm long (or stack 40 mm ones)
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
