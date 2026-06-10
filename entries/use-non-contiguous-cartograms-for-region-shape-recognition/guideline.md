---
id: use-non-contiguous-cartograms-for-region-shape-recognition
title: Use non-contiguous cartograms for region shape recognition
bibliography: references.bib
description: For lookup tasks on geospatial cartograms, prefer a shape-preserving
  cartogram type on distorted map views to improve fidelity and mitigate region-shape
  identification errors for readers matching regions back to the original map.
labels:
- purpose:refine
- basis:empirical
- task:retrieve
- chart:map
- data:geospatial
- quality:fidelity:use
- lever:chart-family
- reading-mode:lookup
---

## Choose a shape-preserving cartogram type <!-- role: advice -->

Use a non-contiguous cartogram when readers must recognize a region by its original outline. For example, replace a contiguous cartogram with a non-contiguous cartogram for map-to-cartogram shape-matching tasks.

## Why shape preservation works here <!-- role: reason -->

Preserving the original region outline removes the extra step of decoding a deformed polygon before the reader can match it to the source geography.

**Mechanism:** A non-contiguous cartogram keeps each region’s original shape, so readers can match outlines directly instead of inferring them from a distorted boundary.

**Evidence:** In the controlled study, non-contiguous cartograms produced significantly lower error than contiguous cartograms on the recognize task, while completion time was not significantly different [@nusratEvaluatingCartogramEffectiveness2018; @zengReviewCollationGraphical2023].

## Use when shape matching is the main job <!-- role: context -->

- **User Goal:** Match a region in the cartogram back to its original geographic shape.
- **Task:** Identify which distorted region corresponds to a region from the source map.
- **Data:** Geospatial regions where outline recognition matters.
- **Chart Setting:** A static cartogram is being used as a map-like view rather than only as an abstract summary.
- **Success Criterion:** Fewer recognition errors.

## Do not use when shared borders matter more than outlines <!-- role: exceptions -->

**Break it when:** The main task is finding which regions touch each other. **Why:** Non-contiguous cartograms do not preserve adjacency, and they performed poorly on neighbor-finding.

## Tradeoffs of shape preservation <!-- role: costs -->

**Sacrifice:** Shared borders between regions.
**Risk:** The map can become sparse and visually fragmented.
**Mitigation:** If adjacency must remain readable, switch to a contiguous cartogram instead of forcing the task onto a non-contiguous one.

## Common failure mode for shape recognition <!-- role: mistakes -->

**Mistake:** Asking readers to recognize region shapes in a cartogram that replaces regions with circles, rectangles, or heavily deformed polygons. **Why it fails:** The original outlines are no longer directly available for matching.

## Check whether shape recognition is being supported <!-- role: check -->

**Failure Sign:** Readers confuse which cartogram region corresponds to the original map region.
**Quick Check:** Ask a reviewer to match one highlighted source-map region to the correct cartogram region.
**Stronger Test:** Compare recognition error on the current cartogram type against a non-contiguous version using the same matching questions.

## Fix the recognition failure <!-- role: fix -->

- Replace the current cartogram type with a non-contiguous cartogram.
- Keep regions in their geographic positions while preserving their original outlines.
- If the chart also needs neighbor lookup, switch to a contiguous cartogram rather than keeping a non-contiguous one.
