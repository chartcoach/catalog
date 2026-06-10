---
id: state-one-share-in-text-instead-of-a-two-slice-pie
title: State the value in text instead of drawing a two-slice pie chart
bibliography: references.bib
description: For binary part-whole communication on a single total, use text instead
  of a pie chart to improve readability and mitigate charting a second value that
  is only the remainder to 100% for readers.
labels:
- purpose:select
- basis:heuristic
- chart:text:use
- chart:pie-donut:avoid
- lever:chart-family
- operator:part-whole
- group-cardinality:binary
- quality:readability
---

## Use text for a two-value whole <!-- role: advice -->

State the one percentage directly in text when the data has only two values that sum to 100%. For example, replace a two-slice pie chart with a sentence that names the main share instead of charting that share and its remainder.

## Why a two-slice pie often adds little <!-- role: reason -->

When a whole is split into only two values, the chart effectively repeats one number and its complement. Stating that number directly can say the same thing without adding a chart.

**Mechanism:** The text presents the only independent value directly, rather than drawing both the value and 100% minus that value.

**Evidence:** The source says pie charts might be unnecessary if you only want to show two values, because that is effectively one value and the difference between it and 100%, and suggests mentioning the one number in the article instead of showing a chart [@muth_pie_charts_2018].

## Use when the data is only one share and its remainder <!-- role: context -->

- **User Goal:** Communicate one share of a whole.
- **Data:** Two values that sum to 100%.
- **Chart Setting:** Deciding whether a pie chart is needed at all.
- **Success Criterion:** The key percentage is clear without extra charting.

## Do not use when the whole has more than two shares <!-- role: exceptions -->

**Break it when:** The data contains more than two values. **Why:** The display is no longer effectively just one independent number and its remainder.

## Tradeoffs of choosing text instead of a chart <!-- role: costs -->

**Sacrifice:** You stop showing the complementary share as a separate slice.
**Risk:** Readers must infer that the second share is whatever remains to 100%.
**Mitigation:** State the one percentage directly in the surrounding text.

## Common misuse of the two-slice pie <!-- role: mistakes -->

**Mistake:** Drawing a pie chart for one value and its remainder. **Why it fails:** The chart uses a full display for information that is effectively one number.

## Check whether the chart is unnecessary <!-- role: check -->

**Failure Sign:** The pie chart has only two slices.
**Quick Check:** Remove the chart and see whether the message still works as one stated percentage in text.
**Stronger Test:** If the article sentence already communicates the key share clearly, keep the text and drop the pie chart.

## Fix the chart choice for a two-value whole <!-- role: fix -->

- Count the slices before publishing the pie chart.
- Remove the pie chart when it only shows one share and its remainder.
- State the key percentage directly in the article text.
