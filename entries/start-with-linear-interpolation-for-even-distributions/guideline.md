---
id: start-with-linear-interpolation-for-even-distributions
title: Start with linear interpolation when values are evenly distributed or when
  outliers should stand out
bibliography: references.bib
description: For initial interpolation review on regional maps with fairly even values
  or deliberate outlier emphasis, use linear interpolation on choropleth color scales
  to improve fidelity and address premature redistribution of the scale for designers
  evaluating alternatives.
labels:
- purpose:refine
- basis:heuristic
- chart:choropleth
- data:geospatial
- quality:fidelity
- lever:encoding
- communication:workflow
- audience:designer
---

## Linear interpolation first <!-- role: advice -->

Start the color scale with linear interpolation when the values are fairly even or when the map should make outliers pop. For example, map the minimum and maximum directly to the lightest and darkest colors, and keep that linear mapping if the distribution has no strong outliers or if only the highest regions should receive the darkest color.

## Why linear interpolation is the default baseline <!-- role: reason -->

Linear interpolation preserves the numeric spacing of the data on the color scale. That makes it a reliable baseline and a direct way to reserve the darkest colors for true extremes.

**Mechanism:** Values keep their original distance from each other on the scale, so evenly distributed data stay visually proportional and extreme values remain isolated by color.

**Evidence:** The article recommends linear interpolation as the default starting point and shows that it works best for fairly even distributions while also drawing strong attention to outliers [@muth_interpolation_2022].

**Notes:** This guidance applies to both classed and unclassed color scales in the article.

## Use when linear spacing matches the data <!-- role: context -->

- **User Goal:** Start choosing an interpolation without distorting the original scale.
- **Data:** Quantitative regional values with a fairly even spread, or values where a few extremes should stand apart.
- **Chart Setting:** A choropleth with a sequential color scale, classed or unclassed.
- **Audience:** Designers comparing interpolation options before finalizing the map.
- **Success Criterion:** The map preserves direct numeric spacing and uses the darkest colors mainly for true extremes.

## Do not keep linear when it flattens the bulk of the data <!-- role: exceptions -->

**Break it when:** The values have extreme outliers and the map needs to show geographic differences among the many low-to-mid values. **Why:** Linear interpolation can push most regions into very similar light colors.

## Tradeoffs of keeping the scale linear <!-- role: costs -->

**Sacrifice:** You give up some visible variation among the many common values.
**Risk:** On skewed data, most regions can collapse into one light color range.
**Mitigation:** Compare a linear version with a distribution-aware version before finalizing the map.

## Common failure with linear interpolation <!-- role: mistakes -->

**Mistake:** Keeping linear interpolation after seeing that most regions share the same light shade. **Why it fails:** It hides differences in the part of the distribution where most regions actually sit.

## How to test whether linear still works <!-- role: check -->

**Failure Sign:** Most regions appear in the lightest class or near the bright end of the gradient.
**Quick Check:** Inspect the distribution first; if the values cluster far from the maximum, linear may be compressing too much of the map.
**Stronger Test:** Compare a linear version with a distribution-aware version and keep linear only if it does not wash out the main regional patterns you need to show.

## What to change if linear is not working <!-- role: fix -->

- Keep linear interpolation as the starting version of the map.
- Retain linear interpolation when the distribution is fairly even.
- Retain linear interpolation when the goal is to make outliers stand out clearly.
- Replace linear interpolation only after checking that it suppresses important variation among the non-outlier regions.
