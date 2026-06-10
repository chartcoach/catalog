---
id: use-stacked-columns-for-a-few-evenly-spaced-dates-when-totals-matter
title: Use stacked columns for a few evenly spaced dates when totals matter
bibliography: references.bib
description: For ordered-time part-to-whole reading across a few evenly spaced dates,
  use stacked columns instead of an area chart when the total is crucial to improve
  readability and mitigate harder part comparisons for readers comparing totals and
  shares together.
labels:
- purpose:select
- basis:heuristic
- time:ordered-time
- chart:bar:use
- chart:area:avoid
- operator:part-whole
- density:sparse
- quality:readability
- lever:chart-family
---

## Choose stacked columns for sparse dated totals <!-- role: advice -->

Choose stacked columns instead of an area chart when you have only a few evenly spaced dates and the total of the parts is crucial. For example, use columns for a small set of dates so readers can compare both total height and individual parts more easily than in an area chart.

## Why the discrete columns help with few dates <!-- role: reason -->

With only a small number of dates, the discrete stacks keep each total separate and make the parts easier to compare than in an area chart, while still showing the total.

**Mechanism:** The chart gives readers clear total heights and clearer part segments at each date, which helps when both totals and shares matter.

**Evidence:** The post says stacked column charts can work well for dates when the total is crucial, and that stacked columns are a better choice than area charts when there are only a few dates because readers can compare the parts more easily [@muth_stacked_columns_2018].

## Use when dates are few and evenly spaced <!-- role: context -->

- **User Goal:** Show totals and their shares at several dates.
- **Task:** Compare both total size and part size across dates.
- **Data:** Time data with equal intervals between dates and only a few date positions.
- **Chart Setting:** The choice is between stacked columns and an area chart.
- **Audience:** Readers need to compare separate dates rather than read a continuous flow.
- **Success Criterion:** Readers can see the total and compare the parts at each date.

## Do not use when date spacing is irregular <!-- role: exceptions -->

**Break it when:** The intervals between dates are different. **Why:** Then the area chart's continuous x-axis is needed to show the spacing correctly.

## What you give up <!-- role: costs -->

**Sacrifice:** You give up the continuous time-axis feel of an area chart.
**Risk:** If the dates are not evenly spaced, the columns will suggest the wrong interval structure.
**Mitigation:** Keep this choice to a small set of evenly spaced dates.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Using an area chart for a small set of evenly spaced dates when readers need to compare individual parts at each date. **Why it fails:** The parts are harder to compare than in stacked columns.

## Test the chart choice <!-- role: check -->

**Failure Sign:** The chart needs both total comparison and part comparison across only a few dates.
**Quick Check:** Mock the data as both stacked columns and an area chart; if the parts are easier to compare in the column version, use stacked columns.
**Stronger Test:** Verify that the dates share the same interval before keeping the column form.

## Revise the design <!-- role: fix -->

- Replace the area chart with stacked columns for the few dated totals.
- Keep the dates at equal intervals.
- Use the stacked totals only when the total height is part of the message.
