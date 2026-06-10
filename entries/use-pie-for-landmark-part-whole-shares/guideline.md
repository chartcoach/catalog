---
id: use-pie-for-landmark-part-whole-shares
title: Use a pie chart for quarter-, half-, and three-quarter shares
bibliography: references.bib
description: For part-whole lookup on a single total with a few shares, use a pie
  chart instead of a stacked bar chart when shares are near 25%, 50%, or 75% to improve
  readability and mitigate harder percentage spotting for readers.
labels:
- purpose:select
- basis:heuristic
- chart:pie-donut:use
- chart:bar:avoid
- lever:chart-family
- operator:part-whole
- group-cardinality:few
- quality:readability
---

## Choose the pie chart for landmark shares <!-- role: advice -->

Choose a pie chart when the main readout is whether a share is about a quarter, half, or three-quarters of a single total. For example, use a pie chart instead of a stacked bar chart when readers need to spot 25%, 50%, or 75% shares quickly.

## Why landmark shares read well in a pie <!-- role: reason -->

A pie chart makes the readout the share's fraction of one whole. That helps quarter-, half-, and three-quarter shares stand out as recognizable portions instead of making readers inspect a stacked alternative.

**Mechanism:** The chart emphasizes the slice's share of 100%, so 25%, 50%, and 75% are easier to notice at a glance.

**Evidence:** The source states that pie charts work best for values around 25%, 50%, or 75%, and that these percentages are easier to spot in a pie chart than in a stacked bar or column chart [@muth_pie_charts_2018].

## Use when the readout is a landmark fraction of one whole <!-- role: context -->

- **User Goal:** Show how one total divides into a few shares.
- **Task:** Help readers spot whether a share is about 25%, 50%, or 75%.
- **Data:** One total split into a few categories.
- **Chart Setting:** Choosing between a pie chart and a stacked bar chart.
- **Success Criterion:** Quarter-, half-, and three-quarter shares are easy to spot.

## Do not use when the task is cross-slice comparison <!-- role: exceptions -->

**Break it when:** Readers need to compare the size of shares, especially when differences are small. **Why:** The pie chart is not the best choice for that comparison task.

## Tradeoffs of choosing the pie <!-- role: costs -->

**Sacrifice:** You give up some ease of comparing one share against another.
**Risk:** Close shares can still be harder to distinguish than in a bar-based display.
**Mitigation:** Use this choice only when the main job is spotting quarter-, half-, or three-quarter shares.

## Common misuse of the landmark-share pie <!-- role: mistakes -->

**Mistake:** Using the pie chart when the main question is which similar-sized share is larger. **Why it fails:** The chart favors spotting landmark fractions, not comparing close slice sizes.

## Check whether the pie wins this chart choice <!-- role: check -->

**Failure Sign:** Readers hesitate when asked whether a share is about one quarter, one half, or three quarters.
**Quick Check:** Mock the same data as a pie chart and a stacked bar chart, then keep the version where 25%, 50%, and 75% are easier to spot.
**Stronger Test:** Ask a reviewer to identify the quarter-, half-, and three-quarter shares from both drafts and compare which version works faster.

## Fix the chart choice for landmark shares <!-- role: fix -->

- Switch from a stacked bar chart to a pie chart when the main readout is a 25%, 50%, or 75% share.
- Limit this use to one total with a few shares.
- If the real task becomes comparing shares against each other, replace the pie chart with a bar chart.
