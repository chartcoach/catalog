---
id: use-a-diverging-chroma-varying-palette-for-gradient-comparison-on-high-frequency-continuous-maps
title: Use a diverging chroma-varying palette for gradient comparison on high-frequency
  continuous maps
bibliography: references.bib
description: For gradient comparison on high-spatial-frequency continuous maps, prefer
  a diverging chroma-varying palette on a color-encoded map to improve judgment accuracy
  and mitigate missed local gradient differences for viewers comparing spatial change.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:map
- quality:fidelity:use
- lever:encoding
- aesthetic:color:use
---

## Diverging palette for steepness comparison <!-- role: advice -->

Use a diverging chroma-varying palette when readers must compare local gradients in a visually complex continuous map. For example, replace greyscale with a coolwarm-like or blue-yellow-like diverging ramp when readers must judge which marked region is steeper on average in a high-spatial-frequency map.

## Why diverging chroma variation helps gradient judgments <!-- role: reason -->

Gradient comparison became easier as spatial complexity increased, but color choice only mattered in the complex fields. In smooth fields, the tested palettes behaved similarly, while at high spatial frequency the best diverging palettes separated from the lower-performing group.

**Mechanism:** In visually complex maps, a diverging palette with strong chroma variation makes local change differences easier to distinguish during side-by-side steepness judgments.

**Evidence:** In the collated high-frequency gradient-comparison result, E-6 ranked first and E-8 ranked third, and both significantly outperformed the lower-performing group; the source paper concludes that diverging chroma-varying ramps support gradient perception in high-spatial-frequency maps, while low-spatial-frequency maps showed no significant palette advantage [@zengReviewCollationGraphical2023; @redaGraphicalPerceptionContinuous2018].

## Use when the map is visually complex and the task is steepness comparison <!-- role: context -->

- **User Goal:** Decide which region changes faster on average.
- **Task:** Compare gradients between two marked map regions.
- **Data:** Continuous quantitative data with high spatial frequency and many small local features.
- **Chart Setting:** A static pseudocolor map where color is the main encoding for the surface.
- **Audience:** Viewers judging local change from the map image.
- **Success Criterion:** More correct steepness judgments between marked regions.

## Do not use when the map is smooth or the task is value lookup <!-- role: exceptions -->

**Break it when:** The field is low-spatial-frequency or the main task is exact quantity lookup rather than steepness comparison. **Why:** The study found no meaningful palette advantage for gradient judgments in smooth maps, and value lookup followed a different ranking.

## Costs of a gradient-specific palette choice <!-- role: costs -->

**Sacrifice:** You tune the palette for local change comparison rather than for all map-reading tasks.
**Risk:** Applying the same palette change to smooth maps adds visual change without measurable gradient-comparison gain.
**Mitigation:** Restrict this palette choice to visually complex fields where readers must compare gradients.

## Common gradient-comparison failure <!-- role: mistakes -->

**Mistake:** Swapping among palettes on a smooth map and expecting the palette change alone to improve steepness judgments. **Why it fails:** The study found no significant differences among the tested palettes at low spatial frequency.

## Check steepness judgments with an A/B comparison <!-- role: check -->

**Failure Sign:** Readers often choose the wrong region when asked which area is steeper on average.
**Quick Check:** Show the same high-frequency map twice, once with the current palette and once with a diverging chroma-varying palette, then ask readers which marked region is steeper; keep the version with more correct answers.
**Stronger Test:** Repeat the same steepness comparison across several high-frequency maps before standardizing the palette.

## Fix the gradient-comparison palette <!-- role: fix -->

- Replace a greyscale or non-diverging palette with a diverging chroma-varying ramp on the same high-frequency map.
- Test a coolwarm-like diverging ramp against the current palette using the same marked-region comparison.
- Retain the palette only if it improves correct steepness judgments on visually complex fields.
- Do not spend palette-optimization effort on smooth fields if steepness comparison is already the task.
