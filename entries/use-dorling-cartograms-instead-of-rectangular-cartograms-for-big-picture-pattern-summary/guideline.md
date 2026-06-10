---
id: use-dorling-cartograms-instead-of-rectangular-cartograms-for-big-picture-pattern-summary
title: Use Dorling cartograms instead of rectangular cartograms for big-picture pattern
  summary
bibliography: references.bib
description: For overview tasks on geospatial cartograms, prefer a Dorling cartogram
  type on area-encoded map views to improve insight and mitigate broad-pattern reading
  errors for readers summarizing spatial trends and distributions.
labels:
- purpose:refine
- basis:empirical
- chart:map
- data:geospatial
- quality:insight:use
- lever:chart-family
- reading-mode:overview
- channel:area
---

## Choose a Dorling cartogram for the big picture <!-- role: advice -->

Use a Dorling cartogram when the chart’s job is to show the overall pattern rather than detailed map reading. For example, replace a rectangular cartogram with a Dorling cartogram for summarize-the-pattern tasks about broad spatial distributions or trends.

## Why Dorling cartograms help overview reading <!-- role: reason -->

Simple circular marks make the overall pattern easier to scan, while heavily schematic rectangular regions interfere with reading the big picture.

**Mechanism:** A Dorling cartogram reduces the visual complexity of the map to circles sized by value, which helps readers summarize broad spatial patterns without getting distracted by distorted polygon geometry.

**Evidence:** In the controlled study, Dorling cartograms ranked best on summarize accuracy and were significantly more accurate than rectangular cartograms, which performed worst for the big-picture task [@nusratEvaluatingCartogramEffectiveness2018; @zengReviewCollationGraphical2023].

## Use when overview matters more than detailed map reading <!-- role: context -->

- **User Goal:** Summarize overall patterns, trends, or distributions across regions.
- **Task:** Read the big picture from a cartogram rather than inspect exact local relationships.
- **Data:** Geospatial regions with values encoded by size.
- **Chart Setting:** A static summary view where the map is used to communicate broad spatial structure.
- **Success Criterion:** Better pattern-summary accuracy.

## Do not use when detailed geography is part of the task <!-- role: exceptions -->

**Break it when:** Geographic locations and adjacencies are important and readers need detailed map reading. **Why:** Dorling cartograms do not preserve shape or topology well enough for those tasks.

## Tradeoffs of using a Dorling cartogram for overview <!-- role: costs -->

**Sacrifice:** Exact region shape and exact adjacency.
**Risk:** Readers may not be able to use the chart for neighbor-finding or shape recognition.
**Mitigation:** If detailed location and adjacency also matter, switch to a contiguous cartogram.

## Common failure mode for pattern summary <!-- role: mistakes -->

**Mistake:** Using a rectangular cartogram for a big-picture summary. **Why it fails:** The severe distortion of shapes and positions makes broad pattern reading less accurate.

## Check whether the overview is readable <!-- role: check -->

**Failure Sign:** Readers miss the overall spatial pattern even though the values are present.
**Quick Check:** Ask one summary question on the current cartogram and on a Dorling alternative.
**Stronger Test:** Compare summary accuracy between the current view and a Dorling version on the same broad-pattern questions.

## Fix the overview failure <!-- role: fix -->

- Replace the rectangular cartogram with a Dorling cartogram.
- Use circles sized by the regional value to simplify the overall pattern.
- If the chart must also support detailed geographic lookup, switch to a contiguous cartogram instead.
