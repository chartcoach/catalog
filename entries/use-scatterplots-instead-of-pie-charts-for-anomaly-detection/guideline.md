---
id: use-scatterplots-instead-of-pie-charts-for-anomaly-detection
title: Use scatterplots instead of pie charts for anomaly detection
bibliography: references.bib
description: For anomaly detection in small static two-dimensional displays, use a
  scatterplot instead of a pie chart on tabular data to improve insight and accuracy
  and mitigate missed outliers for readers scanning for abnormal values.
labels:
- purpose:select
- basis:empirical
- chart:scatter:use
- chart:pie-donut:avoid
- data:tabular
- quality:insight:use
- lever:chart-family
- reading-mode:overview
---

## Choose scatter over pie <!-- role: advice -->

Use a scatterplot when the main question is whether any displayed value looks abnormal. For example, replace a pie chart with a scatterplot when readers must spot an outlying point rather than compare slices.

## Why scatter works better here <!-- role: reason -->

A scatterplot exposes individual points and makes unusual positions easier to notice. A pie chart organizes the display around slices, which makes abnormal observations harder to isolate.

**Mechanism:** Point positions in a scatterplot let readers scan for values that break the visible pattern, while a pie chart centers attention on wedge sizes instead of outlying cases.

**Evidence:** In the experiment, scatterplots ranked above pie charts for anomaly detection in accuracy and user preference, and the later review summarizes this study as recommending scatterplots for find-anomalies tasks. [@saketTaskBasedEffectivenessBasic2019; @zengReviewCollationGraphical2023]

**Notes:** The paper's own summary recommendation for this task was to use scatterplots.

## Use when the task is spotting abnormal values <!-- role: context -->

- **User Goal:** Identify whether one or more displayed values are abnormal.
- **Task:** Find anomalies.
- **Data:** Tabular data shown in a small display with 5-34 marks.
- **Chart Setting:** Static two-dimensional chart.
- **Success Criterion:** Higher anomaly-detection accuracy with a chart people prefer to use.

## Do not use when the task changes to part comparison or exact lookup <!-- role: exceptions -->

**Break it when:** the task changes from spotting abnormal points to reading exact values or making other non-anomaly judgments such as retrieve-value tasks. **Why:** the study did not show scatterplots as the strongest option for exact lookup, and other chart types performed better there.

## Costs of switching from pie to scatter <!-- role: costs -->

**Sacrifice:** You give up the pie chart's slice-based presentation.
**Risk:** A scatterplot is not automatically the best choice for every task on the same data.
**Mitigation:** Use the scatterplot when finding anomalies is the main question, not just one possible secondary read.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keep a pie chart for anomaly detection because it already separates categories into slices. **Why it fails:** slice comparison does not make abnormal observations as visible as point positions do.

## Check the task against the chart choice <!-- role: check -->

**Failure Sign:** Reviewers must find an abnormal value from a pie chart.
**Quick Check:** Render the same data as both a scatterplot and a pie chart and ask which version makes the abnormal case easier to spot.
**Stronger Test:** Run one anomaly question on both versions and compare which chart produces fewer missed anomalies.

## Fix the chart choice <!-- role: fix -->

- Replace the pie chart with a scatterplot when the goal is to find abnormal values.
- Redraw the same observations as individual points so unusual positions can stand out.
- If the pie chart must stay for another purpose, add a separate scatterplot for anomaly finding.
