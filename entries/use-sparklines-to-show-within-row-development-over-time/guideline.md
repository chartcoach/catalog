---
id: use-sparklines-to-show-within-row-development-over-time
title: Use sparklines to show within-row development over time
bibliography: references.bib
description: For trend tasks in ordered-time table columns, use sparklines on tables
  to improve trend recognition and mitigate reliance on only two or three timepoints
  for readers scanning row-by-row changes.
labels:
- purpose:refine
- basis:heuristic
- chart:table
- task:trend
- time:ordered-time
- quality:insight
- lever:encoding
---

## Within-row trend lines <!-- role: advice -->

Replace a small set of separate timepoint columns with a sparkline when the goal is to show development over time. For example, use a mini line chart to show the path between years instead of listing only two or three dates as separate columns.

## Why sparklines help trend reading <!-- role: reason -->

A sparkline shows the direction of change that separate endpoints can hide.

**Mechanism:** Sparklines summarize the in-between path in very little space, so readers can see whether a row rose, fell, or fluctuated instead of inferring trend from just a few isolated timepoints.

**Evidence:** The post recommends showing development over time with sparklines rather than only two or three time points, while noting that each sparkline typically has its own y-axis range and therefore shows a general trend rather than a directly comparable scale [@muth_tables_2019].

## Use when a row needs a compact trend summary <!-- role: context -->

- **User Goal:** See how each row changed over time.
- **Task:** Trend reading within a table row.
- **Data:** Ordered time values currently shown in only a few separate columns.
- **Chart Setting:** Space is limited and the table format is staying in place.
- **Success Criterion:** Readers can see the general trend for each row at a glance.

## Do not use when common scale comparison is required <!-- role: exceptions -->

**Break it when:** A consistent y-axis range across rows is important. **Why:** The post says default sparkline ranges differ by row, so they are not comparable with each other.

## Tradeoffs of sparklines <!-- role: costs -->

**Sacrifice:** You give up direct cross-row scale comparability.\
**Risk:** Readers may compare lines that were scaled differently.\
**Mitigation:** Use a line chart instead when a common y-axis range is important.

## Common sparkline mistake <!-- role: mistakes -->

**Mistake:** Using sparklines when readers need exact cross-row comparison on the same scale. **Why it fails:** The lines show only general trends when each row uses a different range.

## Check whether a sparkline is the right time display <!-- role: check -->

**Failure Sign:** Readers need to compare heights or slopes across rows as if they shared one scale.\
**Quick Check:** Inspect whether each row's sparkline uses its own y-axis range.\
**Stronger Test:** If a common range is required, replace the sparkline view with a line chart.

## Fix the time display <!-- role: fix -->

- Replace separate timepoint columns with a sparkline when the goal is compact trend display.
- Treat the sparkline as a general trend cue, not a shared-scale comparison.
- Switch to a line chart if readers need a consistent y-axis range across rows.
