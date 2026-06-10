---
id: facet-categories-instead-of-coloring-a-single-scatterplot-for-dense-summary-tasks
title: Facet categories instead of coloring a single scatterplot when summary tasks
  face many dense groups
bibliography: references.bib
description: For grouped summary tasks with many categories or dense overlap, prefer
  small-multiple faceting over a single-view category-colored scatterplot to improve
  fidelity and mitigate overplotting errors for readers comparing groups.
labels:
- purpose:select
- basis:empirical
- structure:small-multiples:use
- structure:single-view:avoid
- scope:grouped-result
- density:dense
- group-cardinality:many
- quality:fidelity
---

## Replace one crowded color view with faceting <!-- role: advice -->

Facet categories into separate panels instead of keeping all categories together in one color-coded scatterplot when users must compare groups under high category count or heavy overlap. For example, use row faceting by category for maximum-finding or average-comparison tasks rather than a single scatterplot that distinguishes groups only by color.

## Why faceting beats the crowded color view here <!-- role: reason -->

When many points and many categories share one panel, category colors begin to occlude each other and summary judgments break down. Faceting removes that overlap cost, even though readers spend longer comparing across panels.

**Mechanism:** Separating categories into panels reduces congestion and occlusion that otherwise distort group-level judgments in a single shared scatterplot.

**Evidence:** For summary tasks, colored scatterplots degraded as cardinality and congestion increased, while faceted charts held accuracy better and regained a better rank under high-cardinality conditions despite slower completion times [@kimAssessingEffectsTask2018].

## Use when summary accuracy matters more than speed <!-- role: context -->

- **User Goal:** Compare categories, identify the category containing the maximum, or compare category averages.
- **Task:** Group-level summary judgment.
- **Data:** Many categories, many records per category, or clustered points that produce visible overlap.
- **Chart Setting:** A choice between a single-view category-colored scatterplot and a faceted point plot.
- **Success Criterion:** Fewer summary-task errors under congestion.

## Do not use when speed or space dominates the requirement <!-- role: exceptions -->

**Break it when:** Fast completion or limited vertical space is more important than summary accuracy. **Why:** Faceted charts stayed accurate but took longer and often required more scrolling as the number of categories increased.

## What this costs <!-- role: costs -->

**Sacrifice:** You give up some speed and screen economy.
**Risk:** Readers must compare across multiple panels instead of one shared panel.
**Mitigation:** Make this swap when overlap in the single-view plot is already causing group-comparison errors.

## Common failure around this move <!-- role: mistakes -->

**Mistake:** Keep adding categories and points to one color-coded scatterplot for a summary task. **Why it fails:** Overplotting and occlusion increase errors on group-level judgments.

## How to test the choice <!-- role: check -->

**Failure Sign:** Category-colored points overlap heavily and readers cannot isolate groups reliably.
**Quick Check:** A/B compare the current single-view colored scatterplot against a faceted version on one maximum-finding or average-comparison question.
**Stronger Test:** If the faceted version reduces summary-task error enough to justify a slower read, prefer the faceted version.

## What to change <!-- role: fix -->

- Replace category color with category faceting.
- Keep shared quantitative axes across panels so groups remain comparable.
- Use the faceted version when category count or point overlap is high enough to hurt summary accuracy.
