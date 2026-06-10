---
id: use-line-chart-when-time-series-totals-are-not-important
title: Use a line chart when totals are not the message
bibliography: references.bib
description: For ordered-time trend reading on part-to-whole time series, use a line
  chart instead of stacked columns when totals are not important to improve readability
  and mitigate hard-to-decipher stacked segments for readers scanning change over
  time.
labels:
- purpose:select
- basis:heuristic
- time:ordered-time
- chart:line:use
- chart:bar:avoid
- operator:part-whole
- quality:readability
- lever:chart-family
---

## Switch to a line chart <!-- role: advice -->

Replace stacked columns with a line chart when the total of the parts is not important on time data. For example, plot the component series as lines across dates instead of stacking them into columns when the reader only needs the over-time change.

## Why the line chart reads faster <!-- role: reason -->

Stacked columns make readers decode several segment positions that do not share a baseline, while a line chart lets them follow change over time directly.

**Mechanism:** The line chart removes the need to read both total height and shifting internal segment baselines, so the time pattern is quicker to decipher.

**Evidence:** The post says stacked column charts for dates should only be considered when the total is crucial, and that a line chart is a better choice when the total is not important because readers can decipher it more quickly [@muth_stacked_columns_2018].

## Use when totals are unnecessary <!-- role: context -->

- **User Goal:** Show how component values change over time.
- **Task:** Read change across dates rather than the combined total.
- **Data:** Time series split into parts that sum to a total.
- **Chart Setting:** A stacked column chart for dates is being considered.
- **Audience:** Readers need a quick read of the temporal pattern.
- **Success Criterion:** The trend is understandable without relying on total column height.

## Do not use when totals must stay visible <!-- role: exceptions -->

**Break it when:** The total of all parts is crucial and the chart needs to show totals and shares together. **Why:** That is the case where stacked columns can justify their extra reading effort.

## What you give up <!-- role: costs -->

**Sacrifice:** You give up the explicit total height that stacked columns show.
**Risk:** Readers may no longer read the display as a part-to-whole chart.
**Mitigation:** Make this switch only when the total is not part of the message.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keeping stacked columns even though the takeaway is only about how the parts change over time. **Why it fails:** Readers spend effort decoding stacked segments that do not help answer the question.

## Test the chart choice <!-- role: check -->

**Failure Sign:** The total height is present, but the takeaway never mentions it.
**Quick Check:** Sketch the same data as stacked columns and as a line chart; if the line chart preserves the message without the total, choose the line chart.
**Stronger Test:** State the takeaway without mentioning the total; if the statement still holds, the stacked total is unnecessary.

## Revise the design <!-- role: fix -->

- Replace the stacked columns with a line chart for the component series.
- Remove emphasis on total height if it does not support the message.
- Keep the focus on the over-time changes that the reader actually needs.
