---
id: avoid-very-dark-colormap-regions-on-white-backgrounds
title: Avoid very dark colormap regions on white backgrounds
bibliography: references.bib
description: For comparison tasks on quantitative color scales, avoid very low-luminance
  colors on white-background charts to improve fidelity and mitigate misjudgment of
  dark shades for viewers comparing nearby values.
labels:
- purpose:refine
- basis:empirical
- task:compare
- data:quantitative
- quality:fidelity
- lever:encoding
- channel:color-lightness:avoid
- aesthetic:color:avoid
---

## Dark-end palette control <!-- role: advice -->

Avoid very dark low-end colors when a quantitative colormap is shown on a white background. For example, lighten or remove the black end of greys, magma, or plasma on a white heatmap or legend; those dark tails produced large error spikes.

## Why the dark end fails on white <!-- role: reason -->

Very dark colors on white can look more separated from the background than from each other, so readers struggle to judge which dark shade is closer to a reference.

**Mechanism:** High contrast against white interferes with discrimination among nearby dark shades, especially near the low end of the scale.

**Evidence:** The study found dramatic error increases in the dark regions of greys, magma, and plasma on a white background, and these failures were much worse than predicted by LAB or UCS color-distance models [@liuSomewhereRainbowEmpirical2018].

**Notes:** The paper warns that an analogous problem may also occur for very light colors on dark backgrounds, but that case was not tested.

## When this applies <!-- role: context -->

- **User Goal:** Compare nearby low values accurately.
- **Task:** Judge relative distance between dark shades on a quantitative scale.
- **Data:** Ordered quantitative values encoded with a continuous colormap.
- **Chart Setting:** A white or high-luminance background with the dark end of the palette visible.
- **Audience:** Viewers reading the low end of the scale directly.
- **Success Criterion:** Accurate low-end comparisons rather than visual drama at the darkest values.

## When not to use it <!-- role: exceptions -->

**Break it when:** The chart is not shown on a white or other high-luminance background. **Why:** The measured degradation was tied to dark colors set against white, and the paper does not claim the same magnitude of failure for other backgrounds.

## Costs of avoiding the dark end <!-- role: costs -->

**Sacrifice:** You give up the dramatic black endpoint used by some palettes.
**Risk:** Keeping the black endpoint for style can make nearby low values hard to compare.
**Mitigation:** Start the ramp above black or choose a palette whose low end is not extremely dark when the background stays white.

## Common mistake with dark colors on white <!-- role: mistakes -->

**Mistake:** Trusting perceptual color-distance numbers alone for the darkest colors on a white background. **Why it fails:** The study found much worse discrimination there than the color models predicted.

## How to check it <!-- role: check -->

**Failure Sign:** The darkest two or three steps of the scale look hard to order on the actual white chart.
**Quick Check:** Inspect nearby low-end values on the chart background, not only in a palette editor.
**Stronger Test:** Compare a dark-end palette with a lighter-start alternative on the same white chart and keep the version with fewer low-end errors.

## What to change <!-- role: fix -->

- Remove or lighten the darkest endpoint of the colormap.
- Switch to a palette whose low end does not collapse into near-black on white.
- If the dark palette must stay, change the chart background so the low end is not shown against white.
