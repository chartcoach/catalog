---
id: use-row-facets-over-single-view-hue-encoding-for-dense-summary-tasks
title: Use row facets instead of single-view hue encoding for dense summary tasks
bibliography: references.bib
description: For group-level summary judgments in dense point-based views, prefer
  row facets on categorical groups to improve fidelity and mitigate congestion from
  single-view hue encoding for readers comparing groups.
labels:
- purpose:select
- basis:empirical
- quality:fidelity:use
- lever:layout-structure
- density:dense
- group-cardinality:many
- structure:small-multiples:use
- structure:single-view:avoid
---

## Split dense summary comparisons into row facets <!-- role: advice -->

Use row facets instead of encoding categories only by hue in one panel when readers must compare group summaries under dense conditions. For example, split categories into stacked panels rather than relying on one hue-coded point cloud when the task is to find which group contains the maximum value or to compare group averages across many or overlapping categories.

## Why row facets help in dense summaries <!-- role: reason -->

Dense single-view hue encodings lose accuracy as categories increase, points per category increase, or overlap grows. Row facets trade speed for better separation, which helps preserve group-level summary judgments in those dense cases.

**Mechanism:** Faceting reduces category overlap and congestion, while a single hue-coded panel forces the reader to separate groups inside one crowded field of points.

**Evidence:** For summary tasks, the study found that single-view color-coded point plots degraded as cardinality and congestion increased, while row-faceted views regained relative accuracy under those high-density conditions even though they were slower [@zengReviewCollationGraphical2023; @kimAssessingEffectsTask2018].

## Use when overplotting threatens group summaries <!-- role: context -->

- **User Goal:** Compare groups by maxima or averages rather than read individual values.
- **Task:** Group-level summary judgment.
- **Data:** Many categories, many points per category, or overlap caused by clustered points.
- **Chart Setting:** A single-view hue-coded point plot is under consideration for the category field.
- **Success Criterion:** Better accuracy on group summary judgments despite a denser dataset.

## Do not use this for fast individual-value reading <!-- role: exceptions -->

**Break it when:** The reader mainly needs exact lookup or pairwise comparison of individual points. **Why:** Row facets were slower than single-view layouts on those value tasks.

## What you give up <!-- role: costs -->

**Sacrifice:** You give up some speed and compactness.
**Risk:** Stacked facets can require more scanning and sometimes scrolling.
**Mitigation:** Reserve the facet split for summary tasks where congestion is already harming accuracy.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keep a dense, many-category summary task in a single hue-coded panel. **Why it fails:** Congestion and overlap make it harder to separate groups accurately.

## Compare the dense summary versions directly <!-- role: check -->

**Failure Sign:** Group summaries become hard to judge because points overlap and categories blend together in one panel.
**Quick Check:** Compare a single-view hue-coded version against a row-faceted version on one maximum-search question and one group-average comparison question.
**Stronger Test:** Increase category count or point count with representative data and compare accuracy across the two layouts.

## Split the categories into panels <!-- role: fix -->

- Move the category field from hue in one panel to row facets.
- Keep the summary comparison task the same while re-testing the layout.
- Accept the slower layout only when it clearly improves summary-task accuracy under dense conditions.
