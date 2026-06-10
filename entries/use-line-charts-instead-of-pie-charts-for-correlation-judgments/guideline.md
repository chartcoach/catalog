---
id: use-line-charts-instead-of-pie-charts-for-correlation-judgments
title: Use line charts instead of pie charts for correlation judgments
bibliography: references.bib
description: For correlation judgments in small static two-dimensional displays, use
  a line chart instead of a pie chart on tabular data to improve fidelity and speed
  and mitigate weak association reading for readers judging whether two attributes
  move together.
labels:
- purpose:select
- basis:empirical
- task:relate
- chart:line:use
- chart:pie-donut:avoid
- quality:fidelity:use
- lever:chart-family
- operator:association
---

## Choose line over pie <!-- role: advice -->

Use a line chart when the main question is whether two attributes are strongly related. For example, replace a pie chart with a line chart when readers must decide whether values move together across displayed items.

## Why line works better here <!-- role: reason -->

A line chart exposes the overall relationship across plotted values, while a pie chart does not make that association easy to read. That changes both how quickly people can answer and how often they answer correctly.

**Mechanism:** A line chart supports relationship reading by showing how values vary together across the plotted sequence, while a pie chart asks readers to inspect slices rather than judge an overall association.

**Evidence:** In the controlled task comparison, line charts ranked above pie charts for correlation in accuracy, time, and user preference, and the later collation summarizes this study as recommending line charts for correlate tasks. [@saketTaskBasedEffectivenessBasic2019; @zengReviewCollationGraphical2023]

**Notes:** The tested setting used small static charts with 5-34 visual marks.

## Use when the task is relationship judgment <!-- role: context -->

- **User Goal:** Decide whether two displayed attributes are strongly related.
- **Task:** Correlation.
- **Data:** Tabular data shown in a small display with 5-34 marks.
- **Chart Setting:** Static two-dimensional chart.
- **Success Criterion:** Higher accuracy, faster answers, and stronger user preference.

## Do not use when the task changes to exact value reading <!-- role: exceptions -->

**Break it when:** the task changes from judging association to precisely identifying a specific value or computing a derived value. **Why:** line charts were among the weaker options when readers had to read exact values from specific points.

## Costs of switching from pie to line <!-- role: costs -->

**Sacrifice:** You give up the slice-based form of the pie chart.
**Risk:** A line chart can underperform when the main job is exact value lookup rather than relationship judgment.
**Mitigation:** Use the line chart only when correlation is the primary question.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keep a pie chart for a correlation question because it already shows the same categories. **Why it fails:** the pie chart was one of the least effective options for this task in both performance and preference.

## Check the task against the chart choice <!-- role: check -->

**Failure Sign:** Reviewers must answer a correlation question from a pie chart.
**Quick Check:** Render the same data as both a line chart and a pie chart and ask which version lets a reviewer judge the relationship faster.
**Stronger Test:** Time one correlation question on both versions and compare both errors and completion time.

## Fix the chart choice <!-- role: fix -->

- Replace the pie chart with a line chart when the question is about whether two attributes move together.
- Keep the same underlying data and redraw it as positions on shared axes rather than slices.
- If the current chart must stay for another purpose, add a separate line chart for the correlation question.
