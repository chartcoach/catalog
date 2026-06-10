---
id: replace-pie-with-stacked-bar-when-too-many-shares
title: Use a stacked bar chart instead of a pie chart when there are more than five
  shares
bibliography: references.bib
description: For part-whole reading on a single total with more than five shares,
  use a stacked bar chart instead of a pie chart to improve readability and mitigate
  untidy slice labeling for readers.
labels:
- purpose:select
- basis:heuristic
- chart:bar:use
- chart:pie-donut:avoid
- lever:chart-family
- operator:part-whole
- group-cardinality:many
- quality:readability
---

## Choose the stacked bar chart when slices exceed five <!-- role: advice -->

Replace a pie chart with a stacked bar chart when one total has more than five shares. For example, switch once the pie reaches six or more slices and the labeling starts to look crowded.

## Why many shares strain a pie chart <!-- role: reason -->

A pie chart becomes harder to label cleanly as more slices are added. A stacked bar chart keeps the same part-whole structure but gives a tidier arrangement for labels.

**Mechanism:** The chart reduces label clutter by moving the categories into a more orderly layout than many thin wedges.

**Evidence:** The source says pie charts work best with only a few values, five maximum, and recommends a stacked column or stacked bar chart when there are more than five shares because the labeling will be tidier [@muth_pie_charts_2018].

## Use when one total has many shares <!-- role: context -->

- **User Goal:** Show how one total divides into several categories.
- **Data:** One total with more than five shares.
- **Chart Setting:** Choosing between a pie chart and a stacked bar chart.
- **Success Criterion:** Labels stay tidy and the chart remains easy to read.

## Do not use when the pie has five or fewer shares <!-- role: exceptions -->

**Break it when:** The total has five or fewer shares. **Why:** The source treats a pie chart as workable for a few values and flags the problem once the count goes above five.

## Tradeoffs of choosing the stacked bar chart <!-- role: costs -->

**Sacrifice:** You give up the circular slice form.
**Risk:** Keeping the pie chart makes the overall look messier as slices and labels multiply.
**Mitigation:** Switch to the stacked bar chart once the share count passes five.

## Common misuse of the many-slice pie <!-- role: mistakes -->

**Mistake:** Keeping six or more slices as separate wedges in a pie chart. **Why it fails:** The labeling becomes untidy.

## Check whether the stacked bar wins this chart choice <!-- role: check -->

**Failure Sign:** The pie has more than five slices or the labels feel crowded.
**Quick Check:** Count the shares; if there are six or more, compare the pie chart with a stacked bar version.
**Stronger Test:** Keep the version with the tidier label arrangement.

## Fix the chart choice for many shares <!-- role: fix -->

- Count the slices before finalizing the pie chart.
- Replace the pie chart with a stacked bar chart when the count exceeds five.
- Redraft the labels in the stacked bar chart and keep the tidier version.
