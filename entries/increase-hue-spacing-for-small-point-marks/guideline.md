---
id: increase-hue-spacing-for-small-point-marks
title: Increase hue spacing for small point marks
bibliography: references.bib
description: For color-difference reading in static charts, use wider hue spacing
  on scatter plots with small point marks to improve fidelity and mitigate missed
  color differences for viewers reading web-based visualizations.
labels:
- purpose:refine
- basis:empirical
- chart:scatter
- quality:fidelity:use
- lever:encoding
- channel:color-hue:use
- aesthetic:color:use
---

## Adjust hue spacing for small points <!-- role: advice -->

Increase hue spacing when scatterplot points get small. For example, widen the distance between neighboring point colors, push endpoint colors farther apart for smaller points, or increase point diameter before reusing a palette designed for larger marks.

## Why small points need more hue separation <!-- role: reason -->

Small point marks contribute less visible colored area, so nearby hues are harder to tell apart in a visually busy scatterplot than on large isolated swatches. Widening hue spacing or enlarging the points preserves visible color differences at the size viewers actually see.

**Mechanism:** Smaller point diameter lowers color discriminability, so palettes that look distinct on large patches can collapse on plotted points.

**Evidence:** The knowledge collation records this source as experimental evidence about color-hue encodings on point marks, and the paper reports that perceived color difference for scatterplot points decreases as point diameter shrinks and is worse than isolated-mark predictions under visualization-like conditions [@zengReviewCollationGraphical2023; @szafirModelingColorDifference2018].

**Notes:** The source frames this as a size-aware refinement to an already chosen color encoding, not as a new chart-family choice.

## Use when small points are the limiting case <!-- role: context -->

- **User Goal:** Distinguish differently colored point marks reliably.
- **Data:** Color is already assigned to point marks, and the smallest plotted points are materially smaller than large swatches or legend chips.
- **Chart Setting:** Static scatterplots or other point-based views on standard web or desktop displays.
- **Audience:** Viewers reading the rendered chart rather than inspecting the palette in isolation.
- **Success Criterion:** Neighboring encoded colors remain distinguishable on the smallest plotted points.

## Do not use as the only rule when contrast dominates <!-- role: exceptions -->

**Break it when:** Many adjacent marks are also colored or simultaneous contrast is a central part of the display. **Why:** The experiment used two colored test marks with gray distractors, so the model does not fully cover contrast-heavy conditions.

## Tradeoffs of widening point colors <!-- role: costs -->

**Sacrifice:** Wider hue spacing reduces how many discriminable color steps fit into the same palette range.
**Risk:** Applying large color gaps everywhere can be overly conservative when point marks are not actually small.
**Mitigation:** Base the spacing on the smallest allowable point size instead of the average size.

## Common failure with small point colors <!-- role: mistakes -->

**Mistake:** Reusing a palette chosen on large swatches or larger marks for very small scatterplot points. **Why it fails:** The palette can look separated in isolation while collapsing once the colors are drawn on small plotted points.

## Check the smallest plotted points <!-- role: check -->

**Failure Sign:** Different categories or values look like the same color on the smallest visible points.
**Quick Check:** Inspect the smallest plotted points, not just the legend or a large preview swatch.
**Stronger Test:** Compute a minimum discriminability threshold from the smallest allowable point diameter and verify that neighboring colors still exceed it.

## Fix the point-color collision <!-- role: fix -->

- Increase the distance between neighboring point colors.
- Push the endpoint colors farther apart when point size decreases.
- Increase point diameter if the palette cannot be widened enough.
- Adapt the number of color bins or the color range to the smallest plotted point size before finalizing the chart.
