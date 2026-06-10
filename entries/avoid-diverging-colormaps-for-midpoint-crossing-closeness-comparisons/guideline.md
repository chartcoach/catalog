---
id: avoid-diverging-colormaps-for-midpoint-crossing-closeness-comparisons
title: Avoid a diverging colormap when readers must compare values across the midpoint
bibliography: references.bib
description: For comparison tasks that judge closeness on ordered quantitative color
  scales, avoid a diverging colormap on scalar color encodings to improve fidelity
  and mitigate false grouping across the neutral midpoint for viewers reading relative
  distance.
labels:
- purpose:refine
- basis:empirical
- task:compare
- data:quantitative
- quality:fidelity
- lever:encoding
- operator:difference
- aesthetic:color:avoid
---

## Midpoint-crossing palette choice <!-- role: advice -->

Use a sequential ramp instead of a diverging ramp when readers must judge which of two values is closer and the compared values can fall on opposite sides of the midpoint. For example, replace a blue-orange diverging scale with a sequential ramp for closeness comparisons that cross the center; the diverging scale only matched sequential behavior when all compared values stayed on one half.

## Why midpoint crossing hurts <!-- role: reason -->

A diverging ramp invites grouping by side of the midpoint, so a numerically closer neutral or achromatic value can lose to a farther chromatic value on the same side.

**Mechanism:** When values straddle the midpoint, readers can treat the two chromatic sides as separate groups and misread which option is actually nearest to the reference.

**Evidence:** The tested blue-orange diverging scheme showed elevated errors specifically when comparisons crossed the central hue boundary, while comparisons confined to one half behaved like the underlying single-hue sequential scales [@liuSomewhereRainbowEmpirical2018].

**Notes:** Diverging colormaps are still appropriate when the intended meaning is distance from a neutral midpoint.

## When this applies <!-- role: context -->

- **User Goal:** Decide which value is closer or more similar.
- **Task:** Compare values that may lie on opposite sides of a central reference or zero point.
- **Data:** Ordered quantitative data encoded with a midpoint-centered color scale.
- **Chart Setting:** A continuous legend where readers must compare across both sides of the midpoint.
- **Audience:** Viewers reading relative distance directly from color.
- **Success Criterion:** Correct midpoint-crossing comparisons.

## When not to use it <!-- role: exceptions -->

**Break it when:** The main message is distance from a neutral midpoint or readers mostly compare values within one side of the scale. **Why:** Diverging scales are designed for midpoint-centered interpretation, and the study found within-half comparisons behaved like the corresponding sequential halves.

## Costs of avoiding the diverging ramp <!-- role: costs -->

**Sacrifice:** You lose the explicit visual emphasis of a neutral center.
**Risk:** A sequential replacement can weaken the sense of deviation around a reference point.
**Mitigation:** Keep the diverging scale only when midpoint meaning matters more than cross-midpoint closeness judgments.

## Common mistake with diverging ramps <!-- role: mistakes -->

**Mistake:** Assuming the midpoint-side option will still read as closest when its color is neutral and the farther option shares the reference hue family. **Why it fails:** Readers can group the chromatic colors together and miss that the achromatic option is numerically closer.

## How to check it <!-- role: check -->

**Failure Sign:** Readers miss obvious closeness relationships when one comparison color falls on the opposite side of the midpoint.
**Quick Check:** Test a few representative triplets that cross the midpoint and ask which option is closer to the reference.
**Stronger Test:** Compare the same chart with the current diverging ramp and a sequential ramp on midpoint-crossing comparisons and keep the version with fewer errors.

## What to change <!-- role: fix -->

- Replace the diverging colormap with a sequential colormap when cross-midpoint closeness is the main task.
- Keep the diverging colormap only if the chart is primarily about distance from the midpoint.
- Re-test representative midpoint-crossing comparisons after the palette change.
