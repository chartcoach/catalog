---
id: use-line-chart-when-comparing-shares-directly
title: Use a line chart when the main task is comparing shares directly
bibliography: references.bib
description: For comparing shares over ordered time, prefer a line chart instead of
  an area chart to improve readability and mitigate hard cross-series comparison for
  readers who need to see one share overtake another.
labels:
- purpose:select
- basis:heuristic
- task:compare
- time:ordered-time
- chart:line:use
- chart:area:avoid
- quality:readability:use
- lever:chart-family
- operator:difference
---

## Switch to a line chart <!-- role: advice -->

Use a line chart instead of an area chart when the message depends on one share being larger than another. For example, show the two shares involved in an overtake as lines instead of stacking every share in an area chart.

## Why direct comparison works better with lines <!-- role: reason -->

Stacked areas make cross-series comparison hard because the shares do not share a stable baseline. A line chart puts the compared shares in the same visual system and can focus only on the series that matter.

**Mechanism:** The line chart makes it easier to compare the size and crossing of selected shares, especially when the story is about one share overtaking another.

**Evidence:** The source says area charts are not the best choice for comparing the size of different shares with each other, and recommends a line chart when the point is that one share overtook another; it also notes that a line chart can show only the necessary shares [@muth_area_charts_2018].

## Use when one comparison drives the story <!-- role: context -->

- **User Goal:** Show that one share is larger than another or that one overtakes another.
- **Task:** Compare selected shares directly over time.
- **Data:** Temporal shares that could be shown in a stacked area chart.
- **Chart Setting:** A multi-series part-to-whole chart is being drafted, but the key message is a direct comparison.
- **Audience:** Readers who need to see the comparison quickly.
- **Success Criterion:** The compared shares can be read against each other without decoding the full stack.

## Do not use when the whole and all shares matter together <!-- role: exceptions -->

**Break it when:** The main message is how the total and all shares develop together over time. **Why:** That is the situation where the area chart is meant to help.

## What you give up <!-- role: costs -->

**Sacrifice:** You give up the full stacked view of all shares as one whole.
**Risk:** The total becomes less prominent, and omitted shares are no longer shown.
**Mitigation:** Keep the area chart when the whole composition is the main message.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keeping every share in a stacked area chart when only one comparison matters. **Why it fails:** The key overtake gets buried inside a chart form that is poor for direct cross-series comparison.

## How to test the choice <!-- role: check -->

**Failure Sign:** The chart story can be told by comparing only one or two shares, but the area chart still stacks all shares.
**Quick Check:** Make a line-chart version with only the compared shares and compare whether the overtake becomes clearer.
**Stronger Test:** If the reader must mainly answer “which share is larger when,” reject the area chart.

## What to change <!-- role: fix -->

- Extract the compared shares into a line chart.
- Remove unrelated shares when they are not needed for the message.
- Keep the area chart only if the full composition over time is the real point.
