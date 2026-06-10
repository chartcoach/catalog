---
id: use-box-plots-instead-of-line-graphs-for-interval-spread-comparisons
title: Use box plots instead of line graphs for interval spread comparisons
bibliography: references.bib
description: For spread comparisons across ordered-time intervals, use box plots instead
  of line graphs to maximize fidelity and address inferred variation from raw traces
  for exact interval judgments.
labels:
- purpose:select
- basis:empirical
- task:distribute
- time:ordered-time
- chart:box-violin:use
- chart:line:avoid
- quality:fidelity
- lever:chart-family
---

## Choose box plots for spread <!-- role: advice -->

Choose a box plot when readers must compare how spread out values are within each time interval. For example, use one box plot per month instead of a line graph when the question is which interval is most spread out from its average.

## Why box plots beat lines here <!-- role: reason -->

Spread comparison depends on seeing interval-level variation, not tracing a raw sequence of points. Box plots expose summary distribution structure directly, while line graphs force readers to infer spread from many individual values.

**Mechanism:** The box, whiskers, and central summary reduce the interval to a directly comparable distribution cue, so readers do less visual estimation of variability.

**Evidence:** In the time-series experiment, the box plot was the top-performing design for the spread task and outperformed the plain line graph, and the review summarizes the same paper as showing that different chart types support different summary tasks differently. [@albersTaskdrivenEvaluationAggregation2014; @zengReviewCollationGraphical2023]

## Use when spread is the real question <!-- role: context -->

- **User Goal:** Compare dispersion across repeated time intervals.
- **Task:** Interval spread comparison.
- **Data:** Ordered time series partitioned into repeated intervals such as months.
- **Chart Setting:** Readers do not need to inspect every raw point while making the spread decision.
- **Success Criterion:** Higher answer accuracy on interval spread questions.

## Do not use when raw points or anomaly counts must stay visible <!-- role: exceptions -->

**Break it when:** Readers must inspect raw point values or count outliers within each interval. **Why:** the box plot replaces the raw series, and the study did not use it for the outlier-count task.

## What you give up <!-- role: costs -->

**Sacrifice:** Direct visibility of every raw value in the series.
**Risk:** Tasks that depend on local features or anomaly counts can become harder or unsupported.
**Mitigation:** Use a different view when the task depends on raw points instead of spread summaries.

## Common selection mistake <!-- role: mistakes -->

**Mistake:** Keep a line graph for a spread comparison because it preserves every point. **Why it fails:** Readers must infer dispersion from many points, and accuracy is lower than with a box plot.

## How to check the chart choice <!-- role: check -->

**Failure Sign:** Reviewers trace the whole line to estimate which interval varies most.
**Quick Check:** Show the same spread question once with a line graph and once with interval box plots.
**Stronger Test:** Keep the box plot if it yields more accurate answers to a forced-choice question about which interval is most spread out.

## How to fix it <!-- role: fix -->

- Replace the line graph with one box plot per target interval.
- Keep the boxes in the same time order as the original series.
- If the real question is range rather than spread, switch to explicit interval minima and maxima instead of a line graph.
