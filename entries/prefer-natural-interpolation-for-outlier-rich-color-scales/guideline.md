---
id: prefer-natural-interpolation-for-outlier-rich-color-scales
title: Prefer natural interpolation when clustered values and outliers need different
  treatment
bibliography: references.bib
description: For regional comparison on outlier-rich value maps, prefer natural interpolation
  on choropleth color scales to improve fidelity and mitigate the tradeoff between
  washed-out linear scales and overstated equal-count scales for readers scanning
  geographic patterns.
labels:
- purpose:refine
- basis:heuristic
- task:compare
- chart:choropleth
- data:geospatial
- quality:fidelity
- lever:encoding
- shape:outlier-rich
---

## Distribution-aware interpolation <!-- role: advice -->

Prefer natural interpolation when values cluster tightly in one part of the range but a few outliers sit far away. For example, use Natural breaks for classed scales or Natural interpolation for continuous scales so clustered midrange regions separate into several colors while only a few true outliers get the darkest shade.

## Why natural interpolation balances pattern and rarity <!-- role: reason -->

Natural interpolation follows the actual grouping in the data instead of forcing equal numeric spacing or equal counts. That makes it useful when the map needs to show both internal variation and true outliers.

**Mechanism:** Closely packed values are grouped together while far-apart outliers are separated more aggressively, so the map shows meaningful regional variation without pretending extreme values are common.

**Evidence:** The article presents natural interpolation as the compromise that respects the distribution, reveals differences around the middle of the data, and still leaves only a few regions as clear outliers [@muth_interpolation_2022].

**Notes:** The article discusses this logic for both classed and unclassed color scales.

## Use when the data are clustered with a few far-apart extremes <!-- role: context -->

- **User Goal:** Show geographic patterns across the common values while still signaling that only a few regions are extreme.
- **Task:** Compare regions across an uneven distribution.
- **Data:** Quantitative regional values with dense clustering and a small number of far-apart outliers.
- **Chart Setting:** A choropleth with a classed or unclassed sequential color scale.
- **Success Criterion:** Several colors appear across the main cluster, but the darkest shade is still reserved for only a few regions.

## Do not use natural interpolation when the simple scale already fits the story <!-- role: exceptions -->

**Break it when:** The values are fairly even, or the main point is to draw immediate attention to outliers alone. **Why:** Linear interpolation already serves those cases more directly.

## Tradeoffs of natural interpolation <!-- role: costs -->

**Sacrifice:** You give up simple evenly spaced break values.
**Risk:** The resulting thresholds can be awkward decimals that are hard to read in the legend.
**Mitigation:** Round the thresholds afterward with custom breaks if the map impression stays the same.

## Common failure with natural interpolation decisions <!-- role: mistakes -->

**Mistake:** Staying with linear or equal-count interpolation after they clearly force the map to one side of the tradeoff. **Why it fails:** Linear can hide the main cluster, while equal-count can make extremes look too common.

## How to test whether natural interpolation is the better compromise <!-- role: check -->

**Failure Sign:** Linear leaves most regions near one light color, while equal-count interpolation makes dark colors too common.
**Quick Check:** Inspect the distribution; if many values are tightly packed and a few are far away, natural interpolation is a better match.
**Stronger Test:** Compare linear, equal-count, and natural versions and keep natural if it reveals midrange patterns while reserving the darkest color for only a few regions.

## What to change when linear and equal-count both mislead <!-- role: fix -->

- Change the interpolation to Natural breaks on a classed scale.
- Change the interpolation to Natural on a continuous scale.
- Keep the same palette and let the breakpoints follow the clusters in the data.
- If the legend becomes hard to read, round the resulting thresholds and compare the map again.
