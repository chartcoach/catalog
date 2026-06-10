---
id: make-unequal-numeric-ranges-visible-in-the-color-key
title: Make unequal numeric ranges visible in the color key
bibliography: references.bib
description: For exact and lookup reading in quantitative color keys, use legend segment
  sizing and endpoint labeling on non-linear or uneven diverging scales to improve
  fidelity and mitigate false assumptions of equal ranges for readers interpreting
  magnitude.
labels:
- purpose:refine
- basis:heuristic
- data:quantitative
- quality:fidelity
- lever:encoding
- component:legend:use
- reading-mode:exact
---

## Unequal range encoding <!-- role: advice -->

Make unequal numeric ranges visible in the color key itself. For example, give classes different widths when they cover different value spans, label the min and max when the end classes are much larger than the others, and place the center of a diverging key closer to the side with the smaller extreme range.

## Equal-looking segments imply equal coverage <!-- role: reason -->

Readers naturally infer that equal-looking legend segments represent equal numeric intervals. When the scale is non-linear or the diverging extremes are uneven, the key needs to show that difference directly.

**Mechanism:** Segment width and center position communicate the actual numeric span of each part of the scale, preventing a false equal-interval reading.

**Evidence:** The post says that non-linear interpolations should be communicated clearly, recommends labeling min and max when first or last classes are much bigger than the others, calls differently sized classes an elegant way to show the interpolation, and says uneven diverging extremes should be made obvious by placing the center closer to the nearer extreme in both color and key design. [@muth_color_keys_2023]

## Use when the scale is not evenly spaced <!-- role: context -->

- **User Goal:** Read the scale truthfully rather than assume equal intervals.
- **Data:** Quantitative color scale with non-linear class widths or uneven diverging extremes.
- **Chart Setting:** The legend currently risks making unequal ranges look equal.
- **Audience:** Readers are using the key to interpret magnitude and range.
- **Success Criterion:** The legend reflects the real interval structure of the scale.

## Do not use when the scale is already even <!-- role: exceptions -->

**Break it when:** The class intervals are consistent or the diverging extremes are balanced around the center. **Why:** Equal-sized legend segments already represent the scale truthfully.

## Cost of a more truthful legend <!-- role: costs -->

**Sacrifice:** You lose the neat simplicity of evenly sized legend blocks.\
**Risk:** If unequal widths are subtle or unlabeled, readers may miss why the segments differ.\
**Mitigation:** Pair unequal widths with clear endpoint labels when needed.

## Common equal-interval illusion <!-- role: mistakes -->

**Mistake:** Draw equal-width legend segments for unequal numeric ranges, or center a diverging key visually when the extremes are numerically uneven. **Why it fails:** The key suggests a scale structure that the data does not have.

## Quick review for interval truthfulness <!-- role: check -->

**Failure Sign:** All legend segments look the same width even though their numeric spans differ.\
**Quick Check:** Compare each segment's visual width to the numeric range it covers.\
**Stronger Test:** Verify that the diverging center sits at the true split between the two unequal extremes.

## Concrete edits for uneven scales <!-- role: fix -->

- Resize legend segments so wider segments cover wider numeric ranges.
- Add min and max labels when unusually large end ranges might be missed.
- Move the center of a diverging key so it reflects the actual numeric balance of the two sides.
