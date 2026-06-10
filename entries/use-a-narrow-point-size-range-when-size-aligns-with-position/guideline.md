---
id: use-a-narrow-point-size-range-when-size-aligns-with-position
title: Use a narrow point-size range when point size aligns with position in scatterplots
bibliography: references.bib
description: For summary judgments of x/y mean position, use a narrow point-size range
  on scatterplots with area-encoded third variables that correlate with position to
  improve fidelity and mitigate mean-pull bias for readers estimating the overall
  average.
labels:
- purpose:refine
- basis:empirical
- chart:scatter
- measure:multi
- lever:encoding
- channel:area
- quality:fidelity:use
---

## Point-size range for correlated bubble marks <!-- role: advice -->

Keep the point-size scale narrow when point area is used on a scatterplot and the size field aligns with x/y position. For example, when larger points cluster along one diagonal or in one corner, compress the smallest-to-largest size spread instead of using a medium or wide bubble range.

## Why a narrow size range reduces bias <!-- role: reason -->

When point size is correlated with position, larger marks gather on one side of the scatterplot and pull the perceived center in that direction. Wider size ranges increase the contrast between small and large marks, which strengthens that pull under high correlation.

**Mechanism:** Compressing the size range reduces the visual dominance of the largest marks, so they exert less extra influence on the perceived mean.

**Evidence:** The underlying experiment found a significant interaction between size range and correlation for bias: under high correlation, medium and wide size ranges were more biased than a narrow size range, and the collated results rank the high-correlation wide and medium area conditions among the worst for mean-position bias [@hongWeightedAverageIllusion2022; @zengReviewCollationGraphical2023].

## Use when size and position move together <!-- role: context -->

- **User Goal:** Estimate the overall x/y mean of the point cloud.
- **Task:** Make a summary judgment from the plotted positions rather than read exact bubble sizes.
- **Data:** A third quantitative variable is encoded with point area, and that variable is positively or negatively correlated with x/y position.
- **Chart Setting:** A bubble-like scatterplot is already chosen and the designer controls the point-size scale.
- **Audience:** Readers are expected to judge the mean visually from the marks.
- **Success Criterion:** The perceived mean is not pulled strongly toward the larger-point cluster.

## Do not use when size is not aligned with position <!-- role: exceptions -->

**Break it when:** Point area does not align with position. **Why:** The experiment did not find a significant effect of size range alone; the extra bias appeared when correlation and size range interacted.

## What you give up by narrowing the scale <!-- role: costs -->

**Sacrifice:** You reduce the dynamic range of the size encoding.
**Risk:** The third variable can become harder to read from individual points.
**Mitigation:** Reserve this change for views where mean-position fidelity matters more than exact size comparison.

## Common failure with bubble emphasis <!-- role: mistakes -->

**Mistake:** Widening the bubble-size range to emphasize the third variable while still expecting accurate mean-position judgments. **Why it fails:** Medium and wide size ranges became more biased than a narrow range when size was highly correlated with position.

## How to test the size-range choice <!-- role: check -->

**Failure Sign:** Large bubbles cluster together and the size scale spans a strong small-to-large contrast.
**Quick Check:** Compare the current chart to a narrow-size version with the same positions and data.
**Stronger Test:** Ask a reviewer to click the perceived mean on both versions; if the wider version is pulled farther toward the large-bubble cluster, compress the size scale.

## What to change in the chart <!-- role: fix -->

- Reduce the minimum-to-maximum bubble-size spread to a narrow range.
- Keep the x/y positions and the data mapping fixed while compressing the size scale.
- If mean-position judgment is still critical and size remains distracting, remap the third variable to point lightness.
