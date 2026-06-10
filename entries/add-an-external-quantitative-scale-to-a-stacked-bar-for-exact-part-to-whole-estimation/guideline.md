---
id: add-an-external-quantitative-scale-to-a-stacked-bar-for-exact-part-to-whole-estimation
title: Add an external quantitative scale to a stacked bar for exact part-to-whole
  estimation
bibliography: references.bib
description: For exact part-to-whole estimation, prefer an external quantitative scale
  on stacked bar charts to improve accuracy and address high estimation error for
  readers judging a highlighted share.
labels:
- purpose:refine
- basis:empirical
- chart:bar
- quality:fidelity:use
- lever:text-annotation
- operator:part-whole
- reading-mode:exact
- component:axis:use
---

## Add a quantitative scale to the bar chart <!-- role: advice -->

Add an external quantitative scale when a stacked bar chart is already chosen and readers must estimate one share exactly. For example, keep the two-segment stacked bar and place a 0-100 scale beneath it instead of leaving the highlighted segment to be judged from the bar alone.

## Why the scale improves the bar chart <!-- role: reason -->

This refinement keeps the same bar chart and adds a precise readout aid. In the tested bar variants, the scaled version was the most accurate.

**Mechanism:** The external scale gives readers explicit numeric anchors for estimating the highlighted segment, which reduces absolute error compared with judging the bar without that aid.

**Evidence:** Among the tested bar-chart refinements, the bar with scale ranked above the bar with decile cues and the baseline bar for accuracy, with significant differences reported against both. The review records this as the strongest tested bar refinement in the collated evidence from this study [@redmondVisualCuesEstimation2019; @zengReviewCollationGraphical2023].

## Use when the bar chart is fixed and exact reading matters <!-- role: context -->

- **User Goal:** Improve exact value estimation without changing away from a bar chart.
- **Data:** Two segments that sum to 100%.
- **Chart Setting:** A stacked bar chart is already selected and there is room to show an external quantitative scale.
- **Success Criterion:** Lower absolute error for the highlighted segment.

## Do not use when the scale is not appropriate to the display <!-- role: exceptions -->

**Break it when:** The visualization cannot appropriately show an external quantitative scale. **Why:** The source explicitly notes that a scale is not ideal in all circumstances and suggests internal visual cues as the fallback.

## Costs of adding the scale <!-- role: costs -->

**Sacrifice:** You add an extra chart component that is not always appropriate in every visualization.
**Risk:** Forcing a scale into a constrained design can make the chart a poor fit for that setting.
**Mitigation:** If the scale cannot be shown, use internal cue marks as anchors instead.

## Common bar-chart refinement mistake <!-- role: mistakes -->

**Mistake:** Leave the stacked bar unscaled or rely on weaker internal cues when exact estimation is the goal. **Why it fails:** The source found the scaled bar more accurate than both the baseline bar and the decile-cue bar.

## Check whether the scale solves the reading problem <!-- role: check -->

**Failure Sign:** Readers miss the highlighted percentage or show large spread in their estimates on the bar chart.
**Quick Check:** Ask reviewers to estimate the highlighted share from the same stacked bar with and without the external scale, then compare absolute error.
**Stronger Test:** Compare the scaled bar directly against the decile-cue version, since both were tested as bar refinements.

## Fix the bar chart <!-- role: fix -->

- Add an external 0-100 quantitative scale to the stacked bar.
- Keep the highlighted segment unchanged so the only revision is the added scale.
- If the scale cannot be shown, switch to internal cue marks rather than leaving the bar as the baseline version.
