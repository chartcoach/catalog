---
id: replace-rainbow-colormaps-with-perceptually-ordered-ramps
title: Replace rainbow colormaps with a perceptually ordered quantitative ramp
bibliography: references.bib
description: For comparison tasks on quantitative color scales, avoid rainbow colormaps
  on scalar color encodings to prevent slow and error-prone value reading and address
  misleading similarity judgments for viewers comparing relative differences.
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

## Rainbow ramp replacement <!-- role: advice -->

Replace a rainbow colormap with a perceptually ordered quantitative ramp when color encodes ordered magnitude. For example, swap jet for viridis on a continuous heatmap legend; the tested sequential and perceptually uniform multi-hue ramps both outperformed jet overall.

## Why the rainbow ramp fails <!-- role: reason -->

A rainbow ramp changes hue in ways that do not consistently support ordered distance, so readers spend longer judging similarity and make more mistakes across the scale.

**Mechanism:** When hue boundaries and perceptual spacing do not align with numeric spacing, nearby values can look farther apart than larger value differences, which slows comparison and increases error.

**Evidence:** Jet was the slowest and most error-prone colormap tested overall, and the paper concludes that it should be jettisoned for quantitative color encoding despite one narrow high-performing region created by lucky color-name boundaries [@liuSomewhereRainbowEmpirical2018].

**Notes:** The one strong pocket for jet occurred where color-name boundaries happened to line up with the value grouping.

## When this applies <!-- role: context -->

- **User Goal:** Compare ordered values or gradients by color.
- **Task:** Judge which value is closer, more similar, or farther apart on a quantitative scale.
- **Data:** Ordered quantitative values encoded with a continuous color ramp.
- **Chart Setting:** A chart with a color legend where readers interpret the ramp as ordered magnitude.
- **Audience:** Viewers reading relative differences directly from color.
- **Success Criterion:** Faster and more accurate comparison across the full scale.

## When not to use it <!-- role: exceptions -->

**Break it when:** The encoding is intentionally discrete and relies on category-like color-name boundaries instead of a continuous ordered scale. **Why:** The only strong-performing jet cases were driven by categorical color-name transitions, not by reliable continuous quantitative reading.

## Costs of replacing the rainbow ramp <!-- role: costs -->

**Sacrifice:** You lose the vivid spectral look that often motivates rainbow use.
**Risk:** Replacing jet with an arbitrary non-rainbow ramp can still leave comparison problems.
**Mitigation:** Prefer a perceptually ordered ramp, especially a perceptually uniform multi-hue ramp, rather than any multi-hue palette.

## Common mistake with rainbow replacement <!-- role: mistakes -->

**Mistake:** Replacing jet with another multi-hue ramp that still lacks clear perceptual ordering. **Why it fails:** Multiple hues alone did not guarantee good performance; the tested multi-hue ramps worked when they were judiciously designed.

## How to check it <!-- role: check -->

**Failure Sign:** Comparisons slow down or become inconsistent around hue transitions.
**Quick Check:** Sample low, mid, and high reference colors from the ramp and test a few triplets around major hue changes.
**Stronger Test:** Compare the same chart in jet and in a perceptually ordered ramp such as viridis and keep the version that yields faster and more accurate similarity judgments.

## What to change <!-- role: fix -->

- Replace jet with a perceptually ordered ramp such as viridis.
- Re-test comparisons near major hue transitions after the swap.
- If the chart only needs a few discrete bins, simplify to a small sequential scale instead of using a rainbow ramp.
