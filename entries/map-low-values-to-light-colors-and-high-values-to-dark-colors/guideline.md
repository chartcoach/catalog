---
id: map-low-values-to-light-colors-and-high-values-to-dark-colors
title: Map low values to light colors and high values to dark colors
bibliography: references.bib
description: For magnitude encoding with sequential color scales, use light-to-dark
  ordering on the palette to improve fidelity and mitigate reversed value interpretation
  for readers.
labels:
- purpose:refine
- basis:heuristic
- data:quantitative
- quality:fidelity
- lever:scale-order
- channel:color-lightness:use
- aesthetic:color:use
---

## Sequential scale order <!-- role: advice -->

Order a sequential gradient so lighter colors represent lower values and darker colors represent higher values. For example, reverse a map or heat-style palette if darker colors currently indicate smaller numbers.

## Why light-to-dark ordering feels intuitive <!-- role: reason -->

Readers tend to read darker colors as more and lighter colors as less, so reversing that order adds avoidable interpretation friction.

**Mechanism:** Matching low-to-high values with light-to-dark lightness lets readers infer scale direction quickly from color alone.

**Evidence:** The post explicitly recommends that in color gradients bright colors represent low values while dark colors represent high values because this is most intuitive for most readers [@muth_colors_2018].

## When to use light-to-dark ordering <!-- role: context -->

- **User Goal:** Read ordered values from color.
- **Data:** Quantitative values are encoded by a sequential gradient.
- **Chart Setting:** A legend or scale communicates low-to-high magnitude.
- **Success Criterion:** Readers can infer which colors mean lower and higher values without hesitation.

## When not to use this ordering rule <!-- role: exceptions -->

**Break it when:** Color is encoding categories instead of low-to-high values. **Why:** The rule applies to ordered gradients, not category palettes.

## Tradeoffs of light-to-dark ordering <!-- role: costs -->

**Sacrifice:** An existing branded palette may need to be reversed or replaced.
**Risk:** If the legend order is unclear, readers can still misread the scale.
**Mitigation:** Keep the legend endpoints explicit when you reverse the palette.

## Common sequential-scale mistake <!-- role: mistakes -->

**Mistake:** Mapping low values to dark colors and high values to light colors. **Why it fails:** The scale fights the more intuitive reading of dark as more and light as less.

## How to check sequential scale order <!-- role: check -->

**Failure Sign:** The darkest color in the legend is attached to the smallest value.
**Quick Check:** Read the low and high legend labels and compare them to the lightest and darkest colors.
**Stronger Test:** Ask whether a reader could infer the correct direction of the scale from color alone.

## How to fix reversed sequential scales <!-- role: fix -->

- Reverse the gradient so low values are light.
- Keep high values at the dark end of the palette.
- Update the legend so the labels match the corrected lightness order.
