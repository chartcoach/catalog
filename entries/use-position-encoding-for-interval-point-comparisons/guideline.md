---
id: use-position-encoding-for-interval-point-comparisons
title: Use position encoding for interval point comparisons
bibliography: references.bib
description: For point-comparison tasks over grouped time intervals, prefer position
  encoding on time-series charts to improve fidelity and mitigate missed extrema and
  range judgments for viewers making exact interval comparisons.
labels:
- purpose:refine
- basis:empirical
- task:compare
- time:time-interval
- data:temporal
- quality:fidelity
- lever:encoding
- channel:position:use
- channel:color-lightness:avoid
---

## Position encoding for point comparisons <!-- role: advice -->

Encode value with position when viewers must compare individual points or point-derived ranges across time intervals. For example, use a line graph or modified stock chart instead of a colorfield, woven colorfield, or event-striped color view when the task is to find the interval with the highest point, lowest point, or largest range.

## Why position works for these tasks <!-- role: reason -->

Point comparisons require readers to extract specific values before they compare intervals. Position supports that extraction more reliably than color when the chart must preserve individual highs, lows, and spans.

**Mechanism:** Position makes it easier to read and compare exact point locations, while color supports coarser summaries and makes single-point lookup less precise.

**Evidence:** In the maxima, minima, and range experiments, position-based encodings generally outperformed color-based encodings, supporting the prediction that position is better for point comparisons in time series aggregation tasks [@albersTaskdrivenEvaluationAggregation2014].

## Use when point lookup drives the decision <!-- role: context -->

- **User Goal:** Identify which interval contains the highest value, lowest value, or largest max-minus-min gap.
- **Task:** Compare point-level extrema across known time blocks such as months.
- **Data:** Quantitative time series grouped into discrete intervals.
- **Chart Setting:** A static time-series display where value could be encoded by position or by color.
- **Success Criterion:** Higher accuracy on interval extrema and range judgments.

## Do not use when summary comparison is the main task <!-- role: exceptions -->

**Break it when:** The primary task is comparing interval summaries such as average or spread rather than extracting individual points. **Why:** The paper found that color-based aggregation and explicit interval summaries can better support those summary judgments than raw position alone.

## Costs of prioritizing position <!-- role: costs -->

**Sacrifice:** You give up some support for fast visual summarization of whole intervals.
**Risk:** A plain line can still leave average or spread judgments hard if those summaries are not encoded explicitly.
**Mitigation:** Add task-relevant interval summaries when summary comparison matters alongside point lookup.

## Common failure with this lever <!-- role: mistakes -->

**Mistake:** Encode value only with color for tasks that ask readers to find interval maxima, minima, or ranges. **Why it fails:** Readers must recover specific point values from color, and the study showed that this lowers accuracy on those point-comparison tasks.

## How to test the choice <!-- role: check -->

**Failure Sign:** Reviewers can describe broad color differences but struggle to name the interval containing the extreme point or largest range.
**Quick Check:** Show the same series once with position encoding and once with color encoding, then ask which interval contains the highest point, lowest point, or largest range.
**Stronger Test:** Repeat the A/B check on both smoother and noisier series to see whether the position version remains more reliable.

## What to change <!-- role: fix -->

- Switch the primary value channel from color to vertical position.
- Replace a colorfield-style view with a line-based position view for extrema and range questions.
- Add discrete interval markers for highs and lows if readers must compare ranges across intervals.
