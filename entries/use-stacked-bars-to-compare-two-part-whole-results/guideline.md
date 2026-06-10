---
id: use-stacked-bars-to-compare-two-part-whole-results
title: Use a stacked bar chart to compare shares across two totals
bibliography: references.bib
description: For comparing shares across two totals, use a stacked bar chart instead
  of a pie chart to improve readability and mitigate the single-total limit of pie
  charts for readers.
labels:
- purpose:select
- basis:heuristic
- task:compare
- scope:grouped-result
- chart:bar:use
- chart:pie-donut:avoid
- lever:chart-family
- operator:part-whole
- quality:readability
---

## Choose the stacked bar chart for two totals <!-- role: advice -->

Use a stacked bar chart when you need to compare the shares of two totals. For example, compare two polls with stacked bars rather than trying to make pie charts do a two-result comparison.

## Why two totals outgrow one pie <!-- role: reason -->

A single pie chart can only show one whole and its shares. A stacked bar chart can place two wholes into one comparable display.

**Mechanism:** The chart keeps both totals in the same visual structure, so readers can compare matching shares across results.

**Evidence:** The source says one pie chart can only show one total and its shares, and recommends a stacked bar chart if you want to compare two polls with each other [@muth_pie_charts_2018].

## Use when the comparison spans two totals <!-- role: context -->

- **User Goal:** Compare how two totals break into shares.
- **Task:** Compare corresponding shares across results.
- **Data:** Two totals with categories that sum to 100% within each total.
- **Chart Setting:** Choosing between pie charts and a stacked bar chart.
- **Success Criterion:** Differences across the two totals are easy to compare.

## Do not use when only one total needs to be shown <!-- role: exceptions -->

**Break it when:** You only need to show one total and its shares. **Why:** The single-total limit is no longer a problem.

## Tradeoffs of choosing the stacked bar chart <!-- role: costs -->

**Sacrifice:** You give up the single circular whole.
**Risk:** Using pie charts fragments the comparison across totals.
**Mitigation:** Put both totals into one stacked bar chart when cross-total comparison is the goal.

## Common misuse of pies for two totals <!-- role: mistakes -->

**Mistake:** Using pie charts for a task that compares two polls or two other totals. **Why it fails:** One pie chart can only show one total and its shares.

## Check whether the stacked bar wins this chart choice <!-- role: check -->

**Failure Sign:** The design needs more than one pie to make the comparison.
**Quick Check:** Draft the same two totals as stacked bars and compare whether matching shares are easier to inspect there.
**Stronger Test:** Ask a reviewer which display makes the two results easier to compare and keep the stacked bar if it wins.

## Fix the chart choice for two totals <!-- role: fix -->

- Replace the pie chart approach with a stacked bar chart when comparing two totals.
- Keep both totals in the same chart instead of splitting them into separate pies.
- Use the pie chart only when the display needs to show one total and its shares.
