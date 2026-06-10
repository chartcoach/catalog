---
id: use-a-moderate-number-of-sample-paths-in-static-ensemble-path-displays
title: Use a moderate number of sample paths in static ensemble path displays
bibliography: references.bib
description: For point-location judgments in static uncertainty forecasts, prefer
  a moderate number of visible sample paths on ensemble path maps to improve fidelity
  and mitigate overweighting of a single overlapping path for novice viewers.
labels:
- purpose:refine
- basis:empirical
- chart:map
- data:geospatial
- quality:fidelity
- lever:encoding
- operator:uncertainty
- literacy:novice
---

## Increase displayed path count <!-- role: advice -->

Increase the number of visible sample paths until a single path overlap has less influence on location judgments, but stop before the display looks exhaustive. For example, displays with 17–33 visible paths produced less overlap bias than a 9-path display, while a denser 65-path display performed worse than 17–33 because viewers were more likely to read it as showing all possible paths.

## Why moderate path counts work <!-- role: reason -->

A sparse ensemble path display makes each visible line look more meaningful than it should. Adding more sample paths makes the display read more like a distribution and less like a set of individually decisive routes, but pushing density too high can make the display seem exhaustive.

**Mechanism:** Moderate path counts shift attention from any one visible line toward the overall distribution of paths, which reduces the tendency to overestimate risk when a location happens to sit on a displayed line.

**Evidence:** In static hurricane ensemble maps, the difference between judgments for points on a displayed line versus equally distant points off a displayed line was smaller with 17 and 33 paths than with 9 paths. A 65-path display still reduced the bias relative to 9 paths, but performed worse than 17 and 33 paths, and more viewers treated it as showing all possible paths [@padillaPowerfulInfluenceMarks2020].

**Notes:** The best-performing count in these stimuli was about 30 paths, but the paper notes that the practical maximum can vary with spread, line thickness, and other display parameters.

## Use when all are true <!-- role: context -->

- **User Goal:** Judge how much risk or damage a specific location faces.
- **Task:** Read uncertainty from a static path ensemble rather than from an animation.
- **Data:** Geospatial path uncertainty shown as multiple sampled lines.
- **Chart Setting:** A single-image forecast display where viewers can see individual paths.
- **Audience:** Novice or non-expert viewers with little prior instruction.
- **Success Criterion:** Smaller judgment differences between equal-distance locations that differ only by touching a displayed line.

## Do not use when any are true <!-- role: exceptions -->

**Break it when:** The added path count makes the display look like the full set of possible outcomes or makes gaps in the distribution newly salient. **Why:** Very dense displays can restore misinterpretation by making viewers think the map shows all possible paths.

## Tradeoffs of increasing path count <!-- role: costs -->

**Sacrifice:** Individual paths become less separable as the display gets denser.\
**Risk:** If density is pushed too far, viewers may infer that the display is exhaustive rather than sampled.\
**Mitigation:** Increase path count from sparse to moderate, then stop short of a display that reads as the full set of outcomes.

## Common failure modes <!-- role: mistakes -->

- **Mistake:** Leaving only a sparse handful of visible sample paths. **Why it fails:** Viewers give too much weight to whether one displayed line touches the location.
- **Mistake:** Continuing to add paths until the map looks full. **Why it fails:** Viewers become more likely to think the display shows all possible paths.

## How to test it <!-- role: check -->

**Failure Sign:** A location on a displayed line is judged much riskier than an equally distant location off the line.\
**Quick Check:** Create matched probe views where the target location stays at the same distance from the bundle center and only line overlap changes.\
**Stronger Test:** Compare the on-line minus off-line judgment gap across candidate path counts and keep the count with the smaller gap.

## What to change <!-- role: fix -->

- Increase a very sparse path display to a moderate count of visible sample paths.
- Re-test the display with matched on-line and off-line probe locations after the change.
- If the display now looks exhaustive, remove paths until viewers no longer read it as showing all possible outcomes.
