---
id: use-darker-more-opaque-colors-for-higher-values-on-light-backgrounds
title: Use darker more opaque-looking colors for larger quantities on light backgrounds
  when the colormap appears to vary in opacity
bibliography: references.bib
description: For quantitative comparison on light-background colormaps, use dark-more
  scale order on color scales that appear to vary in opacity to improve reading speed
  and mitigate high-end misreading for viewers interpreting magnitude from color.
labels:
- purpose:refine
- basis:empirical
- quality:readability:use
- lever:scale-order
- channel:opacity:use
- channel:color-lightness:use
---

## Align high values with the dark opaque end <!-- role: advice -->

Assign larger quantities to the darker, more opaque-looking end of the scale when a light background makes the colormap look like a color fading in from that background. For example, on a white background, keep the most background-contrasting dark endpoint at the high-value end for grayscale or other background-interpolated colormaps.

## Why dark-more works on light opacity-varying backgrounds <!-- role: reason -->

On a light background, the darker end is also the more opaque-looking end. Dark-is-more and opaque-is-more point to the same high end, so the mapping is especially easy to read.

**Mechanism:** When the dark endpoint also appears most opaque, readers do not have to resolve a conflict between lightness and opacity cues.

**Evidence:** For colormaps that appeared to vary in opacity, participants were faster with dark-more encoding on light backgrounds, where the darker colors were also the more opaque-looking colors. [@schlossMappingColorMeaning2019]

## Use when the light background creates opacity steps <!-- role: context -->

- **User Goal:** Judge which areas represent larger quantities from a colormap and legend.
- **Data:** Quantitative values encoded with a sequential colormap.
- **Chart Setting:** A light background is fixed, and the scale looks like a high-contrast endpoint interpolated with that background.
- **Audience:** Viewers reading magnitude from color with the help of a legend.
- **Success Criterion:** Faster interpretation of the larger-value end of the scale.

## Do not use when the scale does not look translucent <!-- role: exceptions -->

**Break it when:** The light background does not make the scale appear to vary in opacity. **Why:** Then the opacity cue that supports this specific rule is absent, and the more general dark-is-more rule should be applied without treating opacity as causal.

## Tradeoffs of using the dark opaque end as high <!-- role: costs -->

**Sacrifice:** This mapping is less portable to dark backgrounds.
**Risk:** Reusing the same opacity-varying scale on a dark background can make the other end look more opaque.
**Mitigation:** Keep the background fixed when you design around opacity cues.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Mapping larger quantities to the lighter end on a light background when the scale looks like it fades in from that background. **Why it fails:** The lighter end looks less opaque and conflicts with both dark-is-more and opaque-is-more.

## How to test the mapping <!-- role: check -->

**Failure Sign:** On a light background, the chart feels slower to read when the lighter end is labeled as larger.
**Quick Check:** If the scale looks like one color gradually appearing over the light background, assign the high end to the darkest most opaque-looking endpoint.
**Stronger Test:** Compare dark-more and light-more versions on the same light background and keep the faster-read version.

## What to change <!-- role: fix -->

- Put the light background-matching endpoint at the low end of the legend.
- Assign the most background-contrasting dark endpoint to the high end of the legend.
- Keep the background fixed if the design depends on the scale reading as opacity variation.
