---
id: use-sequential-gradient-for-low-to-high-values
title: Use a sequential color gradient for values that run from low to high
bibliography: references.bib
description: For communicating low-to-high values, use a sequential color gradient
  on quantitative data to improve fidelity and mitigate unordered or two-sided readings
  for readers comparing magnitude.
labels:
- purpose:refine
- basis:heuristic
- data:quantitative
- quality:fidelity
- lever:encoding
- channel:color-lightness:use
---

## Use a one-direction gradient for low-to-high values <!-- role: advice -->

Use a sequential gradient when color encodes numbers that simply go from low to high. For example, map lower values to lighter color and higher values to darker color for measures such as income, temperature, or age.

## Why one-direction gradients fit ordered magnitudes <!-- role: reason -->

Sequential gradients show ordered progression in one direction. Readers can see that middle tones fall between lighter and darker values on the same scale.

**Mechanism:** A bright-to-dark or dark-to-bright run lets readers interpret every color as slightly lower or slightly higher than its neighbors.

**Evidence:** The article recommends sequential color scales for numbers that go from low to high and explains that a middle color reads as between the lighter and darker values [@muth_which_color_scale_2021].

## Use when the values have one ordered direction <!-- role: context -->

- **User Goal:** Compare magnitudes from smaller to larger values.
- **Task:** Read low-to-high progression from color alone.
- **Data:** The color-encoded field is numeric and ordered in one direction.
- **Chart Setting:** Color is being used to encode value ranges rather than category identities.
- **Audience:** Readers comparing relative magnitude across marks or areas.
- **Success Criterion:** The legend reads as one continuous progression from low to high.

## Do not use when the data splits around a meaningful center <!-- role: exceptions -->

**Break it when:** The values extend in two directions away from a meaningful middle value. **Why:** A one-direction gradient does not show both sides of the midpoint.

## Tradeoffs of a sequential gradient <!-- role: costs -->

**Sacrifice:** The scale does not mark a special center.
**Risk:** Using it on centered data hides the split between one side of the midpoint and the other.
**Mitigation:** Switch to a diverging scale when the midpoint itself matters.

## Common scale mistake <!-- role: mistakes -->

**Mistake:** Use unrelated hues or a diverging center for data that only increases from low to high. **Why it fails:** The color scale stops reading as one ordered progression.

## Check whether the legend reads in one direction <!-- role: check -->

**Failure Sign:** The legend does not read as a single run from lower to higher values.
**Quick Check:** Identify the low end and the high end and verify that every intermediate color falls between them.
**Stronger Test:** If the legend has a highlighted center or two opposing hue directions, the scale is not sequential.

## Fix the gradient <!-- role: fix -->

- Replace unrelated hues with a light-to-dark or dark-to-light gradient.
- Keep the legend as one ordered run from low to high.
- Remove any artificial center unless the data truly centers on one.
