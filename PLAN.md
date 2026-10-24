# Plan

I'm doing this in eight weeks, from Oct 24 to Dec 20, 2026. The one hard deadline is ordering the PCB by Dec 4. Each phase has a "done when" so I know when to move on.

## Timeline

| Phase | Dates | Focus |
| --- | --- | --- |
| 0 | Oct 24 | Finish soldering, measure every part |
| 1 | Oct 25 to Nov 1 | Bring-up: test each part from code |
| 2 | Nov 2 to Nov 8 | Control code, bench wiring |
| 3 | Nov 9 to Nov 15 | Frame v1 and wheels (Onshape and 3D printing) |
| 4 | Nov 16 to Nov 22 | Assemble and get the first balance |
| 5 | Nov 23 to Nov 29 | KiCad schematic |
| 6 | Nov 30 to Dec 6 | KiCad layout, **order the PCB by Dec 4** |
| 7 | Dec 7 to Dec 13 | Frame v2 around the PCB |
| 8 | Dec 14 to Dec 20 | Solder the PCB, assemble v2, final tuning |

## Phase checklists

**Phase 0**
- [ ] Solder the IMU header and the driver headers
- [ ] Measure the motor, boards, and battery with calipers
- [ ] Start the Onshape CAD Basics pathway

**Phase 1**
- [ ] Install the Arduino IDE, the ESP32 board package, and the libraries; upload Blink
- [ ] Run an I2C scanner and find the IMU at 0x68
- [ ] Run motor and encoder tests
- [ ] Charge the LiPo once, while watching it, on a hard surface
- [ ] Onshape: Sketching and Part Studios courses, then import the JGB37-520 motor model from GrabCAD and check it against my calipers

**Phase 2**
- [ ] Wire the whole robot on the bench with jumper wires
- [ ] Try the reference firmware and watch the wheels react to tilt
- [ ] Onshape: Assemblies course, then import or model every part

**Phase 3**
- [ ] Design the frame around my part models
- [ ] Print the wheels first, then the frame in parts

**Phase 4**
- [ ] Assemble v1 and tune the PID gains one at a time
- [ ] Done when it stays up for 10 seconds

**Phase 5 and 6**
- [ ] Draw the schematic as a carrier board for my modules
- [ ] Lay out the board, run the checks, and order it by Dec 4

**Phase 7 and 8**
- [ ] Redesign the frame around the PCB and print v2
- [ ] Solder the PCB, assemble v2, retune, and record a demo

## Weekly lessons

Each week I get one lesson with a practice task.

| Week | Lesson |
| --- | --- |
| 1 | I2C and UART |
| 2 | PWM, H-bridges, and encoders |
| 3 | IMU, accelerometer and gyro, and filtering |
| 4 | Control and PID |
| 5 | Reading schematics and PCB basics |
| 6 | PCB layout: traces, ground, decoupling |
| 7 | Timers, interrupts, and RTOS tasks |
| 8 | Debugging with a logic analyzer |

## Risks

- **Finals:** I'm assuming they fall around Dec 10 to 19, so phases 7 and 8 are light.
- **PCB lead time:** boards take 1 to 2 weeks. The robot should balance on v1 even if the PCB is late.
- **LiPo safety:** only charge while I'm watching, on a hard surface, and don't run it below about 6.6 V.
