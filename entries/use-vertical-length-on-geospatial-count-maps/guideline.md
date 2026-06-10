---
id: use-vertical-length-on-geospatial-count-maps
title: Use vertical length encoding for geospatial counts when 2D overlap is a problem
bibliography: references.bib
description: For compare tasks on geospatial count displays with dense overlap and
  long-tailed values, use vertical length encoding on anchored map marks to improve
  fidelity and address overplotting for readers comparing both large and small counts.
labels:
- purpose:refine
- basis:empirical
- task:compare
- data:geospatial
- quality:fidelity
- lever:encoding
- channel:length:use
- shape:skewed
---

## Vertical height on map marks <!-- role: advice -->

Use anchored vertical height for geospatial counts when 2D symbol overlap or weak magnitude channels make comparison hard. For example, replace hue, brightness, or overlapping proportional circles with 3D pins or bars whose height encodes the count at each mapped location.

## Why height works better here <!-- role: reason -->

Length remains a strong quantitative channel, and anchoring the mark to the map keeps the location unambiguous. In the paper's map example, height supports comparison of both dominant locations and much smaller locations while avoiding the low discrimination of brightness and the higher estimation error of circle area.

**Mechanism:** Vertical length gives readers a more discriminable magnitude cue than hue or brightness, while the anchored base of the 3D mark makes the spatial reference point clearer than the center of a large or overlapping circle.

**Evidence:** The paper argues that 3D pin heights on maps can support accurate relative comparison for both large and small counts, while 2D alternatives such as hue, brightness, and proportional circles provide fewer discriminable levels, higher area-estimation error, and overlap problems; it also notes that this works best when the data are long-tailed enough to keep occlusion low [@brath3DInfoVisHere2014].

## Use when map counts would collide in 2D <!-- role: context -->

- **User Goal:** Compare magnitudes across mapped locations.
- **Task:** Judge both very large and relatively small location counts in one view.
- **Data:** Count-like values attached to geographic positions, especially with a long-tailed distribution.
- **Chart Setting:** A map with spatially anchored marks where 2D circles or color fills would overlap or compress the scale.
- **Audience:** Readers who need relative size judgments more than decorative map effects.
- **Success Criterion:** Large and small differences stay visible without ambiguous mark centers or severe overplotting.

## When this breaks <!-- role: exceptions -->

**Break it when:** Many locations produce similarly tall marks that heavily occlude one another. **Why:** The paper treats low occlusion as a key condition for the 3D benefit; once occlusion dominates, the comparison advantage erodes.

## What you trade away <!-- role: costs -->

**Sacrifice:** You give up some of the simplicity of a flat 2D map.
**Risk:** A crowded field of tall marks can create occlusion and navigation burden.
**Mitigation:** Keep the view to cases where the data shape leaves only a few tall outliers and many short marks.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keep the mapped counts in hue, brightness, or overlapping circles when the main job is precise relative comparison. **Why it fails:** Those encodings offer fewer usable levels, higher estimation error, or ambiguous centers in dense regions.

## How to check it <!-- role: check -->

**Failure Sign:** Small nearby values blur together, or large circles cover one another and obscure their exact locations.
**Quick Check:** From one static view, compare a few small values and a few large values; if both comparisons are hard, the encoding is too weak.
**Stronger Test:** Put the same data in a height-encoded map and in a hue- or area-encoded map, then see which one preserves both small and large differences without overlap.

## What to change <!-- role: fix -->

- Replace hue or brightness magnitude coding with anchored vertical height.
- Replace overlapping proportional circles with pins or bars whose base clearly marks the location.
- If tall marks still collide, stop using this 3D encoding for that data slice.
