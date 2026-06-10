---
id: compute-aggregates-at-the-task-interval-for-average-comparisons
title: Compute aggregates at the task interval for average comparisons
bibliography: references.bib
description: For average-comparison tasks over grouped time intervals, use discrete
  per-interval aggregate encoding on time-series charts to improve fidelity and mitigate
  errors caused by continuous aggregation for viewers comparing grouped results.
labels:
- purpose:refine
- basis:empirical
- task:compare
- scope:grouped-result
- time:time-interval
- data:temporal
- quality:fidelity
- lever:encoding
---

## Discrete interval aggregates <!-- role: advice -->

Compute and display the summary at the same interval the reader must compare. For example, add one average bar per month in a composite graph instead of relying on a continuous moving-average line when the question asks which month has the highest average.

## Why task-aligned aggregation works <!-- role: reason -->

Average comparison becomes easier when the chart already matches the grouping used in the question. Readers no longer need to mentally segment a continuous summary into monthly chunks before comparing them.

**Mechanism:** Discrete per-interval summaries align the visual unit of comparison with the task unit of comparison, reducing the extra work of extracting monthly values from a continuous smoothing line.

**Evidence:** For average comparisons, encodings that discretely aggregated the data per month outperformed the remaining encodings, and the paper highlights composite graphs as better matched to this task than a continuous moving-average display [@albersTaskdrivenEvaluationAggregation2014].

## Use when the interval is known in advance <!-- role: context -->

- **User Goal:** Decide which time interval has the highest average.
- **Task:** Compare summaries across fixed blocks such as months.
- **Data:** Quantitative time series with a known grouping level.
- **Chart Setting:** A chart where the designer can compute interval summaries before display.
- **Success Criterion:** Higher accuracy on interval-average comparisons.

## Do not use when the needed interval can change <!-- role: exceptions -->

**Break it when:** The reader's comparison granularity is not known ahead of time or may shift across weeks, months, or other scopes. **Why:** The paper notes that discrete aggregation requires prior task knowledge and can misalign the chart with the reader's actual scope.

## Costs of discrete aggregation <!-- role: costs -->

**Sacrifice:** You give up some flexibility for other temporal scopes and some raw local detail.
**Risk:** A summary computed for months may not help with week-level questions.
**Mitigation:** Keep the raw series visible underneath the interval summary when both local detail and interval averages matter.

## Common failure with this lever <!-- role: mistakes -->

**Mistake:** Add only a continuous moving-average line when the reader must compare averages for discrete time blocks. **Why it fails:** The reader still has to estimate where each block begins and ends and mentally recover a block-level average from a continuous curve.

## How to test the choice <!-- role: check -->

**Failure Sign:** Reviewers trace along a smoothing line instead of directly comparing one summary mark per interval.
**Quick Check:** Show the same data once with per-interval averages and once with a moving average, then ask which interval has the highest average.
**Stronger Test:** Repeat the A/B check across several datasets with different distractor intervals to confirm that the discrete version remains more accurate.

## What to change <!-- role: fix -->

- Replace a continuous moving-average overlay with one summary mark per task interval.
- Use bars or other discrete marks to encode the average for each interval.
- Overlay the raw line beneath the discrete averages if readers still need the original series.
