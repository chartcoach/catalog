---
id: use-quantile-breaks-to-evenly-distribute-classed-map-colors
title: Use quantile interpolation when linear class breaks leave most regions in one
  class
bibliography: references.bib
description: For regional comparison on outlier-rich classed maps, use quantile interpolation
  on choropleth color scales to improve pattern visibility and address underused darker
  classes for readers comparing regions.
labels:
- purpose:refine
- basis:heuristic
- task:compare
- chart:choropleth
- data:geospatial
- quality:insight
- lever:encoding
- shape:outlier-rich
---

## Equal-count class breaks <!-- role: advice -->

Use quantile interpolation on a classed color scale when outliers make linear breaks waste most of the darker colors. For example, split the regions into equal-count classes such as quintiles so each color fills a similar number of areas, instead of leaving most areas in the lightest class under linear or rounded breaks.

## Why quantile breaks reveal more variation <!-- role: reason -->

Quantile interpolation redistributes the color steps across regions rather than across numeric distance. That makes more of the palette visible when the data are crowded into one part of the range.

**Mechanism:** Each class receives the same number of regions, so dark and medium colors appear often enough to expose regional differences that linear breaks can hide.

**Evidence:** The article shows that quantile breaks spread the colors evenly across regions when outliers compress the range, but also warns that this can make high values seem more common than they are [@muth_interpolation_2022].

**Notes:** In the article, quantile interpolation is discussed as a classed-scale option.

## Use when equal color usage is the goal <!-- role: context -->

- **User Goal:** Reveal geographic differences across many regions, not just highlight a few extremes.
- **Task:** Compare regions by broad level rather than preserve exact numeric spacing.
- **Data:** Quantitative regional values with strong outliers that push most regions into one low class under linear breaks.
- **Chart Setting:** A classed choropleth with multiple discrete color steps.
- **Success Criterion:** Each color is used across a similar number of regions, making more regional variation visible.

## Do not use quantile breaks when rarity must stay obvious <!-- role: exceptions -->

**Break it when:** The map must make clear that only a small minority of regions are true outliers. **Why:** Quantile interpolation can imply that high values are common because the darkest class covers as many regions as the lightest class.

## Tradeoffs of equal-count breaks <!-- role: costs -->

**Sacrifice:** You give up direct proportional spacing of the numeric values.
**Risk:** The map can make the highest values look more widespread than they really are.
**Mitigation:** Switch to a distribution-aware interpolation if you need both visible variation and clear rarity.

## Common failure with quantile breaks <!-- role: mistakes -->

**Mistake:** Using quantile interpolation just because it makes the map look more varied. **Why it fails:** Equal color usage can overstate how common the highest values are.

## How to test whether quantile breaks are justified <!-- role: check -->

**Failure Sign:** A linear or rounded classed map puts most regions into one light class.
**Quick Check:** Count how many regions fall into each color; if one class dominates and the goal is regional comparison, quantile is a candidate.
**Stronger Test:** Compare a linear version with a quantile version and reject quantile if the darker classes start implying too many high-value regions.

## What to change if linear class breaks underuse the palette <!-- role: fix -->

- Change the classed interpolation from linear or rounded to quantile.
- Match the quantile segmentation to the number of color steps already in the map.
- Keep quantile only when even color distribution across regions is the point of the map.
- Replace quantile with a distribution-aware interpolation if it makes extreme values look too common.
