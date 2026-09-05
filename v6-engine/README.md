# Toyota 2GR-FE V6 Engine — Assembly Exercise

3.5 L 60° V6, DOHC, dual VVT-i. Modeling exercise from published production dimensions. Simplified assembly focused on rotating-assembly kinematics and overall architecture — not a production digital twin.

## Reference specifications (Toyota 2GR-FE)

| Parameter | Value | Source |
|---|---|---|
| Displacement | 3,456 cc | Toyota |
| Bore | 94.0 mm | Toyota |
| Stroke | 83.0 mm | Toyota |
| Bank angle | 60° | Toyota |
| Bore pitch (same bank) | 105.5 mm | Toyota |
| Bank offset | 36.6 mm | Toyota |
| Connecting rod length (C-C) | 147.5 mm | Toyota service manual |
| Rod big end / small end | 56.0 / 22.0 mm | Toyota service manual |
| Timing chain pitch | 9.525 mm (3/8") | Toyota |
| Firing order | 1-2-3-4-5-6 (120° intervals) | Toyota |
| Cylinder layout | Bank 1: 1-3-5, Bank 2: 2-4-6 | Toyota TSB |

## Assembly breakdown

150 solids, 57 named products. Structured as a proper feature tree with master/pattern/mirror conventions:

- **Cylinder Block and Lower Crankcase** — 60° V6 block, lower bedplate reference, oil pan reference
- **Rotating Assembly** — crankshaft (83 mm stroke, split crankpins for even-fire 120° intervals), 6 pistons + 6 connecting rods + 6 wrist pins (patterned per bank)
- **Cylinder Heads and Valvetrain** — bank 1 head (master) + bank 2 head (mirrored and offset), 24 valves (2 intake + 2 exhaust per cylinder × 6)
- **Camshafts** — intake and exhaust camshafts with patterned lobes
- **Timing Drive** — crank timing sprocket, 2 intake and 2 exhaust VVT-i cam sprockets (circular tooth pattern)
- **Cam Covers** — bank 1 + bank 2 mirror
- **Reference Envelopes** — upper intake plenum, intake system, front timing cover

Envelope: 435 × 362 × 470 mm (bare, no accessory drive / flywheel / dressed intake).

## Files

- [`cad/Toyota_2GR_FE_Architecture_RevA_CleanTree.step`](cad/Toyota_2GR_FE_Architecture_RevA_CleanTree.step) — full assembly, STEP AP214

## Reconstruction note

Original CAD (bachelor's-era hobby exercise) was lost in a laptop hardware failure. This rebuild works from Toyota's published 2GR-FE dimensions cross-referenced across multiple sources (service manual extracts, Toyota TSB for cylinder banking, forum-verified stock rod dimensions).

Simplified deliberately: valves modeled as swept solids without ports, cam profiles as patterned lobes without measured lift curves, timing chains omitted (sprocket positions and ratios preserved), no fasteners, no accessory drive. Scope is assembly architecture and rotating-assembly kinematics — the split-pin crank layout that gives a 60° V6 its even 120° firing is the interesting mechanism to model correctly, and it is preserved here.
