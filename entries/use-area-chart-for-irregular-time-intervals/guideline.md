---
id: use-area-chart-for-irregular-time-intervals
title: Use an area chart when time intervals between dates are irregular
bibliography: references.bib
description: For showing shares over ordered time, use an area chart instead of a
  stacked column chart on irregularly spaced dates to improve fidelity and mitigate
  incorrect spacing of time points for readers interpreting elapsed time.
labels:
- purpose:select
- basis:heuristic
- time:ordered-time
- chart:area:use
- chart:bar:avoid
- quality:fidelity:use
- lever:chart-family
- data:temporal
---

## Keep a continuous time axis <!-- role: advice -->

Use an area chart instead of a stacked column chart when the gaps between dates are not equal. For example, keep the data on a continuous time axis when some date gaps span a few years and others span decades.

## Why the area chart is more faithful here <!-- role: reason -->

Irregular date gaps need a continuous scale to show elapsed time correctly. Equal-width columns do not preserve those unequal intervals.

**Mechanism:** The area chart can place dates at their true positions on a continuous axis, so readers see the real spacing between time points.

**Evidence:** The source gives unequal year intervals as a reason to use an area chart instead of a stacked column chart, because area charts have continuous scales that show dates in the right intervals while column charts do not [@muth_area_charts_2018].

## Use when date spacing matters <!-- role: context -->

- **User Goal:** Show shares over time while preserving the true spacing between dates.
- **Task:** Read change across uneven time intervals.
- **Data:** Temporal values with irregular gaps between dates.
- **Chart Setting:** A stacked column chart is being considered for a short time series with uneven spacing.
- **Audience:** Readers who should interpret elapsed time correctly.
- **Success Criterion:** The chart shows unequal intervals at unequal distances.

## Do not use when dates are few and evenly spaced <!-- role: exceptions -->

**Break it when:** The dates are few and evenly spaced. **Why:** A stacked column chart can then improve labeling and value reading.

## What you give up <!-- role: costs -->

**Sacrifice:** You give up some of the labeling ease of stacked columns.
**Risk:** With only a few evenly spaced dates, the area chart can be harder to read than a stacked column chart.
**Mitigation:** Switch to stacked columns when spacing is even and label readability is the bigger need.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Using equal-width stacked columns for dates that are not equally spaced. **Why it fails:** The chart suggests equal time gaps where the data do not have them.

## How to test the choice <!-- role: check -->

**Failure Sign:** The draft column chart gives the same visual width to unequal date gaps.
**Quick Check:** Compare the column chart with an area chart on a continuous axis; if the spacing changes, keep the area chart.
**Stronger Test:** Inspect the actual date intervals before choosing the chart type.

## What to change <!-- role: fix -->

- Move the data to an area chart with a continuous time axis.
- Position dates according to their actual intervals.
- Avoid equal-width stacked columns when the time gaps are unequal.
