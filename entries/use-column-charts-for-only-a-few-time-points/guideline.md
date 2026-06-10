---
id: use-column-charts-for-only-a-few-time-points
title: Use a column chart for only a few time points
bibliography: references.bib
description: For showing ordered-time data with only a few time points, prefer a column
  chart over a line chart to improve readability and address sparse point-in-time
  comparisons for general audiences.
labels:
- purpose:select
- basis:heuristic
- task:trend
- time:ordered-time
- chart:bar:use
- chart:line:avoid
- lever:chart-family
- quality:readability
---

## Column chart for sparse time points <!-- role: advice -->

Choose a column chart when the time series contains only a few dates. For example, show values for the past five years with columns rather than drawing a line through just a handful of points.

## Why columns work better for a short run of dates <!-- role: reason -->

A few time points read more like a set of discrete comparisons than a continuous development. A column chart fits that sparse structure directly.

**Mechanism:** Columns emphasize each observed time point as its own value instead of implying a longer continuous path.

**Evidence:** For just a few points in time, a column chart is presented as the usual good fit, while line charts are introduced as the classic choice for showing how values changed over months or years [@muth_chart_types_guide_2025].

## Use when the timeline is short <!-- role: context -->

- **User Goal:** Show how a value changed across a short run of dates.
- **Task:** Compare a few observed time points.
- **Data:** Ordered-time data with only a small number of dates.
- **Chart Setting:** A simple time chart for a mainstream audience.
- **Audience:** A mainstream audience.
- **Success Criterion:** Each time point is easy to compare without a sparse line doing unnecessary work.

## Do not use when the development across many dates matters <!-- role: exceptions -->

**Break it when:** The chart covers months or years with enough dates that the evolution of the line itself is important. **Why:** A line chart is the classic intuitive choice for showing how values changed over longer time spans.

## Costs of switching to columns <!-- role: costs -->

**Sacrifice:** You give up the continuous path that a line chart shows.\
**Risk:** If there are many dates, columns can stop fitting the time sequence well.\
**Mitigation:** Use columns only when the time series really has just a few points.

## Common failure with short time series <!-- role: mistakes -->

**Mistake:** Draw a line chart for a very short series of dates just because the data is temporal. **Why it fails:** The chart adds a connected line where readers mainly need to compare a small set of separate time points.

## Check whether the line is doing useful work <!-- role: check -->

**Failure Sign:** The chart contains only a handful of dates, and the connected line adds little beyond linking sparse points.\
**Quick Check:** Compare a column version and a line version of the same short series; if the columns make the few time points easier to compare, keep the column chart.\
**Stronger Test:** Ask whether the chart's message depends on the path between many dates or simply on the values at a few dates.

## Fix the sparse time series display <!-- role: fix -->

- Replace the line chart with a column chart.
- Keep one column per time point.
- Use the line chart only if the series extends across enough dates that the development between them matters.
