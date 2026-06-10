---
id: use-a-diverging-color-scheme-around-a-meaningful-center
title: Use a diverging color scheme around a meaningful center
bibliography: references.bib
description: For overview comparison of regional deviations around a meaningful center,
  use a diverging color scheme on a choropleth to improve readability and mitigate
  hiding one side of the scale for readers scanning both extremes.
labels:
- purpose:refine
- basis:heuristic
- chart:choropleth
- quality:readability
- lever:encoding
- channel:color-lightness:use
- operator:difference
- reading-mode:overview
---

## Diverging palette choice <!-- role: advice -->

Use a diverging color scheme when the mapped values have a meaningful middle and both ends of the scale deserve attention. For example, color values below and above a central reference with different hues and keep the center value in the middle of the scale.

## Why two-sided scales reveal two-sided differences <!-- role: reason -->

A center-based palette makes above-versus-below differences visible at a glance.

**Mechanism:** A diverging scheme separates the two sides of a meaningful midpoint while still showing how far regions are from that center. Readers can locate both extremes instead of only the high end.

**Evidence:** The post recommends diverging schemes when attention should go to both extremes, such as differences between competing sides [@muth_choroplethmaps_2018].

## Use when the midpoint matters <!-- role: context -->

- **User Goal:** Show which regions are on either side of a reference value.
- **Task:** Compare negative versus positive or lower versus higher deviations.
- **Data:** One regional measure with a meaningful center.
- **Chart Setting:** A choropleth is already chosen.
- **Audience:** Readers scanning both ends of the distribution.
- **Success Criterion:** Both sides of the center are easy to distinguish.

## Do not use when the data is one-directional or unordered <!-- role: exceptions -->

**Break it when:** Only the high end needs emphasis, or the categories are unordered. **Why:** The post recommends sequential schemes for one-direction magnitude and qualitative schemes for unordered categories.

## Costs of a two-sided palette <!-- role: costs -->

**Sacrifice:** You reduce the emphasis on only one end of the scale.
**Risk:** The midpoint can disappear if it is not clearly set apart.
**Mitigation:** Make the middle color the lightest and keep the extremes darker.

## Common centerless divergence <!-- role: mistakes -->

**Mistake:** Use a diverging palette without a meaningful center value. **Why it fails:** The colors imply a split in the data that the values do not actually have.

## Check whether the map really needs two sides <!-- role: check -->

**Failure Sign:** One side of the scale matters, but the palette still splits the map into two hues.
**Quick Check:** Confirm that the legend shows an explicit center value and that the story depends on both ends of the scale.
**Stronger Test:** If removing the center would not change the message, switch back to a sequential scheme.

## Edit the palette around the midpoint <!-- role: fix -->

- Set an explicit center value for the scale.
- Assign one hue to values below the center and another hue to values above it.
- Make the center color the lightest point in the palette.
- Darken both extremes so the ends of the scale read clearly.
