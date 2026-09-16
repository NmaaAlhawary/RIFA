# RIFA

Robot design for the **RIFA World Cup**, U13 category — one robot that plays both halves of the match without swapping attachments.

## The two documents

| | |
|---|---|
| **[3D design](rifa-robot-3d.html)** | Interactive. Rotate, pull the explode slider, click any part for its dimensions and the rule that forces them. Includes the 30 cm inspection check and an animated play cycle for both halves. |
| **[Build brief](rifa-robot-design.html)** | The written spec: rules analysis, field geometry, match plan, card avoidance, inspection checklist. |

## The robot

Built on **mBot2** running gear — CyberPi, mBot2 Shield, two 180 Optical Encoder Motors and the Quad RGB sensor — on a deck cut for the job. The stock mBot2 chassis cannot be used: the ball has to run at mat level down the centreline, so the deck is a U-channel with a 60 mm slot, and the wheels move 8 mm outboard so the motor bodies clear it.

| Configuration | Measured | Limit |
|---|---|---|
| Scoring half, wings stowed | 29.4 × 24.7 × 11.9 cm | within 30 cm (inspection) |
| Preparation half, gathering | 31.3 × 31.9 × 11.9 cm | within 35 cm (in play) |
| Preparation half, released | 30.9 × 34.7 × 11.9 cm | within 35 cm (in play) |

Six motors, exactly at the cap: 2 drive · 1 flywheel · 3 servos (wings, feeder, hood).

### How one robot does both jobs

The collector and the shooter coexist because they work at **different heights** — blades at 27 mm, shooter above 50 mm. A fixed 27 mm front blade does the pushing in the preparation half and stops cones before they reach the hood, where they would tip. Two folding wings widen the capture and sweep back along the sides for the scoring half, hinged outboard of the drive wheels so their swept plane is clear of everything.

## What the field photos changed

Three assumptions in the original brief turned out to be wrong:

- **The dispenser has no button.** It is a flat lever at mat level, with a gravity magazine above and a round exit port. The ball leaves **rolling on the mat**, it does not drop — so the flywheel came down 47 mm to meet it and nothing has to lift the ball.
- **The port faces into your half**, not along the lane, with a T dock marking square in front of it. So the dock is perpendicular to the goal and one 90° turn each way is unavoidable.
- **The divider is no rail.** It spans only the middle of the table between the two dispensers and stops well short of the goal, so the run to the penalty line is unguided. Heading comes from the square dock plus the CyberPi gyro.

## Still to confirm

- Whether servos count toward the six-motor limit — at six of six there is no margin.
- Penalty-area dimensions, which are not stated numerically in the rulebook.
- Cone height and the dispenser lever's lateral offset from the ball port.
- The 180 encoder motor's body length. The slot clearance is about 4.5 mm per side; measure before cutting.

---

Dimensions in centimetres unless stated. Rule codes cite the RIFA World Cup Official Match Guide v1.2 (U13, §1.1 controller operation permitted). Figures marked as estimates are scaled from the Appendix A drawing and are not official.
