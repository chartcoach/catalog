---
id: scale-circle-size-by-area-not-radius
title: Scale circle size by area, not radius
bibliography: references.bib
description: For magnitude comparison, use area-proportional size encoding on circle-based
  charts to improve fidelity and mitigate exaggerated size differences for chart readers.
labels:
- purpose:refine
- basis:empirical
- task:compare
- data:quantitative
- quality:fidelity:use
- lever:encoding
- channel:area:use
- operator:difference
---

## Circle size mapping <!-- role: advice -->

Map quantitative values to circle area rather than to circle radius. For example, size a bubble so a doubled value doubles the visible area, not the radius, because radius mapping makes one value look much larger than another.

## Why area-proportional sizing matters <!-- role: reason -->

Readers compare the visible size of the circle, not the hidden geometry formula. When the value is mapped to radius, the displayed area grows exponentially, so the chart overstates the difference between values.

**Mechanism:** Area-proportional sizing keeps the visible mark size aligned with the data, while radius-based sizing inflates the larger mark and exaggerates the message.

**Evidence:** In the circle-size experiment, the deceptive size mapping led readers to judge the larger value as much bigger than in the area-proportional control (mean 2.71 vs. 1.71 on a 5-point scale; p = 0.0007) [@pandeyHowDeceptiveAre2015].

## Use when circle size carries the quantitative message <!-- role: context -->

- **User Goal:** Judge how much one value exceeds another from mark size.
- **Task:** Compare magnitude differences.
- **Data:** Quantitative values encoded by circle size.
- **Chart Setting:** A bubble-like display where circle size is the main quantitative cue.
- **Audience:** Readers relying on the visual size comparison instead of recalculating from labels.
- **Success Criterion:** The perceived size difference tracks the data difference instead of an inflated visual contrast.

## Do not apply this outside circle-size encodings <!-- role: exceptions -->

**Break it when:** The chart does not encode magnitude with circle size. **Why:** This guideline targets area-based marks where scaling the wrong geometric variable makes the visible size grow faster than the data.

## Costs of area-proportional sizing <!-- role: costs -->

**Sacrifice:** You give up some dramatic visual separation between values.
**Risk:** Moderate differences can look less forceful than in a radius-mapped version.
**Mitigation:** Keep the area-proportional sizing and accept the less dramatic appearance to preserve the data message.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Print the numeric value inside the circle but still size the mark by radius. **Why it fails:** The study showed that readers still formed exaggerated size judgments even when the chart displayed the actual values.

## How to review the size mapping <!-- role: check -->

**Failure Sign:** The larger circle looks disproportionately larger than the data ratio.
**Quick Check:** Inspect the sizing rule; if doubling the value doubles the radius instead of doubling the area, the chart uses the distortion tested here.
**Stronger Test:** Build an area-proportional version of the same chart and compare "how much bigger" judgments between the two versions.

## What to change <!-- role: fix -->

- Recalculate circle size from target area rather than radius.
- Redraw the circles so the area ratio matches the data ratio.
- Remove radius-based sizing rather than trying to correct it with printed values alone.
