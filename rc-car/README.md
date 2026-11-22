# 1/8 scale RC race car

Chassis, drivetrain, and suspension model for a Technoxian competition RC electric car.

## Overview

Built for a friend's competition team, the car split cleanly between mechanical design, which I handled completely, and electronics, driving, and race operations, which the team handled. The model covers a three-differential 4WD drivetrain, front and rear suspension with Ackermann steering, a rear wing, and reference envelopes for the bodywork, aiming to give the team a chassis they could build and tune around.

## Specifications

| Parameter | Value |
|---|---|
| Scale | 1/8 |
| Drivetrain | 4WD, three differentials (front, centre, rear) |
| Motor | Brushless, team-selected |
| Battery | 4S Shorty pack |
| Overall envelope (STEP bounding box) | 451 x 280 x 133 mm |

## Assembly breakdown

78 named products, organised into subassemblies:

| Subassembly | Contents |
|---|---|
| Chassis | Main 4 mm chassis plate with battery tray, motor mount base and clamp, battery straps, undertray and skid plate |
| Front suspension and steering | Left and right corners (master plus mirror) with upper camber links, lower wishbones, shocks, shock tower, steering knuckles, hub carriers, Ackermann rack, tie rods, bellcranks, steering servo mount |
| Rear suspension | Mirror-paired wishbones, shocks, shock tower, hub carriers |
| Centre drivetrain | Front and rear centre driveshafts, 47T spur gear reference, motor pinion, motor shaft |
| Differentials | Front, centre, rear |
| Corners | Four wheel and tyre assemblies with CV driveshafts (master plus mirror per axle) |
| Rear wing | Main plane, flap, left and right wing stays (mirror pair) |
| Body envelopes | Front nose, sidepods (mirror pair), canopy, rear deck, full bodywork |

## Files

```text
rc-car/
  cad/RC_Race_Car_Engineering_RevA_CleanTree.step    full assembly, STEP AP214
```

## Reconstruction note

The original CAD was lost in a laptop hardware failure, so the rebuild uses a surviving team STEP file (67 bodies) as ground truth for the bounding box and layout. Symmetric components use grid patterns and bilateral pairs use mirrors across the XZ and YZ planes, which brought the bounding box to within about 7 mm of the team reference on every axis. Body shell, canopy, and sidepods are reference envelopes instead of solid shells.

An authorship signature is embossed on the right chassis-spine rail. Solid shells for the bodywork and canopy, and an FDM printability audit, remain open for a future revision.
