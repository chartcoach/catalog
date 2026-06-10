---
id: use-radar-charts-instead-of-line-charts-for-positive-correlation
title: Use radar charts instead of line charts for positive correlation judgments
bibliography: references.bib
description: For association judgments, prefer radar charts over line charts on positively
  correlated quantitative series to improve fidelity and address weaker discrimination
  of correlation strength for people comparing relationship strength.
labels:
- purpose:select
- basis:empirical
- task:relate
- chart:radar:use
- chart:line:avoid
- quality:fidelity
- lever:chart-family
- operator:association
---

## Choose radar over line for positive relationships <!-- role: advice -->

Use a radar chart instead of a line chart when the relationship is positive and you are choosing between these two forms for correlation judgment. For example, if the same two quantitative series can be drawn either as a radar chart or as a line chart, choose the radar chart for comparing which positive correlation is stronger.

## Why the radar chart works better in this bounded contrast <!-- role: reason -->

The positive-correlation comparison favored radar charts over line charts. This was not presented as a general endorsement of radar charts, but as a measured win within this specific pair.

**Mechanism:** For positive relationships, the radar form gave viewers a more discriminable pattern for comparing correlation strength than the line-chart form.

**Evidence:** Radar charts depicting positive correlations significantly outperformed line charts depicting positive correlations in the paper's correlation-perception experiment and model fits [@harrisonRankingVisualizationsCorrelation2014].

**Notes:** The negative versions of these chart families were excluded from analysis, so this result should stay narrowly scoped to positive correlations.

## Use when the line-versus-radar choice is real and the sign is positive <!-- role: context -->

- **User Goal:** Help viewers rank which positive relationship is more strongly correlated.
- **Task:** Compare association strength rather than read exact values.
- **Data:** Two quantitative series with positive correlation.
- **Chart Setting:** The design choice is specifically between a radar chart and a line chart.
- **Success Criterion:** Viewers can more reliably identify the stronger positive correlation.

## Do not carry this contrast into the unsupported sign case <!-- role: exceptions -->

**Break it when:** The relationship to be judged is negative rather than positive. **Why:** Negative radar and negative line conditions were excluded from the analysis because judgments were unreliable, so the contrast was not supported there.

## Costs of changing chart family <!-- role: costs -->

**Sacrifice:** This is a narrow recommendation for one chart-family contrast and one sign condition.
**Risk:** Treating it as a general rule for all uses of radar and line charts can overgeneralize the result.
**Mitigation:** Apply it only when the task is judging positive correlation strength between these two options.

## Common failure mode in this comparison <!-- role: mistakes -->

**Mistake:** Reuse a line chart for positive-correlation judgment without testing the radar alternative. **Why it fails:** In this specific contrast, the line chart produced weaker correlation discrimination.

## How to test the choice <!-- role: check -->

**Failure Sign:** Reviewers struggle to decide which positive relationship is stronger in the line chart.
**Quick Check:** Render the same positive relationship as both a radar chart and a line chart, then ask which version makes the stronger correlation easier to identify.
**Stronger Test:** Use repeated paired comparisons of slightly different positive correlations and keep the chart family with more consistent correct choices.

## What to change <!-- role: fix -->

- Replace the positive-correlation line chart with a radar chart when these are the two candidate forms.
- A/B test the same positive data in both forms before standardizing the choice.
- Restrict this swap to positive-correlation judgments instead of applying it to negative cases.
