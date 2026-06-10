---
id: use-a-single-24-hour-bar-chart-to-find-the-daily-maximum
title: Use a single 24-hour bar chart to find the daily maximum
bibliography: references.bib
description: For finding the maximum in cyclic-time hourly data, use a single-view
  structure on bar charts to improve fidelity and mitigate wrong-half selections for
  non-expert readers.
labels:
- purpose:select
- basis:empirical
- task:extreme
- time:cyclic-time
- chart:bar
- structure:single-view:use
- structure:multi-view:avoid
- quality:fidelity
- lever:layout-structure
---

## Use one continuous 24-hour bar view <!-- role: advice -->

Use one continuous 24-hour bar chart when the task is to find the day-wide maximum. For example, merge separate AM and PM bar panels into one 24-hour axis instead of asking readers to scan two 12-hour charts for the highest bar.

## Why one continuous view works <!-- role: reason -->

A continuous bar view lets readers scan one run of bars and judge the global maximum without switching panels. Split views force a cross-panel search and can make readers pick the highest bar from the wrong half of the day.

**Mechanism:** One uninterrupted sequence reduces panel switching and supports a direct search for the tallest bar across the full day.

**Evidence:** For the daily-pattern maximum task, the 24-hour linear bar chart was the fastest condition, and split charts produced errors where readers selected the maximum from the wrong chart half [@waldnerComparisonRadialLinear2020; @zengReviewCollationGraphical2023].

## Use when the maximum must be found across the whole day <!-- role: context -->

- **User Goal:** Identify the highest hour in the full 24-hour cycle.
- **Task:** Find the global maximum.
- **Data:** One value per hour across a single day.
- **Chart Setting:** Bar chart shown either as one 24-hour view or as separate AM/PM panels.
- **Audience:** Non-expert readers.
- **Success Criterion:** Fast and correct selection of the day-wide maximum.

## When to break the rule <!-- role: exceptions -->

**Break it when:** The available width cannot support a readable 24-hour bar chart. **Why:** The supported fallback is to keep the display linear and split it into separate bar panels rather than switching to a rose chart.

## What you trade away <!-- role: costs -->

**Sacrifice:** You lose the smaller AM/PM chunks that can make each half feel locally simpler.
**Risk:** If the 24-hour chart is squeezed too tightly, bars can become crowded.
**Mitigation:** Use split linear panels only as a fallback when the continuous 24-hour view does not fit.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keeping separate AM and PM panels when the reader must find the day-wide maximum. **Why it fails:** Readers can stop at the maximum in one panel and miss that the higher bar is in the other panel.

## How to test the choice <!-- role: check -->

**Failure Sign:** Readers report the maximum from AM or PM without checking the other half.
**Quick Check:** A/B test a 24-hour bar chart against split AM/PM bar charts on one maximum-finding question.
**Stronger Test:** Record completion time and note whether wrong answers come from choosing the tallest bar in the wrong panel.

## What to change <!-- role: fix -->

- Merge AM and PM panels into one 24-hour bar chart for the maximum-finding view.
- Keep one continuous hourly axis so the tallest bar is searched in a single scan.
- If the chart cannot fit at full width, use split linear bar panels as the fallback rather than a radial chart.
