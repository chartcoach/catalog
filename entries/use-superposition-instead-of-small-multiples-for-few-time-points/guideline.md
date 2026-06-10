---
id: use-superposition-instead-of-small-multiples-for-few-time-points
title: Use superposition instead of small multiples for a small number of time points
bibliography: references.bib
description: For ordered-time comparison across a small number of time points, use
  superposition on shared axes to improve fidelity and mitigate imprecise cross-panel
  comparison for analysts comparing change over time.
labels:
- purpose:select
- basis:empirical
- task:trend
- time:ordered-time
- structure:single-view:use
- structure:small-multiples:avoid
- lever:layout-structure
- quality:fidelity
---

## Timepoint overlay <!-- role: advice -->

Use superposition on shared axes instead of separate panels when only a small number of time points must be compared precisely. For example, draw two or three time points in one scatterplot rather than placing them in separate panels when the marks remain distinct.

## Why overlay helps precise comparison for few time points <!-- role: reason -->

When only a few time points are present, putting them on the same axes removes the need to compare distances across separated panels. That makes immediate visual comparison easier.

**Mechanism:** Superposition aligns time points in one coordinate system, so readers can compare differences directly without shifting between panels. This improves precision as long as the number of layers stays small enough to avoid occlusion.

**Evidence:** The paper states that superposition facilitates precise and immediate comparison across a small number of time points, while juxtaposition can make precise comparison difficult when visualizations are far apart [@szafirGoodBadBiased2018].

## Use when a few time points need exact side-by-side reading on shared axes <!-- role: context -->

- **User Goal:** Compare a few time points as precisely and immediately as possible.
- **Task:** Judge change across a small number of repeated measurements.
- **Data:** Repeated time measurements with only a small number of time points shown at once.
- **Chart Setting:** Marks remain separable when overlaid on shared axes.
- **Audience:** Analysts comparing temporal differences directly.
- **Success Criterion:** Differences are easier to see in one aligned coordinate system than across separate panels.

## Do not use when the overlay becomes crowded <!-- role: exceptions -->

**Break it when:** Many time points or a larger dataset cause the overlaid marks to occlude one another. **Why:** The source says too many overlaid time points reduce readability through occlusion.

## What you trade away <!-- role: costs -->

**Sacrifice:** You lose scalability to many time points.
**Risk:** Extra layers can quickly create overlap and hide data.
**Mitigation:** Restrict the overlay to a small number of time points.

## Common time-comparison failure <!-- role: mistakes -->

**Mistake:** Separating a small number of time points into panels when precise direct comparison is the goal. **Why it fails:** Readers must compare views that may be far apart instead of reading the differences from one shared frame.

## How to choose between overlay and panels <!-- role: check -->

**Failure Sign:** Separate panels force more eye movement than the task needs, while an overlay would remain legible.
**Quick Check:** Compare an overlaid draft with a small-multiples draft; if the overlay stays distinct and makes differences more immediate, choose the overlay.
**Stronger Test:** Verify that no overlaid marks are hidden or merged once the time points share the same axes.

## What to change <!-- role: fix -->

- Combine the few time points into one plot with shared axes.
- Keep the number of overlaid time points small enough to avoid occlusion.
- Remove separate panels when they only make the same comparison less direct.
- If overlap appears after overlaying, revert to small multiples.
