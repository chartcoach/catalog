---
id: use-a-pie-chart-instead-of-an-unscaled-stacked-bar-for-exact-part-to-whole-estimation
title: Use a pie chart instead of an unscaled stacked bar for exact part-to-whole
  estimation
bibliography: references.bib
description: For exact part-to-whole estimation, prefer a pie chart over an unscaled
  stacked bar on two-segment part-to-whole displays to improve accuracy and mitigate
  error-prone share judgments for readers estimating a highlighted segment.
labels:
- purpose:select
- basis:empirical
- chart:pie-donut:use
- chart:bar:avoid
- quality:fidelity:use
- lever:chart-family
- operator:part-whole
- reading-mode:exact
---

## Choose the pie chart over the unscaled stacked bar <!-- role: advice -->

Use a pie chart when readers must estimate the exact size of one highlighted share in a two-part whole and the alternative is an unscaled stacked bar. For example, use a baseline pie chart instead of a baseline two-segment stacked bar when the reader must enter the darker segment as a whole-number percentage.

## Why the pie chart works better here <!-- role: reason -->

This design choice changes the chart family, not the data. In this specific two-segment exact-reading setup, the pie chart produced smaller estimation error than the unscaled stacked bar.

**Mechanism:** The pie chart gives readers a more accurate basis for estimating a single highlighted share in a two-part whole than the baseline stacked bar used in the comparison.

**Evidence:** In the baseline chart comparison, the pie chart ranked above the stacked bar for accuracy, and the difference was reported as significant. The review records this result as an empirical chart-selection finding for part-to-whole estimation [@redmondVisualCuesEstimation2019; @zengReviewCollationGraphical2023].

**Notes:** This guideline applies to the baseline bar contrast tested in the source, not to all bar-chart variants.

## Use when the chart matches the tested contrast <!-- role: context -->

- **User Goal:** Read the value of one highlighted share as accurately as possible.
- **Data:** Two segments that sum to 100%.
- **Chart Setting:** A single part-to-whole chart with no external quantitative scale and no added internal cue marks.
- **Success Criterion:** Lower absolute error in estimated segment size.

## Do not use when the bar is no longer the baseline bar <!-- role: exceptions -->

**Break it when:** The alternative stacked bar includes an external quantitative scale or stronger internal cue marks. **Why:** The tested pie advantage was against the baseline unscaled bar, and the source also found more accurate refined bar variants.

## Costs of switching chart family <!-- role: costs -->

**Sacrifice:** You give up the bar chart version that can carry an external quantitative scale.
**Risk:** You can overgeneralize this result if you apply it to every bar variant instead of the unscaled baseline bar.
**Mitigation:** If the bar chart must stay, add a quantitative scale or stronger internal cues rather than leaving it as the baseline bar.

## Common selection mistake <!-- role: mistakes -->

**Mistake:** Keep an unscaled stacked bar because bar charts are assumed to be more accurate for part-to-whole estimation. **Why it fails:** In this tested two-segment exact-estimation setup, the baseline bar had higher estimation error than the baseline pie.

## Check the chart choice with a direct A/B test <!-- role: check -->

**Failure Sign:** Readers give noticeably inconsistent or inaccurate percentage estimates from the unscaled stacked bar.
**Quick Check:** Build a matched pie-chart version and a matched unscaled stacked-bar version of the same two-part split, then ask reviewers to estimate the highlighted share as a whole number.
**Stronger Test:** Compare absolute error across several share sizes rather than judging the choice from one example only.

## Fix the chart choice <!-- role: fix -->

- Replace the unscaled stacked bar with a pie chart for the same two-part whole.
- Keep the highlighted segment styling consistent across both versions when you compare them.
- If the stacked bar must remain, add an external quantitative scale or stronger internal cues instead of leaving it unscaled.
