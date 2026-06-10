---
id: overlay-explicit-outlier-markers-for-interval-outlier-counts
title: Overlay explicit outlier markers for interval outlier counts
bibliography: references.bib
description: For outlier-count comparisons over grouped time intervals, use explicit
  outlier overlays on color-based time-series summaries to improve fidelity and mitigate
  missed unusual values for viewers comparing interval outlier frequency.
labels:
- purpose:refine
- basis:empirical
- task:distribute
- time:time-interval
- chart:heatmap
- shape:outlier-rich
- quality:fidelity
- lever:encoding
---

## Outlier overlays on the field <!-- role: advice -->

Overlay explicit outlier marks when viewers must compare how many unusual values appear in each interval. For example, draw broad outlier stripes on top of a smoothed colorfield so unusual values stand out while the underlying field still preserves context.

## Why explicit outlier overlays work <!-- role: reason -->

Outlier counting is easier when unusual values are visually boosted instead of buried inside the full signal. The context field still helps readers keep those outliers tied to their surrounding interval.

**Mechanism:** The overlay makes unusual values visually salient for numerosity estimation, while the smoothed background preserves the broader time-series context.

**Evidence:** In the outlier experiment, event striping outperformed all other tested displays, and the paper attributes this advantage to explicitly mapping outliers while retaining a contextual colorfield underneath [@albersTaskdrivenEvaluationAggregation2014].

## Use when counting unusual values is the task <!-- role: context -->

- **User Goal:** Identify which interval contains the most outliers.
- **Task:** Compare outlier frequency across known time blocks.
- **Data:** Quantitative time series with unusual values that should be highlighted.
- **Chart Setting:** A colorfield-like overview where both context and outlier emphasis matter.
- **Success Criterion:** Higher accuracy on outlier-count comparisons.

## Do not use when the task is a different summary comparison <!-- role: exceptions -->

**Break it when:** The primary task is comparing interval averages or spread instead of counting outliers. **Why:** The paper reports that event striping underperformed standard colorfields on all summary tasks except outlier detection.

## Costs of adding the outlier overlay <!-- role: costs -->

**Sacrifice:** You make the display less general-purpose for other summary tasks.
**Risk:** A design tuned for outlier emphasis can distract from reading averages or spread.
**Mitigation:** Reserve the overlay for views whose main job is outlier comparison.

## Common failure with this lever <!-- role: mistakes -->

**Mistake:** Rely on a smoothed colorfield alone for outlier-count comparison. **Why it fails:** Unusual values are not explicitly boosted, so readers have more difficulty seeing and counting them.

## How to test the choice <!-- role: check -->

**Failure Sign:** Reviewers miss isolated unusual values or disagree on which interval contains more of them.
**Quick Check:** Show the same data with and without the outlier overlay, then ask which interval has the most outliers.
**Stronger Test:** Repeat the A/B check on cases where outliers are distributed across several intervals rather than concentrated in one.

## What to change <!-- role: fix -->

- Add a separate visual layer for outliers above the background field.
- Make the outlier marks broad enough to be counted quickly.
- Keep a smoothed background field underneath so the interval context remains visible.
