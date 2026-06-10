---
id: use-ensemble-members-when-uncertainty-boundaries-could-imply-physical-growth
title: Use ensemble-member encoding when uncertainty boundaries could imply physical
  growth
bibliography: references.bib
description: For area-level interpretation of geospatial uncertainty over time, use
  ensemble-member encoding on maps to improve fidelity and mitigate physical-growth
  misreadings for novice audiences.
labels:
- purpose:refine
- basis:empirical
- chart:map
- data:geospatial
- time:ordered-time
- quality:fidelity
- lever:encoding
- operator:uncertainty
- literacy:novice
---

## Use ensemble-member paths <!-- role: advice -->

Encode geospatial uncertainty with individual ensemble members when an enclosing boundary would widen over the forecast and could be read as the phenomenon's physical extent. For example, on a forecast map, draw multiple plausible paths instead of a widening cone or other summary outline when readers need to judge uncertainty spread, size, or intensity over time.

## Why ensemble-member paths improve uncertainty reading <!-- role: reason -->

An expanding boundary becomes a highly salient shape on the map, so readers can mistake uncertainty growth for physical growth of the phenomenon itself. Individual ensemble members shift attention toward the distribution of possible outcomes instead of toward one enlarging outline.

**Mechanism:** Ensemble-member encoding makes the spread of possible paths visible, which supports interpretations of uncertainty distribution and reduces the chance that a widening boundary will be read as size or intensity change.

**Evidence:** In map-based hurricane forecasts for novice viewers, summary boundary displays produced larger size and intensity judgments over time and were more often reported as showing the storm getting larger, while ensemble displays reduced those errors and better conveyed increasing forecast uncertainty [@padillaEffectsEnsembleSummary2017].

**Notes:** The paper argues that summary displays are most effective when spatial boundaries cannot be misconstrued as physical boundaries.

## When this applies <!-- role: context -->

- **User Goal:** Understand how uncertainty spreads over the map and how the phenomenon changes over time.
- **Task:** Overview or area-level interpretation of uncertainty, size, intensity, or likely impact.
- **Data:** Geospatial forecast data with uncertainty across future positions.
- **Chart Setting:** A static map where a summary boundary would visibly widen through time.
- **Audience:** Novice readers.
- **Success Criterion:** Readers interpret widening as uncertainty growth rather than as physical growth.

## When not to use it <!-- role: exceptions -->

**Break it when:** The task requires judgments about exact points or pairwise point locations. **Why:** Viewers can overweight a single ensemble member that happens to cross the point.

## Tradeoffs of ensemble-member encoding <!-- role: costs -->

**Sacrifice:** You give up the compact single-boundary summary.
**Risk:** Plotting many ensemble members can create visual crowding and make paths hard to differentiate.
**Mitigation:** Use this approach when the paths can still be visually separated well enough for the intended overview task.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keeping a widening uncertainty boundary as the main cue on the map when readers can also interpret that boundary as physical size. **Why it fails:** Readers can infer that the phenomenon grows larger or stronger over time from the boundary itself.

## How to test it <!-- role: check -->

**Failure Sign:** Readers say the display shows the phenomenon getting larger over time or judge later central positions as larger or stronger.
**Quick Check:** Show the map to novice readers and ask whether the display shows physical growth or growing uncertainty.
**Stronger Test:** Compare size or intensity judgments from the boundary version against an ensemble-member version of the same forecast.

## What to change <!-- role: fix -->

- Replace the enclosing uncertainty boundary with individual ensemble members.
- Remove widening boundary shapes from displays intended for novice overview reading.
- Re-test size and intensity interpretation after the change.
