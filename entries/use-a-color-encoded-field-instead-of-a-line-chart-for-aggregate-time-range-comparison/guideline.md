---
id: use-a-color-encoded-field-instead-of-a-line-chart-for-aggregate-time-range-comparison
title: Use a color-encoded field instead of a line chart for aggregate time-range
  comparison
bibliography: references.bib
description: For aggregate comparison in ordered time, prefer a color-encoded field
  over a line chart on single-series temporal displays to improve accuracy and address
  detail-by-detail reading for viewers making overview judgments.
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

## Choose a colorfield for aggregate range comparison <!-- role: advice -->

Use a color-encoded field instead of a line chart when readers need to compare averages across time ranges in a single series. For example, replace a single time-series line graph with a colorfield that maps value to color across the same ordered time axis when readers must pick the interval with the highest average.

## Why the colorfield works for this task <!-- role: reason -->

A color-encoded field supports interval-level reading as an overview task, while a line chart asks readers to inspect many individual positions and mentally combine them into range averages.

**Mechanism:** Mapping value to color across ordered time helps readers judge average level over a range more directly than summing many point heights from a line.

**Evidence:** In the collated experiment, the colorfield design ranked above the line chart for the aggregate task, and the accuracy difference was significant (ANOVA, p < .001) [@zengReviewCollationGraphical2023; @correllComparingAveragesTime2012].

**Notes:** The reported result is about accuracy on an aggregate judgment task, not about precise point lookup.

## Use when the chart must support range-level averaging <!-- role: context -->

- **User Goal:** Identify which time interval has the highest average value.
- **Task:** Compare aggregate values across fixed ranges within one ordered series.
- **Data:** One quantitative series laid out over ordered time with many values per interval.
- **Chart Setting:** Static single-view display of the same series.
- **Audience:** Viewers making an overview judgment from the chart.
- **Success Criterion:** Higher accuracy in choosing the correct interval.

## Do not use when the chart must support exact point reading <!-- role: exceptions -->

**Break it when:** The main task is reading exact individual values or inspecting detailed local patterns in the series. **Why:** The source positions the line graph as the standard display for detail-oriented reading, while the colorfield result is only supported for aggregate judgments.

## Tradeoffs of replacing the line chart <!-- role: costs -->

**Sacrifice:** You give up the position-based encoding used by the line chart.
**Risk:** The color-encoded field can be the wrong choice if readers need exact values rather than interval averages.
**Mitigation:** Keep the line chart when the task changes from range-level averaging to detailed value reading.

## Common failure mode in this decision <!-- role: mistakes -->

**Mistake:** Keeping a line chart for an average-over-ranges decision just because time series are conventionally shown as lines. **Why it fails:** The studied aggregate task was performed more accurately with the color-encoded field than with the line chart.

## Check the choice with a direct comparison task <!-- role: check -->

**Failure Sign:** Reviewers must visually trace many ups and downs in the line to decide which interval has the highest average.
**Quick Check:** Show the same series once as the current line chart and once as a color-encoded field, then ask which interval has the highest average.
**Stronger Test:** Run a small forced-choice test on matched series data and compare accuracy between the line chart and the color-encoded field.

## Fix the chart selection <!-- role: fix -->

- Replace the line chart with a color-encoded field for the aggregate comparison task.
- Keep the same ordered time axis so the compared intervals stay aligned.
- Encode the quantitative value with color across the full series instead of position alone.
- Switch back to a line chart if the task changes to precise point reading.
