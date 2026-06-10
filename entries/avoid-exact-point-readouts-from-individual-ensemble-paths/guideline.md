---
id: avoid-exact-point-readouts-from-individual-ensemble-paths
title: Avoid exact-point readouts from individual ensemble paths
bibliography: references.bib
description: For exact location judgments on geospatial uncertainty maps, avoid using
  individual ensemble-member paths as the readout to prevent overweighting single
  members and mitigate biased point decisions for novice audiences.
labels:
- purpose:refine
- basis:empirical
- chart:map
- data:geospatial
- quality:fidelity
- lever:encoding
- operator:uncertainty
- reading-mode:exact
- literacy:novice
---

## Do not treat path overlap as an exact-point signal <!-- role: advice -->

Avoid using whether a single ensemble member crosses a point as the main readout for exact-location decisions. For example, do not ask viewers to decide which of two nearby locations is at greater risk from an ensemble-path map when one location sits on a path and the other is slightly nearer the center, because the crossed location attracts responses.

## Why exact-point readouts fail on ensemble paths <!-- role: reason -->

A visible path crossing is a salient local feature, so readers can treat one sampled path as if it were a decisive route rather than one draw from a distribution. That makes exact-point judgments shift toward crossed locations even when another nearby location better matches the overall distribution.

**Mechanism:** Individual path crossings compete with distribution-based reading and bias exact point comparisons toward the crossed point.

**Evidence:** In point-based damage judgments from ensemble hurricane forecasts, novice viewers almost always chose the nearer location when it was on a path, but they shifted strongly toward a farther location when that farther location was the one crossed by a path; the effect remained when an equal-damage option was added [@padillaEffectsEnsembleSummary2017].

**Notes:** The paper suggests ensemble displays are better suited to pattern, area, and gist judgments than to point-based judgments.

## When this applies <!-- role: context -->

- **User Goal:** Make a location-specific decision about one point versus another.
- **Task:** Exact point comparison.
- **Data:** Geospatial uncertainty shown as multiple possible paths.
- **Chart Setting:** A static ensemble display where individual paths visibly cross some candidate locations.
- **Audience:** Novice readers.
- **Success Criterion:** Path overlap does not distort which location is judged more at risk.

## When not to use it <!-- role: exceptions -->

**Break it when:** The task is to judge overall patterns, areas, or spread rather than exact points. **Why:** The paper argues that ensemble displays are better suited to those non-point tasks.

## Tradeoffs of avoiding exact-point readouts <!-- role: costs -->

**Sacrifice:** You lose an apparently direct point cue from visible path crossings.
**Risk:** If you ignore this rule, readers can treat sampled paths as exhaustive routes or as full-storm tracks.
**Mitigation:** Use the ensemble display for area or pattern interpretation instead of point comparison.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Letting viewers infer that a point on one visible path is more likely to be hit than a nearby point off the path. **Why it fails:** Readers overweight the single visible path even when the off-path point is closer to the center of the distribution.

## How to test it <!-- role: check -->

**Failure Sign:** A farther point is chosen much more often once it happens to lie on a single path.
**Quick Check:** Create paired-location cases where one farther point lies on a path and one nearer point does not, then compare the choices.
**Stronger Test:** Repeat the paired-location check with an equal-outcome option and see whether path overlap still shifts choices away from the nearer point.

## What to change <!-- role: fix -->

- Remove exact-point comparison tasks from ensemble-path displays.
- Reframe the judgment around areas, spread, or overall pattern instead of a single crossed point.
- If exact-point decisions are required, do not rely on the ensemble-path display alone.
