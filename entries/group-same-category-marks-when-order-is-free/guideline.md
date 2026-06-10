---
id: group-same-category-marks-when-order-is-free
title: Group same-category marks when order is free
bibliography: references.bib
description: For target-search tasks, use spatial grouping of same-category marks
  on reorderable categorical mark views to improve search speed and mitigate slow
  scanning in randomly interleaved layouts for readers locating a single target.
labels:
- purpose:refine
- basis:empirical
- data:categorical
- quality:readability
- lever:layout-structure
- reading-mode:lookup
---

## Spatial grouping <!-- role: advice -->

Spatially group same-category marks when mark order is free. For example, cluster same-color marks into contiguous regions in a grid-, matrix-, or other reorderable mark display instead of leaving them randomly interleaved.

## Why grouping speeds search <!-- role: reason -->

Spatial grouping makes many small marks behave like a few larger perceptual groups. That reduces serial inspection and helps the target stand out even as more marks are added.

**Mechanism:** Grouping by similarity turns a search over many individual marks into a search over a smaller number of grouped regions.

**Evidence:** The review collated this study as graphical-perception knowledge for visualization recommendation, and the underlying experiments found faster target search for grouped than random layouts in both grids and scatterplots, with the gap increasing as the number of marks increased [@zengReviewCollationGraphical2023; @gramazioRelationVisualizationSize2014].

## Use when order is free <!-- role: context -->

- **User Goal:** Locate a known target or anomaly quickly.
- **Task:** Search through many colored marks.
- **Data:** Marks share a small set of nominal color categories.
- **Chart Setting:** Mark order can be rearranged without changing the represented data meaning.
- **Audience:** Readers scanning a view for one target.
- **Success Criterion:** Faster target localization.

## Do not use when position is fixed <!-- role: exceptions -->

**Break it when:** Position or ordering itself encodes the data and cannot be rearranged. **Why:** Grouping by similarity would change the represented structure instead of only improving the search layout.

## Costs of grouping <!-- role: costs -->

**Sacrifice:** Freedom to preserve another ordering.
**Risk:** Ordered blocks of categorical colors can accidentally look like a continuous gradient.
**Mitigation:** Inspect the grouped arrangement for gradient-like color runs before publishing it.

## Common grouping mistake <!-- role: mistakes -->

**Mistake:** Leave same-category marks randomly interleaved after choosing a chart where order is free. **Why it fails:** Readers lose the pop-out benefit and must inspect more individual marks.

## Check grouping with an A/B search test <!-- role: check -->

**Failure Sign:** Readers must scan many individual marks before spotting the target.
**Quick Check:** Compare the current layout with a version where same-category marks are contiguous.
**Stronger Test:** Time the same known-target search on grouped and random orderings of the same data.

## Fix the layout <!-- role: fix -->

- Reorder marks so same-category marks form contiguous regions.
- Keep category regions distinct instead of interleaving their marks.
- If order carries data meaning, leave this view ungrouped and apply a different fix.
