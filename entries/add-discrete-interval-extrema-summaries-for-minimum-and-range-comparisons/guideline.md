---
id: add-discrete-interval-extrema-summaries-for-minimum-and-range-comparisons
title: Add discrete interval extrema summaries for minimum and range comparisons
bibliography: references.bib
description: For minimum and range comparisons over grouped time intervals, use explicit
  extrema summaries on position-based time-series charts to improve fidelity and mitigate
  errors from reading interval lows and spans off an unsummarized line.
labels:
- purpose:refine
- basis:empirical
- task:compare
- time:time-interval
- data:temporal
- quality:fidelity
- lever:encoding
- channel:position:use
---

## Explicit highs and lows per interval <!-- role: advice -->

Add explicit interval highs and lows when readers must compare minima or ranges across time blocks. For example, layer monthly range bars onto a line graph as in a modified stock chart, or show interval whiskers in a box plot, instead of forcing readers to infer lows and spans from the raw line alone.

## Why explicit extrema summaries work <!-- role: reason -->

Minimum and range judgments require readers to find and compare multiple points inside each interval. Directly encoding the interval high and low reduces that search and gives the reader a clearer monthly comparison unit.

**Mechanism:** Explicit extrema summaries turn a multi-step visual search into a direct interval comparison, especially for tasks that depend on the local minimum or on the gap between local minimum and maximum.

**Evidence:** For minima and range tasks, position encodings that explicitly encoded local extrema, such as modified stock charts and box plots, outperformed plain line graphs and other encodings without those summaries [@albersTaskdrivenEvaluationAggregation2014].

## Use when the reader compares interval lows or spans <!-- role: context -->

- **User Goal:** Find the interval with the lowest point or the largest max-minus-min range.
- **Task:** Compare extrema-derived summaries across known time blocks.
- **Data:** Quantitative time series partitioned into discrete intervals.
- **Chart Setting:** A position-based time-series chart where interval summaries can be added.
- **Success Criterion:** Higher accuracy on minimum and range judgments.

## Do not use this as a blanket fix for maxima <!-- role: exceptions -->

**Break it when:** The primary task is comparing interval maxima with box plots alone. **Why:** The paper reports that box plots did not outperform the other position encodings for maxima, and it notes possible whisker-related judgment biases.

## Costs of adding extrema summaries <!-- role: costs -->

**Sacrifice:** You add more visual structure to the chart.
**Risk:** A layered summary such as a modified stock chart can become visually cluttered.
**Mitigation:** Encode only the extrema summaries needed for the task instead of layering many different summaries at once.

## Common failure with this lever <!-- role: mistakes -->

**Mistake:** Leave viewers to recover interval lows and ranges from a plain line graph. **Why it fails:** Readers must search each interval for two separate points and then compare those derived values across intervals.

## How to test the choice <!-- role: check -->

**Failure Sign:** Reviewers scan back and forth across the raw line to estimate interval lows or spans.
**Quick Check:** Show the same data once with explicit interval highs and lows and once without them, then ask which interval has the lowest value or largest range.
**Stronger Test:** Run both questions on the same A/B pair to confirm that the explicit-summary version helps both tasks.

## What to change <!-- role: fix -->

- Add one low marker and one high marker per interval.
- Draw a range bar or whisker summary for each interval.
- Keep the original line underneath only if raw local detail is still needed.
- Replace the raw interval segments with a box-plot summary if clutter becomes a problem.
