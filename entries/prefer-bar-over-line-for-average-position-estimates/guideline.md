---
id: prefer-bar-over-line-for-average-position-estimates
title: Prefer a bar chart over a line chart for average-position estimates
bibliography: references.bib
description: For short-delay average-position judgments, prefer the bar chart family
  over the line chart family on single-series quantitative displays to improve fidelity
  and mitigate systematic bias for readers estimating averages from memory.
labels:
- purpose:select
- basis:empirical
- chart:bar:use
- chart:line:avoid
- data:quantitative
- quality:fidelity
- lever:chart-family
- measure:single
---

## Chart family for average-position summaries <!-- role: advice -->

Choose a bar chart instead of a line chart when readers must recall the average vertical position of one quantitative series after a brief view. For example, use a single set of bars rather than a single line when the chart’s job is average-position estimation from memory and no other design constraint requires a line.

## Why bars work better here <!-- role: reason -->

Bars and lines both encode value with vertical position, but readers do not remember their average positions in the same way. In this task, line averages drift downward, while bar averages drift upward by less overall and with tighter judgments.

**Mechanism:** Choosing bars reduces the size of the remembered-average error for a single series, so the reported average stays closer to the intended vertical position.

**Evidence:** Across the experiments, single-line displays were systematically underestimated and single-bar displays were systematically overestimated; the paper’s design guidance notes that the bias was smaller and judgments were more precise for bars than for lines in this average-position task [@xiongBiasedAveragePosition2020; @zengReviewCollationGraphical2023].

## Use when all of these are true <!-- role: context -->

- **User Goal:** Estimate the average vertical position of one displayed series.
- **Task:** Recall that average after a brief view and short delay.
- **Data:** One quantitative series.
- **Chart Setting:** A single-series line or bar display, with no second graphed series in the same frame.
- **Audience:** Readers making remembered average-position judgments.
- **Success Criterion:** Smaller bias and tighter estimates of the series average.

## Do not use when any of these are true <!-- role: exceptions -->

- **Break it when:** the display contains a second graphed series in the same frame. **Why:** both lines and bars in compound displays still showed systematic bias plus perceptual pull, so the single-series bar-versus-line choice does not by itself solve the multi-series error.
- **Break it when:** readers are not estimating average position after a brief view and short delay. **Why:** the evidence here is limited to recalled average-position judgments.

## Costs of choosing bars here <!-- role: costs -->

**Sacrifice:** This choice reduces bias relative to a line, but it does not eliminate bias.
**Risk:** Readers can still overestimate the average position of bars.
**Mitigation:** Keep the display to one series and test the bar version with the same brief-view average-position judgment that the chart must support.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Choosing a line because position is assumed to be effectively unbiased. **Why it fails:** single lines were systematically underestimated in this task, and bars produced smaller bias with more precise judgments.

## How to test the choice <!-- role: check -->

**Failure Sign:** Readers place the remembered average lower in the line version than intended, or the line version yields larger absolute error than the bar version.
**Quick Check:** Build matched single-series line and bar versions, show each briefly, and ask readers to place the average position with the same response method; keep the version with smaller absolute error.
**Stronger Test:** Compare both average error and response spread across several target average positions before choosing the line version.

## What to change <!-- role: fix -->

- Replace the single line with a single set of bars when the chart’s job is recalled average-position estimation.
- Remove any second graphed series from the same frame before re-testing bar versus line.
- Re-run the brief-view average-position check and keep the bar version if it shows smaller absolute error.
