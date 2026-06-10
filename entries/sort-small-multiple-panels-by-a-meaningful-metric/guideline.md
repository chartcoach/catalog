---
id: sort-small-multiple-panels-by-a-meaningful-metric
title: Sort small-multiple panels by a meaningful metric
bibliography: references.bib
description: For navigation and ranking in small-multiple line charts, use meaningful
  panel order on the panel grid to improve insight and address arbitrary reading order
  for readers scanning many panels.
labels:
- purpose:refine
- basis:heuristic
- structure:small-multiples
- quality:insight
- lever:scale-order
- operator:rank
- component:caption:use
---

## Sort panels by a meaningful metric <!-- role: advice -->

Order small-multiple panels by a value or change measure that matches the question. For example, sort by start value, end value, range, percent change, or difference, and say that sort order in the chart description.

## Why panel order carries analytical meaning <!-- role: reason -->

Panel order tells readers where to start and how categories relate. A metric-driven order turns the grid into an organized comparison rather than a random collection.

**Mechanism:** Sorting by start value, end value, or change makes ranking logic visible and helps readers move through the panels with a clear question in mind.

**Evidence:** The post recommends sorting panels by metrics such as start value, end value, range, percent change, or difference, and says alphabetical order is better than no logic when a meaningful order is absent [@muth_small_multiple_line_charts_2024].

## Use when readers need guidance through many panels <!-- role: context -->

- **User Goal:** Help readers know what to look at first.
- **Task:** Rank or organize categories across many panels.
- **Data:** Multiple panels that could be ordered by start, end, range, percent change, or difference.
- **Chart Setting:** A small-multiple line chart with enough panels that navigation matters.
- **Success Criterion:** The order itself communicates a comparison or ranking logic.

## Do not use a metric sort when there is no meaningful metric to sort by <!-- role: exceptions -->

**Break it when:** There is no obvious substantive logic for a metric sort. **Why:** An arbitrary order does not help navigation; alphabetical order is better than none.

## Costs of imposing an analytical order <!-- role: costs -->

**Sacrifice:** You may lose an alphabetical or otherwise familiar lookup order.
**Risk:** A meaningful sort can still confuse if readers are not told what the ordering rule is.
**Mitigation:** State the sort rule in the chart description.

## Common ordering mistake <!-- role: mistakes -->

**Mistake:** Leave panels unsorted or use an unexplained order. **Why it fails:** Readers cannot tell what to look at first or how the panels relate.

## Check whether the order explains itself <!-- role: check -->

**Failure Sign:** The panel order feels arbitrary.
**Quick Check:** See whether you can name the sort field in one short chart description using start value, end value, range, percent change, or difference.
**Stronger Test:** If you cannot name a meaningful sort field, switch to alphabetical order and check whether navigation becomes clearer.

## Edits that give panel order a job <!-- role: fix -->

- Choose one sorting field that matches the message, such as start value, end value, range, percent change, or difference.
- Apply that order consistently across the panel grid.
- State the sort order in the chart description.
- If no meaningful metric exists, switch to alphabetical order.
