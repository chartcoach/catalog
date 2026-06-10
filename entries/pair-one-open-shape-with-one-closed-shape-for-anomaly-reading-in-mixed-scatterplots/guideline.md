---
id: pair-one-open-shape-with-one-closed-shape-for-anomaly-reading-in-mixed-scatterplots
title: Pair one open shape with one closed shape for anomaly reading in mixed scatterplots
bibliography: references.bib
description: For anomaly-style reading in single-view scatterplots, prefer mixed open
  and closed shape encodings on heterogeneous point displays to improve fidelity and
  mitigate within-category interference in dense point clouds for readers scanning
  grouped points.
labels:
- purpose:refine
- basis:empirical
- chart:scatter
- quality:fidelity
- lever:encoding
- channel:shape:use
- reading-mode:overview
- density:dense
---

## Mixed open and closed shape pairs <!-- role: advice -->

Use one open shape and one closed shape when a single scatterplot must help readers spot which group stands out. For example, use triangle plus cross or square plus cross instead of triangle plus square or asterisk plus cross when both groups share one dense point field.

## Why mixed pairs work for anomaly-style reading <!-- role: reason -->

Mixed open/closed pairs separate the groups more than same-category pairs when both are interleaved in one point cloud. That separation reduces the interference that happens during quick overview judgments about which group stands out.

**Mechanism:** Mixing one open symbol with one closed symbol makes the two groups easier to distinguish in a heterogeneous scatterplot, which improves anomaly-style or numerosity-style reading.

**Evidence:** In the collated find-anomalies results, every mixed open/closed pair ranked above both the closed-closed pair and the open-open pair, and the top mixed pairs were significantly more accurate than both same-category pairs. The source paper also concludes that symbols from the same open/closed category interfere more than symbols from different categories in heterogeneous scatterplot displays, especially for numerosity-style judgments [@zengReviewCollationGraphical2023; @burlinsonOpenVsClosed2018].

**Notes:** The mixed-pair advantage is about shared single-plot displays, not separate homogeneous plots.

## Use when all are true <!-- role: context -->

- **User Goal:** Decide which group stands out in a shared point cloud.
- **Task:** Quick overview judgment across two shape-coded groups, including numerosity-style anomaly reading.
- **Data:** Two quantitative axes with one categorical grouping mapped to shape.
- **Chart Setting:** One scatterplot contains both groups at once, and the display is heterogeneous and visually cluttered.
- **Audience:** Readers scanning for the more prominent group.
- **Success Criterion:** Higher identification accuracy when both groups share the same plot.

## Do not use when any are true <!-- role: exceptions -->

**Break it when:** The chart's main job is trend judgment, or the groups are separated into side-by-side homogeneous plots. **Why:** The collated correlate task ranked the closed-closed pair highest, and the study did not find a reliable open/closed advantage in separate-plot homogeneous displays.

## What this costs <!-- role: costs -->

**Sacrifice:** The mixed pair is not the best choice for every task on the same scatterplot.\
**Risk:** If the chart later becomes a trend-judgment view, the mixed pair can underperform a closed-closed pair.\
**Mitigation:** Choose the shape pair by the primary task before finalizing the legend.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Use two shapes from the same open/closed category in a shared scatterplot meant for anomaly-style overview reading. **Why it fails:** Same-category pairings caused more interference, and the open-open pair was the worst anomaly condition.

## How to test it <!-- role: check -->

**Failure Sign:** Readers misidentify which group stands out or need repeated looks at the legend.\
**Quick Check:** If both legend symbols are open or both are closed in one dense mixed scatterplot, flag it.\
**Stronger Test:** Compare the current pair against a triangle-cross or square-cross version on the same task and count correct responses.

## What to change <!-- role: fix -->

- Change one of the two symbols so the pair spans one open shape and one closed shape.
- Start with triangle-cross or square-cross if you need a direct source-tested revision.
- If the chart's real job is trend judgment, switch the pair to two closed shapes instead of keeping the mixed pair.
