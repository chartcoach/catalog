---
id: avoid-opacity-varying-colormaps-when-backgrounds-may-change
title: Avoid colormaps that appear to vary in opacity when the background may change
bibliography: references.bib
description: For quantitative comparison across changing presentation backgrounds,
  avoid opacity-varying color scales on colormap visualizations to improve reading
  robustness and mitigate background-dependent reversals for viewers interpreting
  magnitude from color.
labels:
- purpose:refine
- basis:empirical
- quality:readability:use
- lever:encoding
- channel:opacity:avoid
- channel:color-lightness:use
---

## Choose a background-robust color scale <!-- role: advice -->

Avoid color scales that look like a single color interpolated with the background when the same colormap may be shown on different backgrounds. For example, replace grayscale or other background-interpolated scales with scales that curve through color space so they do not read as opacity variation, then keep the darker end mapped to larger quantities.

## Why opacity-varying scales are not robust across backgrounds <!-- role: reason -->

The perceived opaque end of the scale changes with the background. A mapping that feels natural on one background can become slower or less intuitive on another if the scale starts to look translucent.

**Mechanism:** Removing the opacity cue prevents the background from changing the inferred high end of the scale, so the dark-is-more mapping stays stable.

**Evidence:** The paper concludes that background only matters when the colormap appears to vary in opacity, and recommends using scales that do not appear to vary in opacity on any background when the design must remain robust across background changes. [@schlossMappingColorMeaning2019]

## Use when the same colormap may travel across backgrounds <!-- role: context -->

- **User Goal:** Keep one colormap easy to interpret in more than one presentation setting.
- **Data:** Quantitative values encoded with a sequential colormap.
- **Chart Setting:** The same chart or palette may appear on both light and dark backgrounds, such as in different slide or display themes.
- **Audience:** Viewers who must rely on the chart's legend and color ordering rather than on prior exposure.
- **Success Criterion:** Stable interpretation of the high end of the scale across backgrounds.

## Do not use when a fixed background is part of the design <!-- role: exceptions -->

**Break it when:** The background is fixed and intentionally used to create an opacity-varying colormap. **Why:** Then matching larger quantities to the more opaque-looking end on that one background can improve reading, even though the mapping will not transfer cleanly to another background.

## Tradeoffs of avoiding opacity variation <!-- role: costs -->

**Sacrifice:** You give up the chance to exploit an opacity cue on one specific fixed background.
**Risk:** A scale chosen only for background robustness may feel less tailored to a single themed presentation.
**Mitigation:** If robustness is the goal, prioritize a scale that does not read as fading into any intended background.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Reusing the same background-interpolated scale on both white and black backgrounds without changing the scale design. **Why it fails:** The apparent opaque end changes with the background, so the preferred mapping changes too.

## How to test the scale choice <!-- role: check -->

**Failure Sign:** The same colormap feels intuitive on one background but not on another.
**Quick Check:** Preview the scale on each intended background and look for cases where the colors resemble a single foreground color fading into that background.
**Stronger Test:** If the intuitive high end flips across backgrounds, replace the scale rather than only flipping the legend.

## What to change <!-- role: fix -->

- Replace a background-interpolated scale with one whose colors curve through color space instead of following a straight interpolation to the background.
- After replacing the scale, keep larger quantities at the darker end.
- Preview the revised scale on every intended background and remove any version that starts to look like opacity variation.
