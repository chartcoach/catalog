---
id: use-small-multiples-for-many-categories
title: Use small multiples instead of one crowded chart when each category needs its
  own space
bibliography: references.bib
description: For many-category charts where readers need to inspect each category
  separately, use small multiples on a multi-view layout instead of a single crowded
  view to improve readability and address category collisions.
labels:
- purpose:select
- basis:heuristic
- structure:small-multiples:use
- structure:single-view:avoid
- lever:layout-structure
- group-cardinality:many
- quality:readability:use
---

## Split the chart into panels <!-- role: advice -->

Use small multiples when each category needs its own space to be readable. For example, replace one line chart, area chart, scatterplot, or stacked bar chart full of categories with a panel of one small chart per category.

## Trade shared space for local clarity <!-- role: reason -->

Putting all categories into one view forces them to compete for the same visual space and color budget. Small multiples remove that crowding and make the pattern in each category easier to see, but they also weaken direct across-category comparison.

**Mechanism:** Separate panels reduce overlap and clutter, so readers can inspect one category at a time instead of disentangling many categories inside one frame.

**Evidence:** The post recommends small multiples for line charts, area charts, scatterplots, and stacked bar charts with many categories, and it explicitly says they make trends or patterns within each category easier to see while making cross-category comparisons harder [@muth_fewer_colors_2022].

## Use when within-category reading matters most <!-- role: context -->

- **User Goal:** Make a many-category chart easier to read.
- **Task:** Inspect trends or patterns within each category.
- **Data:** Many categories are shown at once.
- **Chart Setting:** A single chart is crowded because all categories share the same space.
- **Audience:** Readers who need to read each category separately.
- **Success Criterion:** Each category’s pattern is easy to see in its own panel.

## Do not use when direct cross-category comparison is the main task <!-- role: exceptions -->

**Break it when:** Readers mainly need to compare values directly across categories. **Why:** Small multiples make those across-category comparisons harder.

## Accept weaker side-by-side comparison <!-- role: costs -->

**Sacrifice:** Direct comparison between categories becomes less immediate.
**Risk:** Readers may struggle to judge which category is higher than another at the same point.
**Mitigation:** Use the panel layout only when within-category patterns matter more than cross-category comparisons.

## Avoid paneling when the main question is across categories <!-- role: mistakes -->

**Mistake:** Switching to small multiples when the core task is comparing one category directly against another. **Why it fails:** The separate panels remove the shared frame that supports that comparison.

## Compare the panel version against the combined version <!-- role: check -->

**Failure Sign:** The combined chart looks crowded and hard to disentangle.
**Quick Check:** Create a small-multiple version and compare it with the single combined chart.
**Stronger Test:** Choose the panel version only if it makes each category’s pattern easier to see than the single-view version.

## Restructure the chart into one panel per category <!-- role: fix -->

- Split the categories into separate small charts.
- Keep one category per panel instead of layering all categories into one view.
- Return to the single combined view if the main task turns out to be direct cross-category comparison.
