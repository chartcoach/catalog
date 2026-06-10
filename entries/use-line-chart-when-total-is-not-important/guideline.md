---
id: use-line-chart-when-total-is-not-important
title: Use a line chart when the total is not part of the message
bibliography: references.bib
description: For showing multiple values over ordered time, prefer a line chart on
  temporal series instead of an area chart to improve readability and mitigate unnecessary
  emphasis on the stacked total for readers who mainly need the series trends.
labels:
- purpose:select
- basis:heuristic
- task:trend
- time:ordered-time
- chart:line:use
- chart:area:avoid
- quality:readability:use
- lever:chart-family
---

## Switch to a line chart <!-- role: advice -->

Use a line chart instead of an area chart when the total is not important. For example, keep changing shares as separate lines when readers need the trajectories over time but not the combined stacked height.

## Why the line chart is easier here <!-- role: reason -->

A filled stacked shape adds a total cue that readers must parse even when the total is not part of the story. Removing the fill lets readers focus on the series themselves.

**Mechanism:** The line chart removes unnecessary part-to-whole emphasis, so readers can read the changing values without also interpreting the stacked total.

**Evidence:** The source says area charts work best when the total is as important as its shares, and that many readers will have an easier time understanding a line chart when the total is not important [@muth_area_charts_2018].

## Use when the total is secondary <!-- role: context -->

- **User Goal:** Show how several values change over time.
- **Task:** Follow the trajectories of the series, not the combined total.
- **Data:** Multiple temporal values that could be drawn as a stacked area chart.
- **Chart Setting:** A draft area chart is being considered for a time series.
- **Audience:** Readers who should understand the chart quickly.
- **Success Criterion:** Readers can read the change in each series without needing the stacked height.

## Do not use when the total matters too <!-- role: exceptions -->

**Break it when:** The total is as important as the shares, or each date adds up to 100%. **Why:** The stacked height then carries part of the message, and an area chart can be an intuitive way to show the whole and its parts together.

## What you give up <!-- role: costs -->

**Sacrifice:** You give up the immediate display of the total as the height of the stack.
**Risk:** The part-to-whole relationship becomes less prominent.
**Mitigation:** Keep the area chart when the whole matters as much as the parts.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keeping a filled area chart even though the message does not use the total. **Why it fails:** The fill adds a visual cue that readers must process even though it does not answer the main question.

## How to test the choice <!-- role: check -->

**Failure Sign:** The story still works if the fill is removed and only the series lines remain.
**Quick Check:** Make a line-chart version and compare it with the area-chart version; if both say the same thing and the total is not needed, keep the line chart.
**Stronger Test:** Ask whether the stacked height must be read at all; if not, reject the area chart.

## What to change <!-- role: fix -->

- Remove the area fill and keep the series as lines.
- Recheck whether the total is still part of the intended message.
- If the whole and its shares are both important, switch back to an area chart.
