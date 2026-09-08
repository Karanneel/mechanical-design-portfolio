# 1/8 Scale RC Race Car

Chassis, drivetrain, and suspension for a Technoxian competition RC electric car. Designed for a friend's competition team - I handled all mechanical design; the team handled electronics, driving, and race operations.

## Specs

| Parameter | Value |
|---|---|
| Scale | 1/8 |
| Drivetrain | 4WD, three-differential (front / center / rear) |
| Motor | Brushless (team-selected) |
| Battery | 4S Shorty pack |
| Overall envelope (STEP bbox) | 451 × 280 × 133 mm |

## Assembly breakdown

78 named products organised into subassemblies:

- **Chassis** — main 4 mm chassis plate with battery tray, motor mount base and clamp, battery straps, undertray/skid plate
- **Front Suspension & Steering** — left/right corners (master + mirrored) with upper camber links, lower wishbones, shocks, shock tower, steering knuckles, hub carriers, Ackermann rack, tie rods, bellcranks, steering servo mount
- **Rear Suspension** — mirror-paired wishbones, shocks, shock tower, hub carriers
- **Center Drivetrain** — front and rear center driveshafts, 47T spur gear reference, motor pinion, motor shaft
- **Differentials** — front, center, rear
- **Corners** — 4 wheel + tyre assemblies with CV driveshafts (master + mirror per axle)
- **Rear Wing** — main plane + flap + left/right wing stays (mirror pair)
- **Body Reference Envelopes** — front nose, sidepods (mirror pair), canopy, rear deck, full bodywork

## Files

- [`cad/RC_Race_Car_Engineering_RevA_CleanTree.step`](cad/RC_Race_Car_Engineering_RevA_CleanTree.step) — full assembly, STEP AP214

## Reconstruction note

Original CAD was lost in a laptop hardware failure. Rebuild sourced from a surviving team STEP file (67 bodies) as ground truth for the bounding box and layout. Parametric rebuild uses grid patterns for symmetric components and mirror across XZ/YZ planes for bilateral pairs. Bounding box matched to within ~7 mm on all axes versus the team reference. Body shell, canopy, and sidepods are included as reference envelopes rather than solid shells.

An authorship signature is embossed on the right chassis-spine rail. Bodywork/canopy solid shells and an FDM printability audit remain open items for a future revision.
