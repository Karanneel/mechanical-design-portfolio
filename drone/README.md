# Competition Quadcopter Airframe

8 kg class competition quadcopter, Quad-X configuration, 15" propellers, dual 6S batteries in series, dedicated landing gear and competition-mechanism interface. Designed by me; electronics and flight tuning by the team.

## Specs

| Parameter | Value |
|---|---|
| Class | 8 kg |
| Configuration | Quad-X |
| Propeller size | 15" |
| Battery | Dual 6S in series (12S) |
| Motor-to-motor diagonal | ~500 mm |
| Overall envelope (STEP bbox) | 494 × 494 × 171 mm |

## Assembly breakdown

45 named products, organised by subsystem:

- **Frame** — top plate, bottom plate, standoffs
- **Arms** — 4 arm assemblies (front-left, front-right, rear-left, rear-right), each with arm tube, inner clamp, motor plate, motor end clamp
- **Propulsion** — 4 propulsion units, one per arm
- **Landing Gear** — 4 legs and 2 skids
- **Power System** — battery pair (left + right) plus power distribution board
- **Avionics** — flight controller, 4 ESCs on an ESC tray, RC receiver
- **Payload + Competition Mechanism Envelope** — reference volumes for downstream integration

## Files

- [`cad/Racing_Drone_Verified.step`](cad/Racing_Drone_Verified.step) — full assembly, STEP AP214

## Reconstruction note

Rebuilt from published sizing decisions and layout references after original CAD was lost in a laptop hardware failure. The `_Verified` suffix denotes that the assembly was structurally audited (46 solids, subassembly tree preserved, all bilateral pairs modeled with master + mirror). No claim is made about airworthiness or flight-tested performance of this specific file.
