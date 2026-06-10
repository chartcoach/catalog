---
id: use-bar-charts-instead-of-line-charts-for-cluster-detection
title: Use bar charts instead of line charts for cluster detection
bibliography: references.bib
description: For cluster detection in small static two-dimensional displays, use a
  bar chart instead of a line chart on tabular data to improve fidelity and speed
  and mitigate missed or ambiguous group structure for readers scanning for similar
  values.
labels:
- purpose:select
- basis:empirical
- chart:bar:use
- chart:line:avoid
- data:tabular
- quality:fidelity:use
- lever:chart-family
- density:sparse
---

## Choose bar over line <!-- role: advice -->

Use a bar chart when the main question is how many groups of similar values appear in the display. For example, replace a line chart with a bar chart when readers must count clusters rather than follow a trend.

## Why bar works better here <!-- role: reason -->

A bar chart makes separate groups easier to scan as distinct magnitudes, while a line chart emphasizes connection across points. That helps readers detect and count groups more accurately and with less time.

**Mechanism:** Bar marks support scanning for separated groups of similar values, while connecting those values with a line can pull attention toward continuity instead of grouping.

**Evidence:** In the experiment, bar charts ranked above line charts for cluster tasks in accuracy, time, and user preference, and the later collation summarizes this study as recommending bar charts for cluster tasks. [@saketTaskBasedEffectivenessBasic2019; @zengReviewCollationGraphical2023]

**Notes:** The tested displays were static and used 5-34 marks.

## Use when the task is group finding <!-- role: context -->

- **User Goal:** Count or detect groups of similar values.
- **Data:** Tabular data shown as a small static display.
- **Chart Setting:** Two-dimensional chart with 5-34 marks.
- **Success Criterion:** Better accuracy and faster cluster finding, with stronger user preference.

## Do not use when the task changes to correlation <!-- role: exceptions -->

**Break it when:** the task changes from finding groups to judging whether two attributes are correlated. **Why:** line charts were among the strongest options for correlation, while bar charts were not the top choice there.

## Costs of switching from line to bar <!-- role: costs -->

**Sacrifice:** You give up the connected trend emphasis of the line chart.
**Risk:** Using a bar chart by default can hide that the reader's real question is about relationship rather than grouping.
**Mitigation:** Switch only when the primary question is cluster detection.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Use a line chart for cluster detection because the categories are ordered. **Why it fails:** the connecting line can foreground continuity even when the task is to count separate groups.

## Check the task against the chart choice <!-- role: check -->

**Failure Sign:** Reviewers must count groups or spot clusters from a line chart.
**Quick Check:** Render the same values as both a bar chart and a line chart and see which version makes group counting easier on a sample question.
**Stronger Test:** Time one cluster question on both versions and compare both answer errors and response time.

## Fix the chart choice <!-- role: fix -->

- Replace the line chart with a bar chart when the question is how many groups are present.
- Keep the same summarized values and redraw them as separate bars instead of connected points.
- If the line chart is needed for another task, present a separate bar chart for the clustering question.
