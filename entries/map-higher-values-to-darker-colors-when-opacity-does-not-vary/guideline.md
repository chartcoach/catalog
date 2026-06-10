---
id: map-higher-values-to-darker-colors-when-opacity-does-not-vary
title: Map larger quantities to darker colors when the colormap does not appear to
  vary in opacity
bibliography: references.bib
description: For quantitative comparison in colormap reading, use dark-more scale
  order on sequential colormap encodings that do not appear to vary in opacity to
  improve reading speed and mitigate background-driven misinterpretation for viewers
  interpreting magnitude from color.
labels:
- purpose:refine
- basis:empirical
- quality:readability:use
- lever:scale-order
- channel:color-lightness:use
- component:legend:use
---

## Set the legend to dark-more <!-- role: advice -->

Assign larger quantities to the darker end of the color scale when the colormap does not look like a foreground color fading into the background. For example, keep the darker end of a sequential heatmap or choropleth legend at the high-value end even on a dark background if the scale itself does not visibly suggest opacity steps.

## Why dark-more works here <!-- role: reason -->

Readers form an inferred mapping before or while reading the legend. When the scale does not suggest opacity variation, that inferred mapping is dominated by dark-is-more, so a dark-more legend is read faster.

**Mechanism:** Matching the legend order to the dark-is-more bias reduces the extra interpretation step needed to reconcile the legend with the colors in the chart.

**Evidence:** Across sequential colormaps that did not appear to vary in opacity, participants responded faster when darker colors encoded larger quantities, and this pattern held regardless of background for scales without apparent opacity variation. [@schlossMappingColorMeaning2019]

## Use when dark-is-more should dominate <!-- role: context -->

- **User Goal:** Identify which region, cell, or side contains larger quantities.
- **Data:** Quantitative values encoded with a sequential colormap.
- **Chart Setting:** The color scale does not look like a single reference color interpolated with the background; the legend explicitly maps color to magnitude.
- **Audience:** Viewers who must interpret quantity from color rather than from direct labels.
- **Success Criterion:** Faster, easier legend-based interpretation of which areas represent more.

## Do not use when opacity cues are visible <!-- role: exceptions -->

**Break it when:** The color scale visibly looks like one foreground color fading into the background, so parts of the colormap appear more or less opaque. **Why:** Then an opaque-is-more bias affects interpretation, and dark-more is no longer the only supported mapping.

## Tradeoffs of dark-more ordering <!-- role: costs -->

**Sacrifice:** You give up lighter-high encodings on scales that truly read as opacity variation.
**Risk:** If you treat an opacity-varying scale as non-opacity-varying, dark-more can conflict with the perceived opaque end.
**Mitigation:** Check whether the scale looks like interpolation with the background before fixing the high end to dark.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Reversing the scale to light-more just because the background is dark. **Why it fails:** A dark background alone did not justify light-more encoding when the scale did not appear to vary in opacity.

## How to test the mapping <!-- role: check -->

**Failure Sign:** Readers hesitate or make more effort when the legend says the lighter end is larger.
**Quick Check:** View the scale against the actual background; if the intermediate colors do not resemble opacity steps from a single reference color, treat it as non-opacity-varying.
**Stronger Test:** Compare dark-more and light-more versions of the same chart and keep the version that is interpreted faster.

## What to change <!-- role: fix -->

- Reverse the legend so the darker endpoint corresponds to the larger quantity.
- Keep the background, but replace the scale with one that does not read as a straight interpolation from a high-contrast endpoint to that background.
- If you need the mapping to stay stable across backgrounds, choose a scale whose path curves through color space rather than one that reads as fading into the background.
