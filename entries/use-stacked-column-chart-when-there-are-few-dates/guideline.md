---
id: use-stacked-column-chart-when-there-are-few-dates
title: Use a stacked column chart when there are fewer than about ten dates
bibliography: references.bib
description: For showing shares over ordered time with few dates, prefer a stacked
  column chart instead of an area chart to improve readability and mitigate hard labels
  and value reading for readers comparing several shares.
labels:
- purpose:select
- basis:heuristic
- task:trend
- time:ordered-time
- chart:bar:use
- chart:area:avoid
- quality:readability:use
- lever:chart-family
- density:sparse
---

## Switch to stacked columns <!-- role: advice -->

Use a stacked column chart instead of an area chart when you have fewer than about ten dates. For example, change a short series of stacked areas into stacked columns when you want clearer labels and easier value reading, especially with many shares or shares that vary a lot over time.

## Why short time series read better as columns <!-- role: reason -->

With only a few dates, the continuous area shape offers less benefit than the clearer discrete columns. Labels fit better, and readers can read values more easily.

**Mechanism:** The stacked column chart gives each date its own clearer vertical stack, which makes labels and value reading easier than tracing changing areas across a short time span.

**Evidence:** The source recommends considering a stacked column chart instead of an area chart when there are fewer than about ten dates, and notes that labeling and value reading are improved, especially with many shares and with shares that vary a lot over time [@muth_area_charts_2018].

## Use when the time series is short <!-- role: context -->

- **User Goal:** Show shares over time with a small number of dates.
- **Task:** Read values and labels across a short ordered sequence.
- **Data:** Temporal shares with fewer than about ten dates.
- **Chart Setting:** A stacked area chart is being considered for a short series.
- **Audience:** Readers who need to read labels and values easily.
- **Success Criterion:** The dates and shares are easy to label and read.

## Do not use when date gaps are uneven <!-- role: exceptions -->

**Break it when:** The intervals between dates differ. **Why:** A stacked column chart does not show unequal time gaps on a continuous scale, while an area chart can.

## What you give up <!-- role: costs -->

**Sacrifice:** You give up a continuous time axis.
**Risk:** Equal-width columns can imply equal time gaps even when the dates are not evenly spaced.
**Mitigation:** Keep the area chart when showing the true spacing between dates matters.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keeping a stacked area chart for a very short time series. **Why it fails:** The areas do not add enough benefit to offset the harder labels and harder value reading.

## How to test the choice <!-- role: check -->

**Failure Sign:** The chart has only a handful of dates, but labels and values are still hard to read in the area chart.
**Quick Check:** Make a stacked-column version and compare whether labels and values are easier to read.
**Stronger Test:** Verify that the dates are evenly spaced before choosing stacked columns over the area chart.

## What to change <!-- role: fix -->

- Replace the stacked areas with stacked columns.
- Recheck label placement and value reading in the column version.
- If the date intervals are uneven, revert to an area chart with a continuous time scale.
