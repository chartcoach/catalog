---
id: use-contiguous-cartograms-instead-of-rectangular-cartograms-for-region-location-lookup
title: Use contiguous cartograms instead of rectangular cartograms for region location
  lookup
bibliography: references.bib
description: For lookup tasks on geospatial cartograms, prefer a contiguous cartogram
  type on distorted map views to improve fidelity and mitigate region-location lookup
  errors for readers finding a region on the cartogram.
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

## Choose a locality-preserving cartogram type <!-- role: advice -->

Use a contiguous cartogram when readers must find a region on a distorted map. For example, replace a rectangular cartogram with a contiguous cartogram for locate-the-region tasks.

## Why contiguous cartograms help location lookup <!-- role: reason -->

Keeping the map visually connected helps readers search by approximate geographic position instead of re-learning a schematic layout.

**Mechanism:** A contiguous cartogram preserves more of the map’s spatial arrangement than a rectangular cartogram, so readers can use relative location cues to find the target region.

**Evidence:** In the controlled study, contiguous cartograms outperformed rectangular cartograms on the locate task in both accuracy and time, with statistically significant differences [@nusratEvaluatingCartogramEffectiveness2018; @zengReviewCollationGraphical2023].

## Use when readers must find a region quickly and correctly <!-- role: context -->

- **User Goal:** Find a specific region on the cartogram.
- **Task:** Locate a highlighted region from the source map in the cartogram.
- **Data:** Geospatial regions with meaningful relative positions.
- **Chart Setting:** A static cartogram is used for lookup rather than only for broad summary.
- **Success Criterion:** Lower lookup error and faster completion.

## Do not use when exact shape recognition is the main task <!-- role: exceptions -->

**Break it when:** The main task is recognizing a region by its original outline. **Why:** Non-contiguous cartograms preserve shape better and were more accurate for recognition.

## Tradeoffs of using a contiguous cartogram <!-- role: costs -->

**Sacrifice:** Perfect geometric regularity.
**Risk:** Some region shapes still become distorted.
**Mitigation:** If outline recognition matters more than location lookup, switch to a non-contiguous cartogram.

## Common failure mode for location lookup <!-- role: mistakes -->

**Mistake:** Using a rectangular cartogram for find-the-region tasks. **Why it fails:** The schematic rectangles weaken the relative-position cues that readers use to search the map.

## Check whether location lookup is working <!-- role: check -->

**Failure Sign:** Readers take longer or make more mistakes when finding a target region.
**Quick Check:** Run one locate-the-region question on the current view and on a contiguous alternative.
**Stronger Test:** Compare error and completion time for a small set of location questions across the two cartogram types.

## Fix the location-lookup failure <!-- role: fix -->

- Replace the rectangular cartogram with a contiguous cartogram.
- Keep the cartogram connected so readers can use relative position cues.
- If the task changes from location lookup to shape recognition, switch to a non-contiguous cartogram instead.
