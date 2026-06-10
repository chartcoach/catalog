---
id: use-area-chart-for-uneven-time-intervals
title: Use an area chart when time intervals are uneven
bibliography: references.bib
description: For ordered-time part-to-whole reading with irregular date spacing, use
  an area chart instead of stacked columns to improve temporal fidelity and mitigate
  incorrect equal-spacing cues for readers interpreting time intervals.
labels:
- purpose:select
- basis:heuristic
- time:ordered-time
- chart:area:use
- chart:bar:avoid
- operator:part-whole
- quality:fidelity
- lever:chart-family
---

## Switch to an area chart <!-- role: advice -->

Replace stacked columns with an area chart when the dates are not evenly spaced. For example, use an area chart with a continuous x-axis for irregular dates instead of equal-width columns that imply the same interval between every time point.

## Why uneven dates need continuous spacing <!-- role: reason -->

A stacked column chart spaces dates as separate categories, so unequal intervals look equal. An area chart can place dates on a continuous scale and show the spacing correctly.

**Mechanism:** The continuous x-axis preserves the real distance between dates, so readers do not misread irregular intervals as evenly spaced steps.

**Evidence:** The post says stacked column charts for time data should use dates with the same intervals, and recommends an area chart when intervals differ because continuous scales show the date intervals correctly [@muth_stacked_columns_2018].

## Use when date spacing varies <!-- role: context -->

- **User Goal:** Show totals and shares over time without distorting the spacing between dates.
- **Task:** Preserve the actual timing of changes.
- **Data:** Part-to-whole time data with irregular intervals between dates.
- **Chart Setting:** The choice is between stacked columns and an area chart.
- **Audience:** Readers need to interpret the timing correctly from the axis.
- **Success Criterion:** The x-axis reflects the real interval between dates.

## Do not use when the dates are evenly spaced and few <!-- role: exceptions -->

**Break it when:** The dates are evenly spaced and there are only a few of them. **Why:** In that case stacked columns can make the parts easier to compare across dates.

## What you give up <!-- role: costs -->

**Sacrifice:** You give up the discrete column form.
**Risk:** Readers may find the parts harder to compare than in a small set of stacked columns.
**Mitigation:** Use the area chart only when correct time spacing matters.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Using equal-width stacked columns for irregular dates. **Why it fails:** The chart suggests equal time gaps that the data do not have.

## Test the chart choice <!-- role: check -->

**Failure Sign:** Uneven dates appear with identical spacing on the x-axis.
**Quick Check:** Mock the same data as stacked columns and as an area chart; if the column version forces equal spacing between unequal dates, use the area chart.
**Stronger Test:** Inspect the x-axis; if the dates require a continuous scale, stacked columns are the wrong choice.

## Revise the design <!-- role: fix -->

- Replace the stacked columns with an area chart.
- Put the dates on a continuous x-axis.
- Keep the real interval between dates visible in the final chart.
