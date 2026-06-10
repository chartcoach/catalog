---
id: split-overlapping-time-series-into-small-multiples
title: Split overlapping time series into small multiples
bibliography: references.bib
description: For trend comparison over ordered time with many overlapping series,
  prefer a small-multiple layout on line charts to improve readability and mitigate
  spaghetti-line overlap for general audiences.
labels:
- purpose:select
- basis:heuristic
- task:trend
- time:ordered-time
- structure:small-multiples:use
- structure:single-view:avoid
- density:dense
- lever:layout-structure
- quality:readability
---

## Small-multiple line layout <!-- role: advice -->

Give each time series its own panel when many lines would overlap in one chart. For example, replace a single multi-line time chart that turns into a spaghetti monster with a grid of line charts, one line per category.

## Why separate panels help time-series comparison <!-- role: reason -->

Separate panels remove line overlap while keeping the same trend display for each category. Readers can follow each series without tracing through crossings and collisions in one crowded plot.

**Mechanism:** One line per panel reduces visual interference and keeps the time trend legible for each category.

**Evidence:** When lots of categories overlap in one time chart, giving each line its own little panel is recommended as a way to avoid the spaghetti-monster effect of a crowded multi-line chart [@muth_chart_types_guide_2025].

## Use when many time series overlap <!-- role: context -->

- **User Goal:** Compare how multiple categories changed over time.
- **Task:** Follow separate trends without losing track of individual series.
- **Data:** Ordered-time data with many categories whose lines would overlap heavily.
- **Chart Setting:** A time-series display where the single-view version is crowded.
- **Audience:** A mainstream audience.
- **Success Criterion:** Readers can trace each category's trend without line collisions obscuring it.

## Do not use when one chart is already clear <!-- role: exceptions -->

**Break it when:** You have only one or a few time series and the single line chart is already easy to read. **Why:** A standard line chart is already an intuitive and solid choice, so extra panels do not solve a real problem.

## Costs of splitting the chart <!-- role: costs -->

**Sacrifice:** You give up the single shared plotting area of one multi-line chart.\
**Risk:** The small-multiple version uses more space.\
**Mitigation:** Reserve the split layout for charts where the single-view version has become a spaghetti monster.

## Common failure with crowded line charts <!-- role: mistakes -->

**Mistake:** Keep all categories in one multi-line chart after the lines start overlapping heavily. **Why it fails:** Readers have trouble following individual series once the lines cross and pile up.

## Check whether the single-view chart has become a spaghetti monster <!-- role: check -->

**Failure Sign:** The lines overlap so much that individual categories are hard to trace.\
**Quick Check:** Compare a single-view multi-line draft with a small-multiple draft; if the first looks like a spaghetti monster and the second restores legibility, use small multiples.\
**Stronger Test:** Ask whether a reader can follow any chosen category from start to finish without losing it among other lines.

## Fix the overlap <!-- role: fix -->

- Split the chart into a grid of repeated line charts.
- Put one category in each panel instead of keeping all lines in one view.
- Replace the crowded single-view multi-line chart with a small-multiple layout.
