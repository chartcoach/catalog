---
id: encode-regional-values-with-framed-rectangles-instead-of-shading
title: Encode regional values with framed rectangles instead of shading
bibliography: references.bib
description: For regional quantitative comparison, use framed-rectangle encoding on
  statistical maps to improve judgment fidelity and mitigate shading, area, and clustering
  errors for readers comparing regions.
labels:
- purpose:refine
- basis:empirical
- chart:map
- data:geospatial
- quality:fidelity
- lever:encoding
- channel:position:use
- channel:color-saturation:avoid
---

## Framed-rectangle encoding <!-- role: advice -->

Replace regional shading with framed rectangles when readers must compare quantitative values on a map. For example, draw an equal frame in each region and encode the value by the filled height inside the frame rather than by fill density or texture across the whole area.

## Why framed rectangles work <!-- role: reason -->

Shaded statistical maps ask readers to judge shading or color saturation, which the paper places at the bottom of the perceptual accuracy order. Framed rectangles turn the task into reading bar-like heights, and they also prevent large regions from seeming more important just because they occupy more area.

**Mechanism:** Equal frames give every region the same visual measurement device, so readers compare value by the height inside the frame instead of by region fill. That reduces both low-accuracy shading judgments and distortions created by unequal geographic areas.

**Evidence:** The paper ranks shading and color saturation among the least accurate perceptual tasks and applies that result to statistical maps. Its framed-rectangle redesign also corrects distortions from differing region areas and reduces spurious regional clustering caused by coarse shading [@clevelandGraphicalPerceptionTheory1984].

## Use when map readers must compare region values <!-- role: context -->

- **User Goal:** Compare quantitative values across regions.
- **Task:** Identify large and small regional values and compare nearby areas.
- **Data:** One quantitative value per geographic region.
- **Chart Setting:** A statistical map currently uses shading, texture, or color saturation to encode value.
- **Audience:** Readers making visual regional comparisons.
- **Success Criterion:** Region values are easier to compare without area-driven distortion or false clusters.

## Do not use when the symbols become too small to compare <!-- role: exceptions -->

**Break it when:** The framed rectangles would have to be reduced so much that height differences become optically hard to detect. **Why:** The source notes that the method works only until the symbols become too small for visible differences.

## Tradeoffs of using framed rectangles <!-- role: costs -->

**Sacrifice:** Filled regions are replaced by small in-region bars.
**Risk:** If the rectangles are made too small, optical detection of differences drops.
**Mitigation:** Keep the rectangles large enough to compare, or coarsen the value steps with grouped intervals or reduced vertical resolution.

## Common failure with shaded maps <!-- role: mistakes -->

**Mistake:** Rely on shading or texture alone for regional value comparisons. **Why it fails:** Readers must judge a low-accuracy channel, large regions become visually imposing, and similar shades can create misleading clusters.

## Check whether the map is distorting the values <!-- role: check -->

**Failure Sign:** Large regions look important even when their values are modest, or similar tones create apparent regional clusters.
**Quick Check:** Ask a reviewer to compare a large low-valued region with a small high-valued region and to rank a few nearby regions by value.
**Stronger Test:** Replace the shading with framed rectangles and see whether extremes and regional differences become easier to spot.

## Fix the map <!-- role: fix -->

- Draw equal frames inside regions and fill each frame to the encoded value.
- Stop encoding the value only by shading, texture, or color saturation across the full region area.
- If the map is noisy, group the values into equal-length intervals before drawing the rectangles.
- If you want stronger visual grouping, reduce the vertical resolution of the rectangles only while their differences remain optically visible.
