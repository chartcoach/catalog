---
id: plot-slope-ratios-on-a-log-scale
title: Plot slope ratios on a log scale
bibliography: references.bib
description: For grouped-result comparison of target-absent to target-present slope
  ratios, use log encoding on quantitative ratio plots to improve fidelity and mitigate
  positive-skew distortion for domain experts.
labels:
- purpose:refine
- basis:empirical
- task:distribute
- data:quantitative
- quality:fidelity
- lever:encoding
- operator:distribution
- shape:skewed
---

## Log-transform the ratio <!-- role: advice -->

Plot the target-absent to target-present slope ratio with a log transform instead of raw ratio values. For example, use a histogram of log(slope ratio) or summarize ratio bins with mean log(ratio) or median ratio when raw ratios show a long right tail.

## Why log ratios work <!-- role: reason -->

Raw slope ratios expand sharply when the target-present slope gets close to zero, so a few efficient searches can dominate the display. A log transform compresses those extremes and makes the ratio distribution much closer to normal.

**Mechanism:** Log encoding reduces the visual and statistical pull of extreme small-denominator ratios, so the plotted distribution better reflects the typical relationship between target-present and target-absent slopes.

**Evidence:** The paper reports that untransformed slope ratios were strongly positively skewed, that log-transforming them made the distribution roughly normal, and that ratios became especially large as target-present slopes approached zero [@wolfeWhatCan11998].

**Notes:** The paper also plots median ratio and mean log(ratio) across target-present slope bins to reduce the effect of small denominators.

## Use when ratio skew can dominate <!-- role: context -->

- **User Goal:** Compare slope-ratio distributions or judge whether ratios differ from a 2:1 benchmark.
- **Task:** Summarize or visualize target-absent to target-present slope ratios across many observations or slope bins.
- **Data:** Quantitative slope pairs with some very small target-present slopes and a positively skewed raw ratio distribution.
- **Chart Setting:** A ratio histogram or a binned summary plot of slope ratio.
- **Audience:** Domain experts reading visual-search results.
- **Success Criterion:** The ratio view is not dominated by a few extreme values from very small denominators.

## Do not use when ratios cannot be logged <!-- role: exceptions -->

**Break it when:** Nonpositive ratios must be shown unchanged, or target-present slopes near zero cannot be filtered or handled separately. **Why:** Log values are undefined for nonpositive ratios, and near-zero denominators make raw ratios unstable.

## Tradeoffs of log ratios <!-- role: costs -->

**Sacrifice:** Raw ratio magnitudes become less direct to read off the axis.
**Risk:** Readers can compare logged values to a raw 2.0 benchmark if the transform is not stated clearly.
**Mitigation:** State that the axis or summary uses log(slope ratio) and note any removed nonpositive cases.

## Common raw-ratio failure <!-- role: mistakes -->

**Mistake:** Plot raw mean slope ratios across all observations without handling small target-present slopes. **Why it fails:** A small number of near-zero denominators can stretch the display and distort the apparent center of the distribution.

## How to verify the ratio scale <!-- role: check -->

**Failure Sign:** The ratio plot has a long right tail or a few extremely large values.
**Quick Check:** Count nonpositive ratios and inspect whether many target-present slopes are close to zero before plotting raw ratios.
**Stronger Test:** Compare the raw-ratio distribution with a log-ratio version and confirm that the log-transformed view is substantially less skewed.

## Edits that stabilize the ratio view <!-- role: fix -->

- Remove nonpositive ratio cases before plotting log(slope ratio).
- Replace a raw-ratio axis with a log-ratio axis for the main distribution view.
- Report median ratio or mean log(ratio) in slope bins where small target-present slopes inflate raw means.
