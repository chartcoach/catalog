---
id: use-shared-line-chart-for-same-date-comparisons
title: Use a shared line chart for same-date comparisons
bibliography: references.bib
description: For same-date comparison over ordered time, use single-view structure
  on multi-series line charts to improve fidelity and mitigate cross-panel comparison
  errors for readers judging which series is higher at a specific point.
labels:
- purpose:select
- basis:heuristic
- task:compare
- time:ordered-time
- structure:single-view:use
- structure:small-multiples:avoid
- quality:fidelity
- lever:layout-structure
---

## Use a shared plot for same-date comparisons <!-- role: advice -->

Put series back into one shared line chart when readers need to compare categories at a specific time point. For example, use a single-view line chart instead of separate panels when the key question is which series was higher in a given year.

## Why a shared plot helps point-by-point comparison <!-- role: reason -->

One shared plot preserves common vertical position at each date. Readers can then compare categories directly at the same time point.

**Mechanism:** A shared plotting area makes same-date height comparisons immediate across series, while separate panels break that direct comparison.

**Evidence:** Single-view line charts are recommended over small multiples when the reader needs to answer questions about which series was higher at a given time [@muth_small_multiple_line_charts_2024].

## Use when the question is which series is higher on one date <!-- role: context -->

- **User Goal:** Compare categories at one specific time point.
- **Task:** Decide which series is higher on the same date.
- **Data:** Multiple temporal series sharing the same dates.
- **Chart Setting:** Choosing between separate panels and one shared line chart.
- **Success Criterion:** A same-date higher/lower comparison is immediate.

## Do not use when overlap is the bigger problem <!-- role: exceptions -->

**Break it when:** Even a handful of lines overlap a lot or the main goal is to see each line's shape. **Why:** Overlapping lines can overwhelm readers and make each trend harder to parse.

## Costs of combining panels into one plot <!-- role: costs -->

**Sacrifice:** You give up the breathing room that separate panels provide.
**Risk:** The shared plot can become tangled if many lines cross.
**Mitigation:** Switch back to small multiples when trend shape matters more than same-date comparison.

## Common faceting mistake for comparison tasks <!-- role: mistakes -->

**Mistake:** Separate every series into its own panel when the task is a same-date comparison. **Why it fails:** The faceted layout hides which series is higher at that moment.

## Test the comparison task in both structures <!-- role: check -->

**Failure Sign:** A reader cannot answer a same-date higher/lower question from the faceted version.
**Quick Check:** Compare the faceted version against a single shared-axis line chart using one same-date question; if the shared plot answers it immediately, use the shared plot.
**Stronger Test:** Try several same-date lookups and see whether the answer depends on mentally jumping between panels.

## Edits that restore direct comparison <!-- role: fix -->

- Combine the separate panels into one shared plotting area.
- Keep the series on the same axes so same-date height comparisons are direct.
- If the merged plot becomes too tangled to read, switch back to small multiples for trend reading.
