---
id: use-a-hue-varying-palette-for-exact-value-lookup-on-continuous-maps
title: Use a hue-varying palette for exact value lookup on continuous maps
bibliography: references.bib
description: For exact value lookup on continuous quantitative maps, prefer a hue-varying
  palette on a color-encoded map to improve quantitative accuracy and mitigate location-matching
  errors for viewers reading mapped values.
labels:
- purpose:refine
- basis:empirical
- task:retrieve
- chart:map
- quality:fidelity:use
- lever:encoding
- operator:lookup
- aesthetic:color:use
---

## Hue-varying palette for value lookup <!-- role: advice -->

Use a hue-varying palette when the map must support exact value lookup at specific locations. For example, replace a greyscale ramp with a multi-hue palette on a continuous color map; rainbow ranked highest for lookup accuracy, spectral also ranked near the top, and greyscale ranked worst.

## Why hue variation helps lookup <!-- role: reason -->

Hue variation gives readers more distinct perceptual steps for matching a target value to a location on the map. In this study, higher spatial frequency increased error for every palette, but it did not change the relative ranking of the palettes.

**Mechanism:** A multi-hue ramp improves color-to-value discrimination during lookup, so readers can more accurately find a location matching a requested quantity.

**Evidence:** The collated retrieve-value ranking was E-9 > E-7 > E-5 > E-4 > E-6 > E-8 > E-3 > E-2 > E-1, with every tested color palette significantly outperforming greyscale; the paper interprets this as support for maximizing hue variation for quantity estimation regardless of spatial frequency [@zengReviewCollationGraphical2023; @redaGraphicalPerceptionContinuous2018].

## Use when lookup accuracy is the main job <!-- role: context -->

- **User Goal:** Find or verify the value at a specific location.
- **Task:** Exact value lookup on a continuous color-encoded surface.
- **Data:** Continuous quantitative data spread over space, including both low- and high-spatial-frequency fields.
- **Chart Setting:** A static pseudocolor map where color is the main encoding for the measured quantity.
- **Audience:** Viewers reading mapped values on a standard color display.
- **Success Criterion:** Lower absolute error in matching requested values to locations.

## Do not use when the task changes to fine-grained pattern reading <!-- role: exceptions -->

**Break it when:** The main task is matching fine-grained spatial patterns in a high-spatial-frequency map rather than reading exact values. **Why:** The paper recommends a different palette family for complex pattern perception and notes that rainbow-like lookup-oriented choices are not the best option there.

## Costs of prioritizing lookup accuracy <!-- role: costs -->

**Sacrifice:** You optimize exact lookup rather than every other reading task on the same map.
**Risk:** A palette chosen for lookup can be a poor fit when the main task shifts to fine-grained pattern matching on complex surfaces.
**Mitigation:** Re-evaluate the palette if the map’s job changes from value lookup to pattern or profile interpretation.

## Common lookup-palette failure <!-- role: mistakes -->

**Mistake:** Keeping a greyscale ramp or another low-hue palette when the map’s main job is exact value lookup. **Why it fails:** These palettes produced larger estimation errors than the hue-varying alternatives in the study.

## Check lookup performance directly <!-- role: check -->

**Failure Sign:** Readers miss requested values or choose locations far from the target quantity.
**Quick Check:** Show the same map with the current palette and with a multi-hue alternative, then ask readers to locate a specified value; keep the palette with smaller absolute error.
**Stronger Test:** Repeat the lookup check on both smooth and visually complex regions; keep the hue-varying palette only if it stays better in both.

## Fix the lookup palette <!-- role: fix -->

- Replace a greyscale ramp with a multi-hue palette on the same map.
- Test a hue-varying option with a larger hue range, such as a rainbow-like or spectral-like ramp.
- Re-run the same value-lookup prompts after the palette change and keep the version with smaller errors.
- If the map’s primary job becomes fine-grained pattern matching on complex data, switch away from the lookup-oriented palette family.
