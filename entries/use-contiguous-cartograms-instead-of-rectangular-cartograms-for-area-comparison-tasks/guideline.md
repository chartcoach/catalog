---
id: use-contiguous-cartograms-instead-of-rectangular-cartograms-for-area-comparison-tasks
title: Use contiguous cartograms instead of rectangular cartograms for area-comparison
  tasks
bibliography: references.bib
description: For compare tasks on geospatial cartograms, prefer a contiguous cartogram
  type on area-encoded map views to improve fidelity and mitigate area-judgment errors
  for readers comparing region sizes, ranking regions, or judging growth and shrinkage.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:map
- data:geospatial
- quality:fidelity:use
- lever:chart-family
- channel:area
---

## Choose a contiguous cartogram for area judgments <!-- role: advice -->

Use a contiguous cartogram when readers must compare region areas, identify the largest regions, or judge whether a region grew or shrank. For example, replace a rectangular cartogram with a contiguous cartogram for bigger-than, top-k, or change-detection tasks.

## Why contiguous cartograms help size judgments <!-- role: reason -->

Area judgments get harder when region shapes become overly schematic or visually awkward, and contiguous cartograms reduce that problem relative to rectangular ones.

**Mechanism:** A contiguous cartogram keeps the region as a connected, map-like area, which supports direct size comparison better than a rectangular cartogram with potentially misleading rectangle shapes and aspect ratios.

**Evidence:** In the controlled study, contiguous cartograms had the lowest error across compare, find top-k, and detect change tasks, and they were significantly more accurate than rectangular cartograms on all three tasks [@nusratEvaluatingCartogramEffectiveness2018; @zengReviewCollationGraphical2023].

## Use when readers must compare areas region by region <!-- role: context -->

- **User Goal:** Judge which region is bigger, which regions rank highest, or whether a region increased or decreased.
- **Task:** Compare areas, find top-k, or detect change in a cartogram.
- **Data:** Geospatial regions with values encoded by area.
- **Chart Setting:** A static cartogram where individual region areas must be compared directly.
- **Success Criterion:** Fewer size-comparison errors.

## Do not use when only the overall pattern matters <!-- role: exceptions -->

**Break it when:** The chart’s job is broad pattern summary rather than region-by-region area judgment. **Why:** Dorling cartograms performed best for summarize tasks and rectangular cartograms were not needed for that overview role.

## Tradeoffs of using a contiguous cartogram for size judgments <!-- role: costs -->

**Sacrifice:** Perfect regularity of region shape.
**Risk:** Some shapes still distort enough to make other tasks, such as exact shape recognition, harder.
**Mitigation:** If the task changes to shape recognition, switch to a non-contiguous cartogram.

## Common failure mode for area comparison <!-- role: mistakes -->

**Mistake:** Using a rectangular cartogram for region-size judgments. **Why it fails:** Rectangle forms and aspect ratios make region-by-region size judgments less accurate in practice.

## Check whether the cartogram supports area judgments <!-- role: check -->

**Failure Sign:** Readers miss which region is bigger, which ranks highest, or whether a region changed size.
**Quick Check:** Ask one larger-than or top-k question on the current cartogram and on a contiguous alternative.
**Stronger Test:** Compare error rates across a small set of compare, ranking, and change-detection questions.

## Fix the area-comparison failure <!-- role: fix -->

- Replace the rectangular cartogram with a contiguous cartogram.
- Keep area as the value channel, but move the reader to connected, map-like regions rather than rectangles.
- If the chart only needs a broad overview, switch to a Dorling cartogram instead of keeping the rectangular form.
