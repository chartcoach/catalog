---
id: use-line-chart-for-a-single-value-over-time
title: Use a line chart for a single value over time
bibliography: references.bib
description: For showing one value over ordered time, prefer a line chart instead
  of an area chart to improve readability and mitigate an unnecessary zero-baseline
  requirement for readers following the trend.
labels:
- purpose:select
- basis:heuristic
- task:trend
- time:ordered-time
- chart:line:use
- chart:area:avoid
- quality:readability:use
- lever:chart-family
- measure:single
---

## Switch to a line chart <!-- role: advice -->

Use a line chart instead of an area chart when you are showing only one value over time. For example, remove the fill from a single time series and keep a line, especially when you do not want the y-axis to start at zero.

## Why a single series does not need an area <!-- role: reason -->

A single filled area adds little that a line does not already show. The line keeps the trend readable without imposing an area-chart treatment that is harder to label and often tied to a zero baseline.

**Mechanism:** The line chart keeps attention on the one changing value and avoids the extra area encoding that does not help the reader with a single series.

**Evidence:** The source recommends considering a line chart instead of an area chart when showing one value over time, especially if the y-axis should not start at zero [@muth_area_charts_2018].

## Use when there is only one series <!-- role: context -->

- **User Goal:** Show how one value changes over time.
- **Task:** Follow a single trend.
- **Data:** One temporal series.
- **Chart Setting:** A single-series area chart is being considered.
- **Audience:** Readers who need a straightforward reading of the trend.
- **Success Criterion:** The single trend is readable without unnecessary fill.

## Do not use when the series has only a few dates <!-- role: exceptions -->

**Break it when:** There are only a few dates. **Why:** The source says a column chart can also be a better choice in that case because labeling will be better.

## What you give up <!-- role: costs -->

**Sacrifice:** You give up the filled shape under the line.
**Risk:** With only a few dates, the line chart may not label as well as a column chart.
**Mitigation:** Switch to columns when the time series is very short.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Using a filled area for a single time series by default. **Why it fails:** The extra fill does not add much, and it can force a less flexible y-axis treatment.

## How to test the choice <!-- role: check -->

**Failure Sign:** The chart contains only one temporal series but still uses a filled area.
**Quick Check:** Make a line-chart version and compare whether the trend reads just as well or better.
**Stronger Test:** If you want a y-axis that does not start at zero, reject the area chart.

## What to change <!-- role: fix -->

- Remove the fill and keep the series as a line.
- If the series has only a few dates, try a column chart instead.
- Keep the area form only if the filled shape itself is essential to the message.
