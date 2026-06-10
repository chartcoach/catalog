---
id: use-sequential-colormap-without-midpoint
title: Use a sequential colormap when values have no meaningful midpoint
bibliography: references.bib
description: For ordered or continuous value comparison without a meaningful midpoint,
  use sequential color encoding on color-mapped charts to improve fidelity and mitigate
  false pattern detection for readers including those with color-vision deficiency.
labels:
- purpose:refine
- basis:empirical
- data:ordinal
- data:quantitative
- quality:fidelity
- lever:encoding
- aesthetic:color:use
- needs:color-vision-deficiency
---

## Color scale choice <!-- role: advice -->

Use a sequential colormap when color encodes ordered values and the data has no meaningful middle point. For example, in a heatmap, choropleth, or scalar-field view, map low-to-high values with one ordered scale instead of a rainbow palette.

## Why ordered color works better here <!-- role: reason -->

Ordered color scales keep visual differences aligned with data differences. Rainbow palettes change unevenly across hue, create artificial bands, and make smoothly varying data look grouped into named colors.

**Mechanism:** A sequential scale preserves relative magnitude, so nearby values look nearby and larger value changes look larger. This reduces false grouping and makes low-to-high structure easier to read, including for some readers who cannot distinguish all rainbow hues.

**Evidence:** The paper reports that rainbow colormaps distort perceived value relationships, create false divisions in smoothly varying data, and become less accessible for colorblind readers; it recommends sequential colormaps for ordered or continuous data without a meaningful midpoint [@szafirGoodBadBiased2018].

## Use when ordered color is the message <!-- role: context -->

- **User Goal:** Compare magnitude, locate highs and lows, or read smooth variation.
- **Task:** Compare ordered values from low to high.
- **Data:** Ordered or continuous values without a natural center value that readers must compare against.
- **Chart Setting:** A chart uses color as the main value encoding.
- **Audience:** Readers must interpret value differences at a glance, including some with color-vision deficiency.
- **Success Criterion:** Equal-looking color steps correspond more closely to equal data steps, without false bands.

## Do not use when a center value matters or values are categorical <!-- role: exceptions -->

- **Break it when:** The data has a meaningful midpoint such as a baseline or natural zero. **Why:** The source recommends a diverging colormap for direct comparison to that middle point.
- **Break it when:** The data is categorical. **Why:** The source notes that hue-based grouping can be useful for categories rather than ordered magnitudes.

## What you trade away <!-- role: costs -->

**Sacrifice:** You give up strong emphasis on above-versus-below a central reference value.
**Risk:** If a meaningful midpoint does exist, a purely sequential scale makes comparison to that midpoint less direct.
**Mitigation:** Switch to a diverging scale when the midpoint is part of the task.

## Common palette failure <!-- role: mistakes -->

**Mistake:** Using a rainbow palette for smoothly varying values. **Why it fails:** Readers see artificial blue, green, yellow, and red bands, and equal numeric differences no longer look equal.

## How to review the palette <!-- role: check -->

**Failure Sign:** Smooth data looks split into named-color regions or abrupt boundaries.
**Quick Check:** Scan the scale and ask whether some hue transitions look much stronger than others for similar value steps.
**Stronger Test:** Compare the same chart with a sequential scale; if apparent clusters or boundaries disappear, the original palette was distorting the data.

## What to change <!-- role: fix -->

- Replace the rainbow palette with a sequential colormap.
- Make the color progression visually ordered from low to high.
- Reserve categorical hue sets for categorical data.
- Switch to a diverging colormap if the task depends on a meaningful middle value.
