---
id: design-the-color-key-with-endpoints-and-even-intervals
title: Design the color key with endpoints and even intervals
bibliography: references.bib
description: For ordered choropleth legends, use a color key with scale endpoints,
  evenly spaced intermediate values, and a center on diverging scales to improve readability
  and mitigate confusing legend decoding for readers interpreting map colors.
labels:
- purpose:refine
- basis:heuristic
- chart:choropleth
- component:legend:use
- quality:readability
- lever:text-annotation
- polish:annotation
---

## Color key structure <!-- role: advice -->

Make the color key show the full ordered scale in regular steps. For example, show the lowest and highest values plus two to four evenly spaced values in between, and include the center value when the palette is diverging.

## Why a regular legend is easier to decode <!-- role: reason -->

Readers understand map colors faster when the legend is simple and evenly structured.

**Mechanism:** A key that shows the endpoints and regular steps gives readers a quick mental model of the scale. Adding the midpoint on a diverging scale clarifies what the two sides mean.

**Evidence:** The post says color keys are crucial, recommends showing low and high values plus two to four in-between values for sequential schemes, warns against uneven intervals such as 0, 15, 50, and says diverging keys should display the center value [@muth_choroplethmaps_2018].

## Use when the map has an ordered color scale <!-- role: context -->

- **User Goal:** Help readers decode what the colors mean.
- **Task:** Read an ordered legend for a sequential or diverging scheme.
- **Data:** Ordered values with a continuous or stepped color key.
- **Chart Setting:** A choropleth uses a visible color key.
- **Audience:** Readers interpreting the legend during map reading.
- **Success Criterion:** The legend can be deciphered quickly.

## Do not use this structure for unordered categories <!-- role: exceptions -->

**Break it when:** The map uses a qualitative categorical color scheme. **Why:** The post gives this key structure for sequential and diverging scales, not for unordered categories.

## Costs of a fuller legend <!-- role: costs -->

**Sacrifice:** The legend takes more room than a minimal endpoint-only key.
**Risk:** Too many intermediate labels can make the key confusing.
**Mitigation:** Limit the intermediates to only a few evenly spaced values.

## Common legend-label failure <!-- role: mistakes -->

**Mistake:** Label the color key with uneven numeric intervals or omit the midpoint on a diverging scale. **Why it fails:** Readers get a harder-to-decipher legend and a less clear sense of the scale.

## Check whether the legend is regular <!-- role: check -->

**Failure Sign:** The legend labels jump by irregular amounts or the diverging midpoint is missing.
**Quick Check:** Read the key left to right and verify equal numeric intervals between labeled values.
**Stronger Test:** Count the labeled intermediates and keep only a few plus the endpoints and, if needed, the center.

## Edit the legend labels <!-- role: fix -->

- Add the lowest and highest labeled values to the key.
- Replace irregular legend labels with evenly spaced intervals.
- Add the center value on diverging scales.
- Remove extra intermediate labels that make the key harder to scan.
