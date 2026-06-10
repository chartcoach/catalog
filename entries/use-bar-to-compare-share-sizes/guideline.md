---
id: use-bar-to-compare-share-sizes
title: Use a bar chart instead of a pie chart to compare share sizes
bibliography: references.bib
description: For comparing shares within a single total, use a bar chart instead of
  a pie chart to improve readability and mitigate hard-to-see small differences for
  readers.
labels:
- purpose:select
- basis:heuristic
- task:compare
- chart:bar:use
- chart:pie-donut:avoid
- lever:chart-family
- operator:part-whole
- quality:readability
---

## Choose the bar chart for share comparison <!-- role: advice -->

Use a bar chart when readers need to compare the sizes of shares within one total. For example, replace a pie chart with a bar chart when differences between shares are small.

## Why bars support share comparison better than pies <!-- role: reason -->

A bar chart gives each share a directly comparable length. That makes small differences easier to inspect than asking readers to compare slice sizes in a pie.

**Mechanism:** The chart turns the task into side-by-side length comparison, which helps readers judge which share is larger.

**Evidence:** The source says pie charts are not the best choice if readers need to compare the size of shares, especially when differences are small, and recommends considering a bar or column chart instead [@muth_pie_charts_2018].

## Use when the task is comparing shares within one total <!-- role: context -->

- **User Goal:** Compare the sizes of categories that add up to a whole.
- **Task:** Judge which share is bigger and by how much.
- **Data:** One total divided into multiple shares.
- **Chart Setting:** Choosing between a pie chart and a bar chart.
- **Success Criterion:** Small differences between shares are easy to see.

## Do not use when the task is spotting landmark fractions <!-- role: exceptions -->

**Break it when:** The main question is whether a share is around 25%, 50%, or 75%. **Why:** Pie charts work better for spotting those landmark percentages.

## Tradeoffs of choosing the bar chart <!-- role: costs -->

**Sacrifice:** You stop showing the shares as slices of a circle.
**Risk:** Keeping the pie chart makes close differences hard to compare.
**Mitigation:** Switch to the bar chart when cross-category comparison is the main job.

## Common misuse of the share-comparison bar <!-- role: mistakes -->

**Mistake:** Keeping a pie chart for a task that asks readers to compare similarly sized shares. **Why it fails:** Small differences are harder to compare in a pie.

## Check whether the bar wins this chart choice <!-- role: check -->

**Failure Sign:** Readers struggle to tell which of two similar shares is larger.
**Quick Check:** Draft the same data as both a pie chart and a bar chart, then compare which one makes the larger share more obvious.
**Stronger Test:** Ask a reviewer to identify the larger of two close shares from both drafts and keep the easier version.

## Fix the chart choice for share comparison <!-- role: fix -->

- Replace the pie chart with a bar chart when the goal is comparing share sizes.
- Make the switch as soon as the differences between shares are small.
- Keep the pie chart only if the real job is spotting quarter-, half-, or three-quarter shares instead.
