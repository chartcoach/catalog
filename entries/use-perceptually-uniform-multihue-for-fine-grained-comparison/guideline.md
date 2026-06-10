---
id: use-perceptually-uniform-multihue-for-fine-grained-comparison
title: Use a perceptually uniform multi-hue colormap for fine-grained quantitative
  comparison
bibliography: references.bib
description: For comparison tasks on continuous quantitative color scales, prefer
  a perceptually uniform multi-hue colormap on scalar color encodings to improve fidelity
  and mitigate missed small value differences for viewers judging relative similarity.
labels:
- purpose:refine
- basis:empirical
- task:compare
- data:quantitative
- quality:fidelity
- lever:encoding
- operator:difference
- aesthetic:color:use
---

## Multi-hue ramp choice <!-- role: advice -->

Use a perceptually uniform multi-hue colormap when readers must distinguish nearby values on a continuous quantitative scale. For example, replace a single-hue blues ramp with viridis on a heatmap or scalar field when small span differences matter; viridis stayed accurate where single-hue ramps lost resolution.

## Why the multi-hue ramp works <!-- role: reason -->

A multi-hue ramp can separate nearby values more clearly than a single-hue ramp because hue and luminance both change while the scale still preserves order.

**Mechanism:** Adding hue variation to a luminance ramp increases separation between nearby values, so readers make fewer mistakes when judging which value is closest to a reference.

**Evidence:** Viridis was among the fastest and most accurate tested colormaps, and single-hue ramps showed a clear error increase at the smallest spans where nearby values had to be distinguished; across studies, the perceptually uniform multi-hue ramps had the lowest error overall [@liuSomewhereRainbowEmpirical2018].

**Notes:** Single-hue ramps remained competitive when value differences were larger.

## When this applies <!-- role: context -->

- **User Goal:** Compare which values are closest or most similar.
- **Task:** Judge relative distance between nearby values on an ordered color scale.
- **Data:** Ordered quantitative values encoded by a continuous color scale.
- **Chart Setting:** A scalar field or other view with a continuous legend where local differences matter.
- **Audience:** Viewers reading the color scale directly.
- **Success Criterion:** Low error on near-value comparisons without slowing readers.

## When not to use it <!-- role: exceptions -->

**Break it when:** The scale is discretized to only a few bins and the task does not depend on distinguishing very small value differences. **Why:** The paper notes that single-hue colormaps may still be acceptable for discrete scales with about 5–7 colors, and the tested single-hue ramps performed well at larger spans.

## Costs of the multi-hue ramp <!-- role: costs -->

**Sacrifice:** You give up the visual simplicity of a single-hue ramp.
**Risk:** A multi-hue ramp that is not judiciously designed can still read poorly.
**Mitigation:** Use a perceptually uniform multi-hue ramp that also ramps in luminance, as in viridis.

## Common mistake with the multi-hue decision <!-- role: mistakes -->

**Mistake:** Keeping a single-hue ramp after increasing the number of bins or asking readers to separate nearby values. **Why it fails:** The tested single-hue ramps showed a strong resolution drop at the smallest spans.

## How to check it <!-- role: check -->

**Failure Sign:** Adjacent colors look different enough, but deciding which of two nearby values is closer to a reference still feels uncertain.
**Quick Check:** Sample three nearby values from the scale and ask which comparison color is closer to the reference.
**Stronger Test:** Compare the same chart with the current single-hue ramp and a perceptually uniform multi-hue ramp on low-span comparisons and keep the version with fewer errors.

## What to change <!-- role: fix -->

- Replace the single-hue ramp with a perceptually uniform multi-hue ramp such as viridis.
- Preserve a luminance ramp while adding hue change across the scale.
- If you must keep a discrete scale, keep the number of bins small enough that readers are not forced into low-span judgments.
