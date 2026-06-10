---
id: use-diverging-colormap-with-meaningful-midpoint
title: Use a diverging colormap when values have a meaningful midpoint
bibliography: references.bib
description: For ordered or continuous value comparison around a meaningful midpoint,
  use diverging color encoding on color-mapped charts to improve fidelity and mitigate
  weak baseline comparison for readers interpreting deviation from a reference value.
labels:
- purpose:refine
- basis:empirical
- data:ordinal
- data:quantitative
- quality:fidelity
- lever:encoding
- aesthetic:color:use
---

## Midpoint color scale <!-- role: advice -->

Use a diverging colormap when color encodes ordered values around a meaningful middle point. For example, when values show difference from a baseline or a natural zero, map the midpoint to a neutral middle color and let colors diverge continuously on both sides.

## Why midpoint color needs a split <!-- role: reason -->

A midpoint task is not only about magnitude. Readers must also see which values fall on each side of a reference and how far away they are.

**Mechanism:** A diverging scale makes the center value visually explicit and supports direct comparison to that reference point. This reduces ambiguity that occurs when all values are placed on one continuous scale with no visible middle.

**Evidence:** The paper recommends diverging colormaps for ordered or continuous data when there is a meaningful middle point, such as differences from a baseline or a natural zero value, because they support comparisons to that middle point [@szafirGoodBadBiased2018].

## Use when deviation from a reference matters <!-- role: context -->

- **User Goal:** Judge whether values are above, below, or near a reference.
- **Task:** Compare magnitude relative to a midpoint.
- **Data:** Ordered or continuous values with a meaningful center such as a baseline or natural zero.
- **Chart Setting:** A chart uses color as the main value encoding.
- **Audience:** Readers must compare values to the middle point quickly and accurately.
- **Success Criterion:** The center value is visually obvious and both sides of the scale are easy to distinguish.

## Do not use when there is no meaningful center <!-- role: exceptions -->

- **Break it when:** The data has no meaningful midpoint. **Why:** The source recommends a sequential colormap for pure low-to-high magnitude reading.
- **Break it when:** The data is categorical. **Why:** The task is no longer ordered comparison around a center.

## What you trade away <!-- role: costs -->

**Sacrifice:** You give up a single uninterrupted low-to-high ramp.
**Risk:** If the midpoint is arbitrary or unimportant, the split can imply a distinction that the analysis does not need.
**Mitigation:** Use a sequential scale when the task is simple magnitude reading rather than deviation from a reference.

## Common midpoint failure <!-- role: mistakes -->

**Mistake:** Using a sequential or rainbow scale when the main task is comparison to a baseline. **Why it fails:** Readers do not get a clear visual center, so above-versus-below comparisons become less direct.

## How to review the midpoint mapping <!-- role: check -->

**Failure Sign:** Readers can see low and high values, but not the reference split.
**Quick Check:** Inspect the scale and verify that the midpoint is mapped to a neutral middle color.
**Stronger Test:** Ask whether a reader can identify values on either side of the baseline without reading the legend closely.

## What to change <!-- role: fix -->

- Set the meaningful midpoint to the center of the colormap.
- Use a neutral middle color at that midpoint.
- Use continuous color ramps that diverge on both sides of the center.
- Replace the diverging scale with a sequential one if no real midpoint exists.
