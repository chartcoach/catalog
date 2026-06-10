---
id: split-overlapping-line-series-into-small-multiples
title: Split overlapping time series into small-multiple panels
bibliography: references.bib
description: For trend reading over ordered time, use small-multiple structure on
  multi-series line charts with overlapping lines to improve readability and mitigate
  line-crossing confusion for readers scanning each category separately.
labels:
- purpose:select
- basis:heuristic
- task:trend
- time:ordered-time
- structure:small-multiples:use
- structure:single-view:avoid
- quality:readability
- lever:layout-structure
---

## Panelize overlapping series <!-- role: advice -->

Split overlapping series into one panel per line when the goal is to read each trend clearly over time. For example, replace one shared line chart with a small-multiple line chart when even a handful of lines cross heavily or when readers need to see each line's shape and pace of change.

## Why separate panels improve trend reading <!-- role: reason -->

Separate panels remove the need to trace one line through crossings and let readers judge each series on its own. That makes the direction and volatility of each trend easier to see.

**Mechanism:** Readers inspect one line at a time instead of untangling an overlaid bundle, so the shape of each series becomes legible.

**Evidence:** Small-multiple line charts are recommended when overlapping lines need untangling and when the main goal is to show the shape, pace, and up-and-down movement of each category's trend [@muth_small_multiple_line_charts_2024].

**Notes:** This can be worthwhile even with only a handful of lines if they overlap a lot.

## Use when overlap hides the trend shape <!-- role: context -->

- **User Goal:** Read each category's trend shape over time.
- **Data:** Multiple temporal series that overlap in one shared plot.
- **Chart Setting:** Deciding between one overlaid line chart and one panel per series.
- **Success Criterion:** Each line can be followed without disentangling crossings.

## Do not use when same-date comparison is the main job <!-- role: exceptions -->

**Break it when:** Readers need to compare lines with each other at a specific point in time. **Why:** Separate panels make it hard to see which series is higher on the same date.

## Costs of splitting the lines into panels <!-- role: costs -->

**Sacrifice:** You give up direct same-date height comparison across series.
**Risk:** Readers may no longer be able to answer a higher-versus-lower question at one time point quickly.
**Mitigation:** Keep or return to a shared plot if the main question becomes same-date comparison.

## Common overlap mistake <!-- role: mistakes -->

**Mistake:** Keep adding lines to one shared plot because there are only a few of them. **Why it fails:** Even a handful of lines can overlap enough to overwhelm readers and hide each trend.

## Compare both layouts before choosing <!-- role: check -->

**Failure Sign:** Readers must trace through crossings to follow a single line.
**Quick Check:** Mock up the same data as separate panels and as one shared plot; if the panelized version makes each line's shape readable without disentangling overlap, choose small multiples.
**Stronger Test:** Compare which version better shows how quickly and how much each category rises and falls.

## Edits that move an overlaid chart to small multiples <!-- role: fix -->

- Create one panel per series instead of overlaying all series in one plot.
- Keep the time axis aligned across panels so each series still reads over the same period.
- If the main question shifts to which series is higher on one date, revert to one shared plot.
