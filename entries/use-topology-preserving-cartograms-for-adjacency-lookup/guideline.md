---
id: use-topology-preserving-cartograms-for-adjacency-lookup
title: Use a topology-preserving cartogram for adjacency lookup
bibliography: references.bib
description: For lookup tasks on geospatial cartograms, prefer a topology-preserving
  cartogram type on distorted map views to improve fidelity and mitigate neighbor-identification
  errors for readers checking which regions touch.
labels:
- purpose:refine
- basis:empirical
- task:relate
- chart:map
- data:geospatial
- quality:fidelity:use
- lever:chart-family
- reading-mode:lookup
---

## Preserve shared borders for neighbor finding <!-- role: advice -->

Choose a topology-preserving cartogram when readers must identify neighboring regions. For example, use a contiguous or rectangular cartogram instead of a non-contiguous or Dorling cartogram for find-the-neighbor tasks.

## Why topology preservation matters for adjacency <!-- role: reason -->

Neighbor lookup depends on shared borders, and readers make many more mistakes when those borders are broken or only approximated.

**Mechanism:** A topology-preserving cartogram keeps adjacency explicit, so readers can answer neighbor questions from the cartogram itself instead of inferring them from approximate proximity.

**Evidence:** In the controlled study, contiguous and rectangular cartograms substantially outperformed non-contiguous and Dorling cartograms on the find adjacency task, with significant error advantages for topology-preserving designs over the non-topology-preserving ones [@nusratEvaluatingCartogramEffectiveness2018; @zengReviewCollationGraphical2023].

## Use when touching relationships are part of the question <!-- role: context -->

- **User Goal:** Determine which regions share a border.
- **Task:** Find adjacency in a cartogram.
- **Data:** Geospatial regions where topological relations matter.
- **Chart Setting:** A static cartogram is being used for neighbor lookup rather than only for broad overview.
- **Success Criterion:** Lower adjacency error.

## Do not use when borders are not the main reading need <!-- role: exceptions -->

- **Break it when:** The main task is recognizing a region by its original shape. **Why:** Non-contiguous cartograms preserve shape better for that task.
- **Break it when:** The main task is only broad pattern summary. **Why:** Dorling cartograms were better for summarize tasks and do not need exact adjacency.

## Tradeoffs of preserving topology <!-- role: costs -->

**Sacrifice:** Some shape or position fidelity, depending on the cartogram type.
**Risk:** A rectangular cartogram can become too schematic for other map-reading tasks.
**Mitigation:** If the chart also needs stronger geographic recognizability, use a contiguous cartogram rather than a rectangular one.

## Common failure mode for adjacency lookup <!-- role: mistakes -->

**Mistake:** Expecting a non-contiguous or Dorling cartogram to support neighbor finding because nearby regions still look close. **Why it fails:** Proximity is not a reliable substitute for preserved shared borders.

## Check whether adjacency is readable <!-- role: check -->

**Failure Sign:** Readers confuse touching regions with merely nearby regions.
**Quick Check:** Ask one neighbor-finding question on the current cartogram and on a topology-preserving alternative.
**Stronger Test:** Compare adjacency error on the same set of questions across the two cartogram types.

## Fix the adjacency failure <!-- role: fix -->

- Replace the current cartogram with a contiguous cartogram or a rectangular cartogram.
- Preserve shared borders between regions instead of relying on proximity alone.
- If the current rectangular cartogram is too schematic for the rest of the task, switch to a contiguous cartogram.
