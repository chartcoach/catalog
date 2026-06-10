---
id: use-discrete-interval-means-for-interval-average-comparisons
title: Use discrete interval means instead of a continuous moving average for interval-average
  comparisons
bibliography: references.bib
description: For interval-average comparisons in ordered time, use discrete interval
  mean encodings on time-series charts to maximize fidelity and address boundary-crossing
  summary cues for exact interval judgments.
labels:
- purpose:refine
- basis:empirical
- task:compare
- time:ordered-time
- quality:fidelity
- lever:encoding
---

## Encode one mean per interval <!-- role: advice -->

Compute and draw one mean for each comparison interval when readers must choose which interval has the highest average. For example, add a per-interval mean bar in a composite time-series view instead of relying only on a continuous moving-average line that crosses interval boundaries.

## Why discrete means work better <!-- role: reason -->

Average comparison improves when the displayed summary is computed at the same granularity the reader must compare. A continuous moving average does not line up cleanly with discrete interval judgments, but one mean readout per interval does.

**Mechanism:** Task-aligned discrete summaries let readers compare interval means directly instead of mentally segmenting a continuous smooth line into separate intervals.

**Evidence:** In the time-series experiment, the composite graph with discrete interval means outperformed the plain line graph and the modified stock chart on the average task, and the review summarizes this paper as showing that different designs support different tasks, with computationally aligned summaries helping aggregate comparisons. [@albersTaskdrivenEvaluationAggregation2014; @zengReviewCollationGraphical2023]

**Notes:** This rule depends on knowing the comparison interval in advance.

## Use when the interval is known and averages matter <!-- role: context -->

- **User Goal:** Select the interval with the highest average.
- **Task:** Compare averages across repeated time intervals.
- **Data:** Ordered time series grouped into known discrete intervals.
- **Chart Setting:** The chart currently shows raw values or a moving-average line, and the comparison interval is known beforehand.
- **Success Criterion:** Higher answer accuracy on interval-average questions.

## Do not use when local features drive the task <!-- role: exceptions -->

**Break it when:** The main question is a point maximum, point minimum, within-interval range, or anomaly count. **Why:** interval means suppress the local features those tasks require.

## What you give up <!-- role: costs -->

**Sacrifice:** Some raw day-to-day detail in the main comparison cue.
**Risk:** A discrete mean summary is only useful when the encoded interval matches the reader's task.
**Mitigation:** Keep the raw series visible underneath when readers still need point-level context.

## Common aggregation mistake <!-- role: mistakes -->

**Mistake:** Use only a moving-average line for a discrete interval-average question. **Why it fails:** The continuous smoothing is not computed at the same unit the reader must compare.

## How to check the aggregation level <!-- role: check -->

**Failure Sign:** The average cue crosses interval boundaries or fails to show one readout per interval.
**Quick Check:** Count whether the chart exposes exactly one mean value for each target interval.
**Stronger Test:** A/B test a moving-average view against a discrete-mean view on the same highest-average question.

## How to fix it <!-- role: fix -->

- Compute the mean separately for each target interval.
- Encode each interval mean as a discrete readout aligned to that interval.
- Keep the raw series as a separate overlaid line only if readers still need point-level context.
- Remove moving-average-only views when the job is discrete interval average comparison.
