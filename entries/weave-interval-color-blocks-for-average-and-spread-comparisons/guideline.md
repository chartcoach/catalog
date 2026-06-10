---
id: weave-interval-color-blocks-for-average-and-spread-comparisons
title: Weave interval color blocks for average and spread comparisons
bibliography: references.bib
description: For average and spread comparisons over grouped time intervals, use blocked
  woven color encoding on colorfield charts to improve fidelity and mitigate distraction
  from local temporal structure for viewers reading interval-level summaries.
labels:
- purpose:refine
- basis:empirical
- task:compare
- time:time-interval
- chart:heatmap
- quality:fidelity
- lever:encoding
- channel:color-lightness:use
---

## Woven color blocks for interval summaries <!-- role: advice -->

Break local order inside each interval when using color to support interval summaries. For example, permute the cell positions within each month to form woven color blocks instead of a continuous colorfield when readers must compare interval averages or spread.

## Why weaving helps summary reading <!-- role: reason -->

A continuous strip preserves local temporal structure that can distract from judging the overall distribution inside each interval. Weaving turns each interval into a summary texture that is easier to compare at a glance.

**Mechanism:** By breaking local structure and grouping values into task-aligned blocks, the display better supports visual summarization of the interval's average level and variability.

**Evidence:** The paper reports that color weaving improved the perceptual system's ability to summarize encoded values, and woven colorfields outperformed standard colorfields on average and spread comparisons while point lookup became harder [@albersTaskdrivenEvaluationAggregation2014].

## Use when the chart is a color overview of grouped intervals <!-- role: context -->

- **User Goal:** Compare interval averages or interval spread rather than exact daily values.
- **Task:** Read summary patterns across known time blocks.
- **Data:** Quantitative time series encoded as color over discrete intervals.
- **Chart Setting:** A colorfield-style overview where the designer can rearrange values within each interval.
- **Success Criterion:** Higher accuracy on average and spread judgments.

## Do not use when exact points or outliers matter most <!-- role: exceptions -->

**Break it when:** The task is to find exact points, interval extrema, or the interval with the most outliers. **Why:** The paper notes that weaving makes particular datapoints harder to extract and the woven display underperformed on maxima, minima, range, and outlier tasks.

## Costs of weaving the field <!-- role: costs -->

**Sacrifice:** You lose local temporal structure within each interval.
**Risk:** Exact point lookup becomes harder because the original day order is no longer visible inside the block.
**Mitigation:** Use weaving only when the task is interval summary comparison.

## Common failure with this lever <!-- role: mistakes -->

**Mistake:** Keep the original sequential order in a continuous color strip for average or spread comparisons. **Why it fails:** Local streaks and shapes compete with the reader's attempt to summarize the interval as a whole.

## How to test the choice <!-- role: check -->

**Failure Sign:** Reviewers trace local color streaks instead of comparing whole interval blocks.
**Quick Check:** Show the same color-encoded series as a continuous strip and as woven interval blocks, then ask which interval has the highest average or greatest spread.
**Stronger Test:** Repeat the A/B check on both smoother and noisier series to see whether the woven version still supports the summary task better.

## What to change <!-- role: fix -->

- Regroup the display into task-aligned interval blocks.
- Randomly permute the cell positions within each block.
- Use the woven version only for summary tasks, not for exact day-level lookup.
