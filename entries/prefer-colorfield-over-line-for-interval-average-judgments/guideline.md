---
id: prefer-colorfield-over-line-for-interval-average-judgments
title: Prefer a colorfield over a line chart for interval-average judgments
bibliography: references.bib
description: For overview comparison of averages across fixed intervals in ordered
  time series, prefer color encoding on a heatmap-like series display over a line
  chart to improve judgment fidelity and mitigate peak-finding errors for viewers
  summarizing dense data.
labels:
- purpose:select
- basis:empirical
- task:compare
- time:ordered-time
- chart:heatmap:use
- chart:line:avoid
- quality:fidelity:use
- lever:chart-family
---

## Choose the chart family for interval-average reading <!-- role: advice -->

Choose a colorfield when the job is to identify which interval in a time series has the highest average, and avoid relying on a line chart for that decision. For example, replace a daily line graph with a heatmap-like strip that maps each day to color when readers must compare monthly averages rather than read exact daily values.

## Why the colorfield works better here <!-- role: reason -->

A colorfield supports averaging over a region as a visual readout, while a line chart asks readers to judge an aggregate from a continuous shape. That makes the colorfield more effective when the question is about interval averages rather than individual peaks.

**Mechanism:** Encoding value with color lets readers pool many points within an interval as a summary, while encoding value with height makes the same judgment depend on estimating an overall shape.

**Evidence:** In a controlled study of ordered series where readers had to pick the interval with the highest average, colorfield displays significantly outperformed line graphs, and line graphs were more sensitive to close distractor averages and noise [@correllComparingAveragesTime2012].

## Use when the task is interval-level summary, not point lookup <!-- role: context -->

- **User Goal:** Pick which predefined interval has the highest average value.
- **Task:** Compare or rank averages across fixed intervals in one full series.
- **Data:** Ordered one-dimensional series with many points per interval and enough noise or close competitors that a single peak can mislead.
- **Chart Setting:** A single display shows the whole series and the interval boundaries at once.
- **Audience:** Viewers who can make a basic average judgment without domain-specific knowledge.
- **Success Criterion:** Higher accuracy in choosing the correct interval average.

## Do not replace the line chart when exact values are the main target <!-- role: exceptions -->

**Break it when:** Readers must retrieve precise individual values or inspect low-level temporal detail. **Why:** The paper notes that position encodings such as line graphs are more precise for detailed value reading, while the colorfield helps the summary task.

## Tradeoffs of switching to a colorfield <!-- role: costs -->

**Sacrifice:** You give up some precision for exact point-value reading.
**Risk:** Readers may lose detail about local ups and downs while focusing on the interval summary.
**Mitigation:** Use the colorfield only when the main question is about interval averages rather than exact daily values.

## Common failure mode: keeping the conventional line chart for a summary task <!-- role: mistakes -->

**Mistake:** Keeping a line chart because it is the standard time-series form even when the question is which interval averages highest. **Why it fails:** The tallest visible peak often does not belong to the interval with the highest average, and the line chart underperformed on this judgment.

## How to test the chart choice <!-- role: check -->

**Failure Sign:** Reviewers repeatedly choose the interval with the highest peak instead of the interval with the highest average.
**Quick Check:** Show the same representative dense series as both a line chart and a colorfield, then ask viewers to pick the highest-average interval under brief viewing.
**Stronger Test:** Include hard cases where the best interval is only slightly above distractors and the highest peak falls in a different interval.

## What to change <!-- role: fix -->

- Replace the line chart with a colorfield strip that maps each time point's value to color.
- Use the colorfield for full-series overview questions that ask readers to compare averages across fixed intervals.
- Validate the redesign on cases where the highest peak and the highest interval average occur in different intervals.
