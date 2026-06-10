---
id: use-tables-instead-of-line-charts-for-exact-value-lookup
title: Use tables instead of line charts for exact value lookup
bibliography: references.bib
description: For exact value lookup in small static two-dimensional displays, use
  a table instead of a line chart on tabular data to improve fidelity and speed and
  mitigate imprecise point reading for readers identifying specific values.
labels:
- purpose:select
- basis:empirical
- task:retrieve
- chart:table:use
- chart:line:avoid
- quality:fidelity:use
- lever:chart-family
- operator:lookup
- reading-mode:exact
---

## Choose table over line <!-- role: advice -->

Use a table when the main question is the exact value of a specific item. For example, replace a line chart with a table when readers must look up a precise value instead of infer it from point positions and axis ticks.

## Why table works better here <!-- role: reason -->

A table presents the value directly, while a line chart can force interpolation from positions and ticks. That improves both exactness and speed for lookup tasks.

**Mechanism:** Tables remove the need to estimate a value from a plotted point, so readers can read the requested value directly instead of inferring it from the chart scale.

**Evidence:** In the experiment, tables ranked above line charts for retrieve-value tasks in accuracy, time, and user preference, and the paper explicitly warned against line charts for tasks that require precise identification of a specific data-point value; the later review includes this study among the evidence used for retrieve-value recommendations. [@saketTaskBasedEffectivenessBasic2019; @zengReviewCollationGraphical2023]

**Notes:** The paper linked line-chart underperformance on exact-value tasks to reading values from interval ticks.

## Use when the task is exact lookup <!-- role: context -->

- **User Goal:** Read the exact value for a specified item.
- **Task:** Retrieve value.
- **Data:** Tabular data shown in a small static display with 5-34 marks.
- **Chart Setting:** Two-dimensional display without interaction.
- **Success Criterion:** Higher lookup accuracy, faster reading, and stronger user preference.

## Do not use when the task changes to correlation <!-- role: exceptions -->

**Break it when:** the task changes from exact lookup to judging correlation. **Why:** line charts were among the strongest options for correlation, so replacing them with tables can remove the stronger association view.

## Costs of switching from line to table <!-- role: costs -->

**Sacrifice:** You give up the continuous trend view of the line chart.
**Risk:** A table can be a weaker choice when the task is to see a relationship or overall pattern rather than read one value exactly.
**Mitigation:** Switch only when exact value lookup is the primary task.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keep a line chart for exact lookup because the point is already plotted. **Why it fails:** the reader still has to estimate the value from the axis rather than read it directly.

## Check the task against the chart choice <!-- role: check -->

**Failure Sign:** Reviewers must answer a precise value question from a line chart.
**Quick Check:** Compare the same question on a table and a line chart and see whether the line version requires interpolation from the scale.
**Stronger Test:** Time one exact-value question on both versions and compare both answer errors and completion time.

## Fix the chart choice <!-- role: fix -->

- Replace the line chart with a table when the question asks for a specific exact value.
- Present the requested values directly in cells instead of asking readers to read them from plotted positions.
- If the line chart is still needed for another task, add a table alongside it for the lookup task.
