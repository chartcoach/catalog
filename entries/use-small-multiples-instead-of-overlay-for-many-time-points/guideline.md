---
id: use-small-multiples-instead-of-overlay-for-many-time-points
title: Use small multiples instead of overlay when comparing many time points
bibliography: references.bib
description: For ordered-time comparison across many time points, use small multiples
  on repeated views of the same variables to improve insight and mitigate occlusion
  for analysts comparing change over time.
labels:
- purpose:select
- basis:empirical
- task:trend
- time:ordered-time
- structure:small-multiples:use
- structure:single-view:avoid
- lever:layout-structure
- quality:insight
---

## Timepoint panels <!-- role: advice -->

Use small multiples rather than overlaying many time points on the same axes. For example, place each year in its own panel instead of stacking all years into one scatterplot when many time points would cause marks to cover one another.

## Why separate panels scale better over time <!-- role: reason -->

A single overlaid view becomes harder to read as more time points are added. Once multiple time slices share the same space, marks can hide each other and the comparison breaks down.

**Mechanism:** Small multiples keep each time point visible while preserving the repeated visual structure needed for comparison. This supports comparison across larger temporal datasets without the occlusion caused by too many layers in one view.

**Evidence:** The paper states that juxtaposition scales comparisons across larger datasets, while superposition over too many time points causes marks to occlude one another [@szafirGoodBadBiased2018].

## Use when many repeated time views must stay visible <!-- role: context -->

- **User Goal:** Compare change across many time points.
- **Task:** Track how the same variables evolve over time.
- **Data:** Repeated time measurements over enough time points that an overlay would become crowded.
- **Chart Setting:** The design can allocate separate panels for each time point.
- **Audience:** Analysts comparing temporal change across a larger dataset.
- **Success Criterion:** Each time point remains visible without marks hiding one another.

## Do not use when only a small number of time points need precise direct comparison <!-- role: exceptions -->

**Break it when:** Only a small number of time points must be compared and precise immediate comparison is the priority. **Why:** The source says superposition supports more precise and immediate comparison across a small number of time points.

## What you trade away <!-- role: costs -->

**Sacrifice:** You lose direct overlay on shared axes.
**Risk:** Panels that are far apart can be harder to compare precisely.

## Common time-comparison failure <!-- role: mistakes -->

**Mistake:** Layering many time points into one plot. **Why it fails:** Too many layers cause marks to occlude one another and some values become hard or impossible to inspect.

## How to choose between panels and overlay <!-- role: check -->

**Failure Sign:** The overlaid plot hides points, lines, or paths from some time points.
**Quick Check:** Compare a small-multiples draft to an overlaid draft; if the overlaid version loses visibility through overlap, choose small multiples.
**Stronger Test:** Inspect whether each time point can be read without another time point covering it.

## What to change <!-- role: fix -->

- Split the overlaid view into one panel per time point.
- Keep the repeated chart structure the same across panels.
- Reduce the number of time points shown at once if space is limited.
- If the comparison involves only a few time points and marks stay separable, switch to an overlay.
