# Competition quadcopter airframe

Airframe model of an 8 kg class Quad-X competition quadcopter with 15" propellers and dual 6S batteries in series.

## Overview

Designed around an electronics stack and competition mechanism chosen by the team, the airframe covers the frame, four arm assemblies, landing gear, and the mounting for batteries and avionics, where flight tuning and electronics stayed with the team. Mechanical design was my part of the build, aiming to keep the packaging clean enough for the team to integrate hardware without reworking the structure.

## Specifications

| Parameter | Value |
|---|---|
| Class | 8 kg |
| Configuration | Quad-X |
| Propeller size | 15" |
| Battery | Dual 6S in series (12S) |
| Motor-to-motor diagonal | about 500 mm |
| Overall envelope (STEP bounding box) | 494 x 494 x 171 mm |

## Assembly breakdown

45 named products, organised by subsystem:

| Subsystem | Contents |
|---|---|
| Frame | Top plate, bottom plate, standoffs |
| Arms | Four arm assemblies (front-left, front-right, rear-left, rear-right), each with arm tube, inner clamp, motor plate, motor end clamp |
| Propulsion | Four propulsion units, one per arm |
| Landing gear | Four legs and two skids |
| Power | Battery pair (left and right) with power distribution board |
| Avionics | Flight controller, four ESCs on an ESC tray, RC receiver |
| Payload | Reference volumes for the competition mechanism |

## Files

```text
drone/
  cad/Racing_Drone_Verified.step    full assembly, STEP AP214
```

## Reconstruction note

Rebuilt from published sizing decisions and layout references after the original CAD was lost in a laptop hardware failure. The `_Verified` suffix means the assembly was structurally audited, with 46 solids, the subassembly tree preserved, and every bilateral pair modelled as a master plus a mirror. Airworthiness and flight performance of this file are untested.
