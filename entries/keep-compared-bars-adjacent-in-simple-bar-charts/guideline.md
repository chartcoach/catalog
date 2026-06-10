---
id: keep-compared-bars-adjacent-in-simple-bar-charts
title: Keep compared bars adjacent in simple bar charts
bibliography: references.bib
description: For exact comparison tasks, prefer adjacent placement of compared bars
  on simple bar charts to improve fidelity and mitigate separation errors for viewers
  making quick visual estimates.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:bar
- quality:fidelity:use
- lever:layout-structure
- operator:difference
- reading-mode:exact
---

## Adjacent target bars <!-- role: advice -->

Place bars that readers must compare next to each other. For example, keep the target bars adjacent instead of separating them with intervening categories when the task is to judge one bar as a percentage of another.

## Why adjacency works <!-- role: reason -->

Distance itself makes bar-height comparison harder because readers must carry one height across space before matching it to the other bar. The penalty is larger when the reference bar is short.

**Mechanism:** Adjacent bars reduce the spatial carry needed for an exact height judgment, so readers make fewer separation-driven errors.

**Evidence:** Separated bar comparisons produced higher absolute error than adjacent comparisons, and most of that penalty came from the separation itself rather than from intervening distractors; the collated review records this paper as follow-up evidence on bar-chart comparison accuracy [@talbotFourExperimentsPerception2014; @zengReviewCollationGraphical2023].

**Notes:** The separation penalty grew when the reference bar was short.

## When to use adjacency <!-- role: context -->

- **User Goal:** Compare two category values exactly.
- **Task:** Judge one bar relative to another, such as a ratio or percentage estimate.
- **Data:** One quantitative value per category.
- **Chart Setting:** A simple bar chart with separate bars rather than stacked segments.
- **Audience:** Viewers making unaided visual estimates.
- **Success Criterion:** Lower absolute comparison error.

## When not to use adjacency <!-- role: exceptions -->

**Break it when:** The compared values are segments inside the same stacked bar rather than separate bars. **Why:** In that setting, immediate adjacency increased part-to-whole bias, and adding separation helped.

## Tradeoffs of adjacency <!-- role: costs -->

**Sacrifice:** Freedom to leave the compared categories far apart in the displayed order.\
**Risk:** If the compared bars must remain separated, exact judgments become less reliable, especially for short bars.\
**Mitigation:** Apply adjacency to the pair that must be read most precisely.

## Common spacing mistake <!-- role: mistakes -->

**Mistake:** Leaving a large gap between the two target bars because the distractors seem unimportant. **Why it fails:** Separation alone accounted for most of the added error.

## Check bar proximity <!-- role: check -->

**Failure Sign:** Readers hesitate or disagree when comparing two distant bars, especially when one bar is short.\
**Quick Check:** Redraw the same pair so the target bars are adjacent and see whether the comparison reads more cleanly.\
**Stronger Test:** Run a small A/B estimate task on adjacent versus separated versions and compare absolute error.

## Fix bar separation <!-- role: fix -->

- Move the compared bars next to each other.
- Reorder the categories when that comparison is the main task.
- Treat separated short bars as a high-risk layout and regroup the pair before publication.
