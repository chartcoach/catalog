---
id: use-diverging-color-scale-to-show-more-differences
title: Use a diverging color scale to make within-range differences more visible
bibliography: references.bib
description: For difference reading in quantitative color-encoded charts, use a diverging
  color scale on data with a midpoint to improve insight and address compressed visual
  differences within a full-range sequential ramp for readers comparing nearby values.
labels:
- purpose:refine
- basis:heuristic
- task:compare
- data:quantitative
- quality:insight
- lever:encoding
- operator:difference
- aesthetic:color:use
---

## Increase color resolution within each half-range <!-- role: advice -->

Use a diverging color scale when readers need to see smaller differences within the lower or upper half of the range. For example, a diverging map or calendar heatmap can make 10- or 20-point differences more visible because each gradient covers only half the full range instead of all of it.

## Why half-range gradients separate values better <!-- role: reason -->

A single sequential gradient spreads all values across one ramp. A diverging scale splits the range in two, so similar numeric gaps produce larger visible differences within each half.

**Mechanism:** Separate gradients for the two sides of the midpoint increase visible contrast within each side of the data range.

**Evidence:** The article says diverging scales let readers see more differences because one gradient covers only half the number range, making modest gaps more pronounced in examples such as maps and a calendar heatmap [@muth_diverging_vs_sequential_2021].

## Use when nearby values need to look different <!-- role: context -->

- **User Goal:** Make nearby quantitative values easier to distinguish by color.
- **Task:** Compare differences within the lower half or upper half of the scale.
- **Data:** Quantitative values with a meaningful middle point and important variation on each side.
- **Chart Setting:** A chart such as a map or heatmap that already uses a quantitative color scale.
- **Audience:** Readers are comparing similar values, not only locating the maximum.
- **Success Criterion:** Values a modest distance apart no longer look almost the same color.

## Do not use when immediate decoding matters more <!-- role: exceptions -->

**Break it when:** Immediate intuitive reading without consulting a legend matters more than extra differentiation. **Why:** Diverging scales are less intuitive and require clearer decoding support.

## Costs of more visible differences <!-- role: costs -->

**Sacrifice:** You add decoding work because the scale has two sides.\
**Risk:** Readers may not know which side is high or low if the midpoint and key are unclear.\
**Mitigation:** Make the midpoint and endpoints explicit in the legend or surrounding text.

## Common difference-reading failure <!-- role: mistakes -->

**Mistake:** Using a sequential ramp across the entire range when the important comparisons happen within one half of the range. **Why it fails:** Modest gaps collapse into nearly the same color.

## Check whether differences are being compressed <!-- role: check -->

**Failure Sign:** Values that are meaningfully apart still look only slightly different in color.\
**Quick Check:** Compare two nearby values in the same half of the range across sequential and diverging previews; if diverging makes their gap visibly clearer, use it.\
**Stronger Test:** Inspect whether one gradient is covering the full range or whether each half has its own gradient.

## Fix compressed color differences <!-- role: fix -->

- Split the scale into a diverging palette centered on the meaningful middle value.
- Recheck the legend so readers know which side of the midpoint each hue represents.
- Keep the sequential scale only if the added decoding cost is not acceptable.
