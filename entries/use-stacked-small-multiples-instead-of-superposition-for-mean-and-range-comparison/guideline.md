---
id: use-stacked-small-multiples-instead-of-superposition-for-mean-and-range-comparison
title: Use vertically stacked small multiples instead of superposition for mean and
  range comparison
bibliography: references.bib
description: For set-to-set comparison of mean or range during brief inspection, prefer
  vertically stacked small-multiple layouts on paired bar charts to improve fidelity
  and mitigate errors from overlapping sets for brief visual inspection.
labels:
- purpose:select
- basis:empirical
- task:compare
- chart:bar
- structure:small-multiples:use
- structure:single-view:avoid
- quality:fidelity:use
- lever:layout-structure
---

## Stacked small-multiple layout <!-- role: advice -->

Choose a vertically stacked small-multiple layout when readers must decide which bar set has the larger mean or wider range. For example, place the two bar charts one above the other and avoid a single superposed view that overlays both series in the same space.

## Why stacked separation works for these set-level comparisons <!-- role: reason -->

Set-level comparisons depend on seeing each bar set as its own unit. A stacked layout keeps the two sets separate while preserving direct vertical alignment, whereas superposition forces readers to separate overlapping groups before comparing them.

**Mechanism:** Vertical separation supports whole-set comparison of the bar sets, and the stacked arrangement lets readers compare corresponding bar lengths by slicing downward between the two charts.

**Evidence:** In two crowdsourced staircase experiments, vertically stacked bar charts produced the most precise judgments for largest-mean and widest-range comparisons, while superposed charts produced the least precise judgments for both tasks [@jardinePerceptualProxiesVisual2020].

**Notes:** The paper also reports that mean judgments were consistent with global proxies such as mean length and bar centroids, while range judgments were consistent with focal within-set delta proxies.

## Use when comparing whole bar sets <!-- role: context -->

- **User Goal:** Decide which of two bar sets has the larger mean or the wider range.
- **Task:** Set-to-set comparison rather than item-to-item change detection.
- **Data:** Two quantitative series shown as multiple bars per set.
- **Chart Setting:** Paired horizontal bar charts where the layout choice is between separated views and an overlaid view.
- **Audience:** Readers making a brief visual judgment.
- **Success Criterion:** Small differences in mean or range remain discriminable.

## Do not use when the task shifts to item-level change <!-- role: exceptions -->

**Break it when:** The reader must find which individual item changed the most between the two series. **Why:** The paper reports that item-to-item biggest-delta judgments were better supported by animated or superposed arrangements than by separated stacked views.

## What you trade away with stacked separation <!-- role: costs -->

**Sacrifice:** You give up the compactness of a single overlaid chart.
**Risk:** If applied to an item-to-item change task, the separated layout can weaken the direct local cues that highlight the largest change.
**Mitigation:** Reserve the stacked layout for whole-set mean or range comparison.

## Common layout failure <!-- role: mistakes -->

**Mistake:** Overlay the two bar sets in one shared plotting space to save space. **Why it fails:** Superposition was the least precise arrangement for deciding which set had the larger mean or the wider range.

## Compare the stacked and superposed versions directly <!-- role: check -->

**Failure Sign:** Reviewers hesitate, inspect overlaps, or lose track of which whole set is larger.
**Quick Check:** Build stacked and superposed versions of the same two bar sets and ask for a brief larger-mean or wider-range judgment; prefer the stacked version if it yields surer answers.
**Stronger Test:** Run a short timed A/B test and compare correctness on the same comparison task across the two layouts.

## Convert the overlaid chart into stacked small multiples <!-- role: fix -->

- Split the superposed bar chart into two separate bar charts.
- Place one chart directly above the other so corresponding bars align vertically.
- Remove the superposed version when the decision is about the larger mean or wider range.
