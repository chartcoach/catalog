---
id: use-a-single-24-hour-linear-bar-chart-for-am-pm-interval-comparisons
title: Use a single 24-hour linear bar chart for AM and PM interval comparisons
bibliography: references.bib
description: For exact paired AM/PM comparison in cyclic-time hourly data, use a single-view
  structure on linear bar charts to improve fidelity and mitigate underestimation
  of small value differences for non-expert readers.
labels:
- purpose:select
- basis:empirical
- task:compare
- time:cyclic-time
- chart:bar
- structure:single-view:use
- structure:multi-view:avoid
- quality:fidelity
- lever:layout-structure
- operator:difference
---

## Compare AM and PM on one bar axis <!-- role: advice -->

Use a single 24-hour linear bar chart when readers must compare the same hour in AM and PM. For example, place all 24 hourly bars on one continuous axis instead of asking readers to compare matched hours across separate 12-hour AM and PM panels.

## Why one axis helps comparison <!-- role: reason -->

A single linear view keeps the whole day in one structure, so readers do not have to switch between panels before judging the difference. Split panels can make small differences feel equal or smaller than they are.

**Mechanism:** One continuous axis reduces cross-panel lookup and supports more direct difference judgment between matched hours.

**Evidence:** For paired AM/PM interval comparison, the 24-hour linear bar chart was the fastest condition, while split charts showed errors where readers answered “same” for small nonzero differences and the paper reports a tendency for separated charts to underestimate value differences [@waldnerComparisonRadialLinear2020; @zengReviewCollationGraphical2023].

## Use when paired hourly differences matter <!-- role: context -->

- **User Goal:** Judge whether the same hour in AM and PM is lower, equal, or higher.
- **Task:** Compare paired hourly values.
- **Data:** One value per hour across a 24-hour cycle.
- **Chart Setting:** Linear bar chart available either as one 24-hour view or as separate AM/PM panels.
- **Audience:** Non-expert readers.
- **Success Criterion:** Fast comparison with fewer missed or underestimated differences.

## When to break the rule <!-- role: exceptions -->

**Break it when:** The available width cannot support a readable 24-hour linear bar chart. **Why:** The supported fallback is a split linear bar chart, not a radial chart.

## What you trade away <!-- role: costs -->

**Sacrifice:** You lose the explicit AM/PM panel boundary that separates the day into two chunks.
**Risk:** If the chart becomes too narrow, the 24-hour view can get cramped.
**Mitigation:** If you must split the view, keep the chart linear and accept the weaker comparison performance as a fallback.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Using separate AM and PM panels because matching hours look neatly paired across panels. **Why it fails:** The panel break slows the comparison and can make readers underestimate small differences.

## How to test the choice <!-- role: check -->

**Failure Sign:** Readers answer that two matched hours are equal when the values differ slightly, or they spend time jumping between panels.
**Quick Check:** A/B test a single 24-hour linear bar chart against split AM/PM linear bar charts on one same-hour comparison.
**Stronger Test:** Log how often readers answer “same” for small but nonzero paired differences in each version.

## What to change <!-- role: fix -->

- Merge AM and PM into one 24-hour linear bar chart for the comparison view.
- Keep the hourly bars on one continuous linear axis when the reader must judge differences.
- If the chart cannot fit, use split linear panels as the fallback rather than switching to a radial form.
