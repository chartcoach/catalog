---
id: use-a-diverging-palette-when-values-deviate-from-a-baseline
title: Use a diverging palette when values deviate from a baseline
bibliography: references.bib
description: For baseline comparison in quantitative charts, use a diverging color
  gradient on the value encoding to improve insight and mitigate weak separation between
  below-baseline and above-baseline values for readers.
labels:
- purpose:refine
- basis:heuristic
- data:quantitative
- quality:insight
- lever:encoding
- operator:difference
- channel:color-hue:use
- aesthetic:color:use
---

## Diverging gradient <!-- role: advice -->

Use a diverging color gradient when the message is how values differ from a baseline. For example, map below-baseline and above-baseline values to clearly different hues and place a light gray center at the baseline instead of white.

## Why diverging palettes sharpen baseline reading <!-- role: reason -->

When the main question is which side of a baseline a value falls on, a single sequential scale hides that split.

**Mechanism:** Two distinct hue directions make below-baseline and above-baseline values immediately separable, and a neutral center marks the baseline itself.

**Evidence:** The post recommends diverging palettes when the goal is to emphasize how a variable diverts from a baseline, says both sides should use clearly distinguishable hues, and says the center color should ideally be light gray rather than white [@muth_colors_2018].

## When to use a diverging palette <!-- role: context -->

- **User Goal:** See whether values are below or above a reference point.
- **Data:** Quantitative values are compared against a meaningful baseline.
- **Chart Setting:** Color carries the direction and amount of deviation.
- **Success Criterion:** Readers can tell both magnitude and side of the baseline quickly.

## When not to use a diverging palette <!-- role: exceptions -->

**Break it when:** There is no meaningful baseline and the message is only low-to-high magnitude. **Why:** Diverging palettes are for deviation from a reference point.

## Tradeoffs of diverging palettes <!-- role: costs -->

**Sacrifice:** The scale becomes more complex than a single sequential gradient.
**Risk:** An arbitrary midpoint can suggest a meaning the data does not support.
**Mitigation:** Use a diverging palette only when the baseline is genuinely important to the message.

## Common diverging-palette mistake <!-- role: mistakes -->

**Mistake:** Using similar hues on both sides of the baseline or centering the palette on white. **Why it fails:** The split around the baseline becomes harder to read.

## How to check a diverging palette <!-- role: check -->

**Failure Sign:** The midpoint color does not clearly mark the baseline or the two sides look too similar.
**Quick Check:** Verify that the legend midpoint matches the baseline value.
**Stronger Test:** Check whether a reader can tell from color alone which values are above and below the baseline.

## How to fix a weak diverging palette <!-- role: fix -->

- Switch from a sequential scale to a diverging scale.
- Use clearly distinguishable hues on the two sides of the midpoint.
- Replace a white midpoint with a light gray midpoint at the baseline.
