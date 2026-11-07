# cad

My Onshape parts and what's been printed. The design behind them (sizes, layout, and why) is in [../design/](../design/).

Onshape document: TILT (link to add)

| Part | Designed | Printed | Notes |
| --- | --- | --- | --- |
| Motor fit-test plate | yes | yes | Fits perfectly. Proves the hole pattern and the 6.75 mm shaft offset. |
| Middle plate | yes | yes | ESP32 holes, wire slots, honeycomb |
| Top plate | yes | printing | Battery strap slots, wire hole, spare holes, raised TILT logo and light bar in a second color |
| Bottom plate | yes | printing | IMU holes, buck converter slots, motor mount holes, wire slots, raised front arrow. Driver gets foam tape (no holes). |
| Motor mounts (x2) | yes | printing | L shape: wall uses the fit-test hole pattern, tab screws up into the bottom plate (2.8 mm holes, M3 x 6). Second one is mirrored. |
| Wheels (x2) | yes | printing | 84 mm with a groove for a tire (TPU or bike tube) to make 90 mm. 5 rim holes, D-shaped shaft hole. |
| Tires (x2) | no | no | TPU if Thinkbox has it, otherwise bike inner tube |
| Frame v2 | no | no | Rebuilt around the PCB later |

Plans for the new parts: [bottom plate](../design/images/parts/bottom-plate-plan.png), [motor mount side view](../design/images/parts/motor-mount-side-view.png), [motor mount 3D](../design/images/parts/motor-mount-3d.png). How I built each one is in the [Nov 7 log](../log/2026-11-07.md).

## Print settings

| | Plates | Wheels and motor mounts |
| --- | --- | --- |
| Material | PLA (stiff) | PETG (tougher, survives falls) |
| Layers | 0.16 mm High Quality | 0.16 mm High Quality |
| Walls / infill | 3 / 20% | 4 / 40% |
| Supports | none | none |
| Extras | Ironing on top, seam aligned, filament change where the raised logo starts | Ironing on top, seam aligned, auto brim |
