---
id: prefer-bars-over-lines-for-delayed-average-position-judgments
title: Prefer bars over lines for delayed average-position judgments
bibliography: references.bib
description: For average-position reports after a short delay, prefer bar charts over
  line charts on single-series quantitative displays to improve fidelity and mitigate
  systematic position bias for readers reproducing a series' average level from memory.
labels:
- purpose:select
- basis:empirical
- chart:bar:use
- chart:line:avoid
- lever:chart-family
- measure:single
- quality:fidelity:use
---

## Chart family for average-level recall <!-- role: advice -->

Use a bar chart instead of a line chart when the main readout is a single series' average vertical position after brief viewing. For example, replace a single line with a single set of bars when readers must reproduce the series' average height after a short delay, and choose the bar version over the line version when both are otherwise viable.

## Why bars reduce this error <!-- role: reason -->

Average-position reports from a single series were biased in both chart families, but the line version pushed estimates downward more than the bar version pushed them upward. Choosing bars does not remove bias, but it reduces the distortion and improves precision relative to lines for this specific readout.

**Mechanism:** The chart family changes how viewers encode and later reproduce the series' overall vertical level, so the same average can be remembered as too low in a line chart and less inaccurately in a bar chart.

**Evidence:** Across controlled experiments, average line positions were systematically underestimated, average bar positions were systematically overestimated, and the authors conclude that bias was smaller and judgments were more precise for bars than for lines, recommending bars when other constraints do not dominate [@xiongBiasedAveragePosition2020].

**Notes:** This guidance is about average-position reports after a short delay, not about all possible tasks on line and bar charts.

## When to use this choice <!-- role: context -->

- **User Goal:** Reproduce one series' average vertical position as accurately as possible.
- **Task:** Judge the series briefly, then report its average level from memory.
- **Data:** One quantitative series.
- **Chart Setting:** A single-series display where either a line chart or a bar chart is still possible.
- **Audience:** Readers making memory-based average-position judgments.
- **Success Criterion:** Smaller systematic bias and tighter spread in reproduced average positions.

## When not to use this choice <!-- role: exceptions -->

**Break it when:** The task is not a delayed average-position report for a single series. **Why:** The paper only establishes this chart-family preference for average-position judgments after brief viewing and a short delay.

## What this choice costs <!-- role: costs -->

**Sacrifice:** This rule changes the chart family to reduce bias for one readout, not to eliminate bias entirely.
**Risk:** Treating bars as unbiased can still leave systematic error, because bar averages were also overestimated.
**Mitigation:** Use this as a bias-reduction choice, then test the chosen bar version with the target average-position task.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Switch from a line to bars and assume the problem is solved. **Why it fails:** The bar version still produces systematic error; it is only less biased and more precise than the line version in the tested task.

## How to test the choice <!-- role: check -->

**Failure Sign:** Readers place the remembered average level lower from the line version than from the bar version.
**Quick Check:** Mock the same single series as both a line chart and a bar chart, show each briefly, add a short delay, and ask readers to place the average height; keep the bar version if its error is smaller.
**Stronger Test:** Repeat the comparison across several low, medium, and high average positions and compare both signed error and spread.

## How to fix a failing chart <!-- role: fix -->

- Convert the single line series to a bar series when the key judgment is average level after brief viewing.
- Re-run the same delayed average-position check on the bar version before release.
- If the line form must stay, treat average-position readouts from that chart as high-risk and validate them explicitly.
