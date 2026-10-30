# TILT robot: full handoff (as of Oct 30, 2026)

Read this first in any new chat. Zachary's rules: short, super simple, no jargon, no m dashes, student-authentic drafts. He learns by doing (Claude gives steps, he does them, Claude explains why). He does his own caliper measurements. Claude makes decisions. Personal GitHub only: `zachary-hue`, never the business account. He pushes with GitHub Desktop.

## Project
Self-balancing robot named TILT. ESP32, TB6612FNG motor driver, MPU-9250/6500 IMU, LM2596 buck set to 5.0 V, 2 x JGB37-520 12 V 110 RPM motors with encoders, 2S 7.4 V 2200 mAh Crazepony LiPo. Based on `anwarminarso/ESP32-SelfBalancing`. Goals: learn and own every part (Onshape CAD, 3D printing, KiCad custom PCB, soldering, own firmware in VS Code + PlatformIO, weekly lessons). Finish Dec 6, last final Dec 16. 10 to 12 hours a week. PCB order by Nov 20. Fallback: frame v1 balances even if the PCB is late.

## Design decisions
- 3 printed PLA plates (3 mm, 3 walls, 20% infill) on 4 M3 hex standoffs per gap, about 20 cm tall. Plates about 136 x 88 mm rounded octagons.
- Bottom plate: IMU, driver, buck. Middle plate: ESP32. Top plate: battery with velcro strap through slots.
- Honeycomb holes in the middle plate. A row of spare M3 holes along the back edge of every plate for adding stuff later.
- Front is +Z. Front light bar, arrow, TILT logo on the top plate.
- Colors: black plates, dark blue wheels, black O-ring, gray motor mounts, light blue logo/arrow/trim, silver standoffs.
- Wheels 65 mm with O-ring, printed with a D-shaped hole and set screw. Axle height 32.5 mm.
- Motor mounts about 4 mm thick, bolt to gearbox face with M3 x 8 screws. Plate screws stay M3 x 6.

## Measurements (mm), all in cad/measurements.md in the repo
Motor: 6 M3 holes on a 31 mm circle centered on the body. Shaft is about 6.75 mm off center. The 3 other screws on the gearbox face are not mounting holes. Shaft diameter 6, flat to round 5.6, shaft length about 15, ring height 6.09, G1 18.75, G2 5.2, W 32.68, H 5.74, L 12.22, C 48.8, D 36.77, E 31, d 2.86, f at least 6.83.
IMU: 25.95 x 15.55, thickness with pins 11.20, holes 3.23 diameter, 19.90 apart.
Driver: 20.16 x 20.35, thickness with pins 11.10, no mounting holes (needs clips or pegs).
Battery: 76 x 35.60 x 19.30, wires plus plug 92 from pack to plug tip.
ESP32: 57 x 28.41, thickness with pins 13.05, holes 3.11 diameter, 52 apart.
Buck: 43.6 x 21.18, height 11.57, two holes 3.11 diameter on a diagonal, 34.6 apart.

## Done
- Plain-English plan doc (claude.ai Docs artifact "Self-Balancing Robot: Build & Learning Plan", https://claude.ai/artifact/15RHFhCDQJ77RonoB83vz1). It does not yet have the measured numbers or the M3 x 8 change.
- Realistic annotated renders saved in repo `images/` (tilt-v1-annotated.png, tilt-v1-front-view.png, tilt-v1-top-view.png).
- README.md and cad/README.md have design notes. cad/measurements.md has every measurement above.
- IMU and driver headers soldered (photos of joints not yet checked).
- Measurement guide diagrams made for motor, IMU, driver, battery, ESP32, buck.

## To do
1. Plate layout drawing using all measurements, then Onshape CAD. The render still draws the motors centered on the axle and ignores the 6.75 mm shaft offset.
2. Repo PLAN.md still has the old 8-phase Dec 20 plan. Sync it to the 6-week plan. Add a log entry.
3. Update the plan doc with the measured numbers, M3 x 8 screws and shaft offset.
4. Replace the stale Project doc claude/self-balancing-robot-project-plan.md.
5. Check solder-joint photos. Then PlatformIO setup, 8 small test sketches, 6 weekly lessons (week 1: I2C, UART, motor basics).
6. Ask: exams or deadlines before Dec 16? Does he have M3 hardware (Thinkbox has standoffs and screws)?

## Schedule
6 weeks, Oct 24 to Dec 6. Thanksgiving week light.
