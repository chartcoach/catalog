---
id: sort-line-chart-x-order-for-correlation-judgment
title: Sort line-chart x order when the goal is correlation judgment
bibliography: references.bib
description: For relate tasks, use value-based x ordering on line charts to improve
  fidelity and mitigate imprecise positive-correlation judgments for readers distinguishing
  nearby association strengths.
labels:
- purpose:refine
- basis:empirical
- task:relate
- chart:line
- quality:fidelity:use
- lever:scale-order
- operator:association
---

## Sort the x order into an ordered line <!-- role: advice -->

Sort the x order to create an ordered line chart when readers need to judge correlation strength from a line-based display. For example, take a plain line chart of two quantitative variables and sort the x positions by value so the relationship is shown as an ordered line rather than the unsorted line form.

## Why ordering helps the line chart <!-- role: reason -->

This is a change inside the line-chart design, not a different dataset. The improvement came from altering the explicit variable order on the x axis.

**Mechanism:** Sorting the x order changed the line display into a form with smaller JNDs for positive correlations, making nearby association strengths easier to distinguish.

**Evidence:** Ordered line charts depicting positive correlations significantly outperformed plain positive line charts, and ordered line performance was also much more stable across positive and negative directions; the 2023 review collated this as empirical guidance for correlation-related chart design [@harrisonRankingVisualizationsCorrelation2014; @zengReviewCollationGraphical2023].

## Use when the line-based view can be reordered <!-- role: context -->

- **User Goal:** Improve correlation judgment while staying in a line-based display.
- **Task:** Compare nearby association strengths.
- **Data:** Two quantitative variables shown with a line chart.
- **Chart Setting:** A static line-based view where x order can be sorted instead of left unsorted.
- **Success Criterion:** More reliable discrimination of nearby correlation values.

## Do not use this move when x order must stay fixed <!-- role: exceptions -->

**Break it when:** The line chart must preserve its existing x ordering and cannot be sorted. **Why:** The tested improvement came specifically from changing the x order to form the ordered line chart.

## What you give up by sorting the line <!-- role: costs -->

**Sacrifice:** You give up the original unsorted x ordering.
**Risk:** If the unsorted order is the main message, reordering changes what the line view shows.
**Mitigation:** Use the ordered version only when judging correlation strength is the main job of the line chart.

## Common implementation mistake <!-- role: mistakes -->

**Mistake:** Keeping an unsorted line chart for correlation judgment when x order is free to change. **Why it fails:** The positive ordered-line version was more precise than the plain positive line version.

## How to test the refinement <!-- role: check -->

**Failure Sign:** The plain line chart makes nearby correlations look too similar to judge reliably.
**Quick Check:** Render the same data as a plain line chart and as an ordered line chart, then compare them on close correlation values.
**Stronger Test:** Ask reviewers to choose which of two close-correlation displays is more correlated in each version and keep the version with more consistent answers.

## What to change <!-- role: fix -->

- Sort the x order to create the ordered-line version of the chart.
- Compare the ordered and plain line versions with the same data and display size.
- Keep the ordered version when it yields more reliable correlation judgments.
