---
id: add-explicit-interval-extrema-for-range-and-minimum-comparisons
title: Add explicit interval minima and maxima for within-interval range comparisons
bibliography: references.bib
description: For within-interval extremum and range comparisons in ordered time, use
  explicit interval extrema overlays on line charts to maximize fidelity and address
  missed local highs and lows for exact interval judgments.
labels:
- purpose:refine
- basis:empirical
- task:extreme
- time:ordered-time
- chart:line
- quality:fidelity
- lever:encoding
- channel:position:use
---

## Add interval extrema overlays <!-- role: advice -->

Overlay explicit interval minima and maxima when readers must compare within-interval lows, highs, or ranges. For example, add per-interval high and low markers or bars to a line chart instead of leaving range and minimum judgments to the raw trace alone.

## Why explicit extrema help <!-- role: reason -->

Range and minimum comparisons become easier when the chart exposes each interval's endpoints directly. Readers no longer need to scan the full trace to reconstruct local highs and lows before comparing intervals.

**Mechanism:** Explicit extrema overlays convert a search through many raw points into a direct comparison of already-marked interval endpoints.

**Evidence:** In the time-series experiment, modified stock charts and box plots, both of which explicitly encoded interval extrema, outperformed the plain line graph on minimum and range tasks, and the review summarizes this paper as showing position-based charts with explicit summaries helping find-extremum and determine-range tasks. [@albersTaskdrivenEvaluationAggregation2014; @zengReviewCollationGraphical2023]

**Notes:** The source also warns that adding more summaries can introduce clutter.

## Use when readers compare lows or spans by interval <!-- role: context -->

- **User Goal:** Compare the lowest point or the full high-low span across repeated time intervals.
- **Task:** Interval minimum or interval range comparison.
- **Data:** Ordered time series partitioned into discrete intervals such as months.
- **Chart Setting:** A line chart is already in use and the raw series still needs to remain visible.
- **Success Criterion:** More accurate answers on interval minimum and range questions.

## Do not use when the summary target is different <!-- role: exceptions -->

**Break it when:** The main question is interval average or spread rather than extrema or range. **Why:** extrema overlays do not directly encode mean or spread, and other designs performed better for those tasks.

## What you give up <!-- role: costs -->

**Sacrifice:** A simpler, less annotated line display.
**Risk:** The extra summary marks can create visual clutter.
**Mitigation:** Add only the extrema summaries needed for the target comparison.

## Common overlay mistake <!-- role: mistakes -->

**Mistake:** Add a moving average but still omit interval minima and maxima for a range task. **Why it fails:** The mean overlay does not expose the local endpoints that define minimum and range.

## How to check the overlay <!-- role: check -->

**Failure Sign:** Reviewers must trace the whole line to estimate each interval's low and high before answering.
**Quick Check:** Ask whether each interval's minimum and maximum can be pointed to directly without scanning the full trace.
**Stronger Test:** A/B test the same line chart with and without extrema overlays on interval minimum and range questions.

## How to fix it <!-- role: fix -->

- Add one explicit maximum mark for each target interval.
- Add one explicit minimum mark for each target interval.
- Keep the raw line underneath the summaries if point-level context still matters.
- If the real task is spread rather than range, switch to interval box plots instead of adding more extrema overlays.
