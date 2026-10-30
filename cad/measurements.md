# Measurements

All in mm, measured by me with calipers. Motor is the JGB37-520 (12 V, 110 RPM) with encoder.

## Motor

| Name | What | Value |
| --- | --- | --- |
| Shaft width | round part | 6.0 |
| Flat to round | across the shaft at the flat | 5.6 |
| A | shaft length, tip to top of the ring | about 15 |
| B | ring height above the gearbox face | 6.09 |
| Ring width | diameter of the raised ring | 11.97 |
| C | gearbox face to the board at the back | 48.8 |
| D | motor body width | 36.77 |
| E | mounting holes, center to center across (6 holes, M3) | 31 |
| d | mounting hole diameter | about 2.86 |
| F | mounting hole depth | at least 6.83 (rod too thick to reach the bottom) |
| G1 | top edge of body to top of ring | about 18.75 |
| G2 | bottom of ring to bottom edge of body | 5.2 |
| L | length of the flat on the shaft | 12.22 |
| W | round board at the back, width | 32.68 |
| H | white plug sticks out past the board | 5.74 |

## What I learned

- The 6 mounting holes are centered on the motor body, but the shaft is NOT. It sits about 6.75 mm off center (toward the G2 side).
- So the mount needs the shaft hole in one place and the 6 holes on a 31 mm circle centered about 6.75 mm away from it.
- The 3 other screws on the gearbox face hold the gearbox together. They are not mounting holes.

## Boards

| Part | Measurement | mm |
|---|---|---|
| IMU | Length | 25.95 |
| IMU | Width | 15.55 |
| IMU | Thickness with pins | 11.20 |
| IMU | Hole diameter (d) | 3.23 |
| IMU | Hole center to center (S) | 19.90 |
| Driver | Length | 20.16 |
| Driver | Width | 20.35 |
| Driver | Thickness with pins | 11.10 |
| ESP32 | Length | 57 |
| ESP32 | Width | 28.41 |
| ESP32 | Thickness with pins | 13.05 |
| ESP32 | Hole diameter (d) | 3.11 |
| ESP32 | Hole center to center, along the long side (S) | 52 |
| Buck | Length | 43.6 |
| Buck | Width | 21.18 |
| Buck | Height, board bottom to top of tallest capacitor (T) | 11.57 |
| Buck | Hole diameter (d) | 3.11 |
| Buck | Hole center to center, diagonal (S) | 34.6 |

The driver has no mounting holes, so it gets clips or pegs. The IMU, ESP32, and buck converter holes all fit M3 screws.

## Battery (measured Oct 28)

| Measurement | mm |
|---|---|
| Length (with casing) | 76 |
| Width | 35.60 |
| Thickness | 19.30 |
| Wires + plug, from pack to plug tip | 92 |

Plan: strap slot goes across the middle of the pack, and I leave about 100 mm of room past the wire end for the wires and plug.

Everything is measured now.
