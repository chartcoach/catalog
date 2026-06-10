---
id: use-line-chart-for-small-differences-over-time
title: Use a line chart when differences between values are very small
bibliography: references.bib
description: For comparing multiple values over ordered time, prefer a line chart
  on temporal series instead of an area chart to improve fidelity and mitigate hidden
  small differences for readers who need to see subtle change.
labels:
- purpose:select
- basis:heuristic
- task:compare
- time:ordered-time
- chart:line:use
- chart:area:avoid
- quality:fidelity:use
- lever:chart-family
---

## Switch to a line chart <!-- role: advice -->

Use a line chart instead of an area chart when the differences between values are very small. For example, redraw small gaps as lines and allow a tighter y-axis range instead of forcing a zero-based area chart.

## Why the line chart reveals small gaps <!-- role: reason -->

Area charts usually need a zero baseline, which compresses small differences. A line chart can use a tighter y-axis range, so subtle separations stay visible.

**Mechanism:** The line chart can stretch the y-axis to show tiny differences that disappear when an area chart starts at zero.

**Evidence:** The source says area charts work best for considerably large differences, and recommends a line chart when differences are very small because the y-axis of a line chart does not need to start at zero [@muth_area_charts_2018].

## Use when subtle differences are the message <!-- role: context -->

- **User Goal:** Show small differences between values over time.
- **Task:** Compare closely spaced series or small changes.
- **Data:** Multiple temporal values with only slight separation.
- **Chart Setting:** An area chart is under consideration for a time series.
- **Audience:** Readers who need to detect subtle differences.
- **Success Criterion:** Small differences remain visible in the chart.

## Do not use when differences are already large <!-- role: exceptions -->

**Break it when:** The differences between the values are considerably large. **Why:** The area chart can then show the trends well enough without hiding the message.

## What you give up <!-- role: costs -->

**Sacrifice:** You give up the filled part-to-whole look of the area chart.
**Risk:** The chart no longer emphasizes the total as a stacked shape.
**Mitigation:** Use the line chart only when the small differences themselves are the key message.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keeping an area chart even though the important differences are tiny. **Why it fails:** The zero-based area scale compresses the variation that readers need to see.

## How to test the choice <!-- role: check -->

**Failure Sign:** The series look nearly flat or merged in the area chart even though their differences matter.
**Quick Check:** Make a line-chart version with a tighter y-axis and compare whether the small differences become legible.
**Stronger Test:** If the important gaps only become visible after removing the area fill and zero-baseline constraint, reject the area chart.

## What to change <!-- role: fix -->

- Replace the area chart with a line chart.
- Use a y-axis range that shows the small differences clearly.
- Keep the area chart only if the differences are large enough to stay visible.
