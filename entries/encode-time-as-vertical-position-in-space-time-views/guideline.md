---
id: encode-time-as-vertical-position-in-space-time-views
title: Encode time as vertical position when 2D overlap hides movement
bibliography: references.bib
description: For ordered-time analysis of geospatial trajectories, use vertical position
  for time on a 3D space-time view to improve insight and address overlapping 2D traces
  for readers reconstructing movement patterns.
labels:
- purpose:refine
- basis:empirical
- task:trend
- time:ordered-time
- data:geospatial
- quality:insight
- lever:encoding
- channel:position:use
---

## Vertical time separation <!-- role: advice -->

Move time into a vertical spatial axis when a 2D map view piles different moments on top of the same places. For example, lift spatio-temporal points into a 3D space-time cube so repeated positions over time form a readable trajectory or oscillation instead of a flat overlapping cloud.

## Why the third axis helps here <!-- role: reason -->

Separating time from map position lets viewers see sequence and motion directly rather than infer it from overlapping marks or weak brightness changes. The paper contrasts a crowded 2D spatio-temporal view with a 3D view where the vertical time axis makes the movement pattern visible.

**Mechanism:** The extra axis creates spatial separation for successive time points, so order and repeated movement become visible as structure instead of staying hidden inside overplotting.

**Evidence:** The paper argues that the third dimension can make time more visibly distinguishable than 2D brightness coding, and its space-time example shows that vertical time encoding reveals oscillation that is hard to perceive in the overlapping 2D view [@brath3DInfoVisHere2014].

## Use when time is colliding with place <!-- role: context -->

- **User Goal:** Reconstruct motion or sequence through geographic space.
- **Task:** See what came before and after, and identify repeated or oscillating movement.
- **Data:** Time-stamped locations or geotemporal point data.
- **Chart Setting:** A mapped point or trajectory display where multiple times occupy the same or nearby positions.
- **Audience:** Readers who need pattern visibility more than a flat map-only view.
- **Success Criterion:** Movement order is visible directly from the geometry rather than inferred from overlapping points.

## When this breaks <!-- role: exceptions -->

**Break it when:** The 3D points are effectively non-anchored and the scene lacks enough cues to decode depth. **Why:** The paper notes that random 3D point locations cannot be determined reliably without additional perspective cues or supportive data structure.

## What you trade away <!-- role: costs -->

**Sacrifice:** You give up the simplicity of a flat map.
**Risk:** Readers may struggle with depth if the 3D scene does not provide enough positional cues.
**Mitigation:** Use this move where the temporal structure itself or other scene cues make the 3D position readable.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Leave time in a 2D overlapping map and try to rescue the sequence with brightness alone. **Why it fails:** The ordering and movement pattern remain hard to perceive when points occupy the same space.

## How to check it <!-- role: check -->

**Failure Sign:** Readers can see where points are but cannot tell the direction, repetition, or oscillation over time.
**Quick Check:** Ask whether the temporal path is visible from the geometry itself rather than from labels or memory.
**Stronger Test:** Compare the same data in a 2D overlapping map and in a 3D vertical-time view, then inspect which one makes the movement pattern directly readable.

## What to change <!-- role: fix -->

- Add a vertical axis dedicated to time.
- Separate repeated locations by placing successive time points at different heights.
- If the lifted points still feel ambiguous, add stronger depth cues or use a view whose data structure gives clearer spatial cues.
