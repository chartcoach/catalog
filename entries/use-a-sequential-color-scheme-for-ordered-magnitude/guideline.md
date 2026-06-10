---
id: use-a-sequential-color-scheme-for-ordered-magnitude
title: Use a sequential color scheme for ordered magnitude
bibliography: references.bib
description: For overview comparison of one ordered regional measure, use a sequential
  color scheme on a choropleth to improve readability and mitigate weak emphasis of
  high values for readers scanning the map.
labels:
- purpose:refine
- basis:heuristic
- chart:choropleth
- quality:readability
- lever:encoding
- channel:color-lightness:use
- measure:single
- reading-mode:overview
---

## Sequential palette choice <!-- role: advice -->

Use a sequential color scheme when the choropleth encodes one ordered measure and you want high values to stand out. For example, run the fill from a lighter shade to a darker shade so the darkest regions carry the highest values.

## Why one-direction scales fit one-direction data <!-- role: reason -->

A one-direction scale matches the way readers scan ordered magnitude on a map.

**Mechanism:** A sequential scheme gives viewers one visual direction from low to high. That makes the regions with larger values easy to locate during an overview read.

**Evidence:** The post recommends a sequential color scheme when attention should go to high values such as unemployment rates [@muth_choroplethmaps_2018].

## Use when one side of the scale matters most <!-- role: context -->

- **User Goal:** Show where values are low versus high.
- **Task:** Scan the map for the largest values.
- **Data:** One ordered regional variable.
- **Chart Setting:** A choropleth is already chosen.
- **Audience:** Readers doing an overview read of magnitude.
- **Success Criterion:** High-value regions stand out quickly.

## Do not use when both extremes or categories matter <!-- role: exceptions -->

**Break it when:** The message depends on both extremes around a meaningful center, or the data is unordered categories. **Why:** The post recommends diverging schemes for both extremes and qualitative schemes for unordered data.

## Costs of a one-direction palette <!-- role: costs -->

**Sacrifice:** You do not give equal emphasis to both ends of the scale.
**Risk:** Extra hue changes can overstate contrast.
**Mitigation:** Let the light-to-dark progression do most of the work and keep added hue changes restrained.

## Common palette mismatch <!-- role: mistakes -->

**Mistake:** Use a qualitative-looking or center-splitting palette for one ordered measure. **Why it fails:** The map stops giving a clear low-to-high reading and high values no longer stand out cleanly.

## Check whether the palette matches the data <!-- role: check -->

**Failure Sign:** The highest regions do not stand out immediately.
**Quick Check:** Read the legend from low to high and confirm that the colors move in one clear direction toward a darker end.
**Stronger Test:** Compare the sequential draft with a non-sequential draft and keep the version that isolates high-value regions faster.

## Edit the palette for ordered magnitude <!-- role: fix -->

- Replace the fill palette with a sequential scheme.
- Map the lowest values to the lightest shade and the highest values to the darkest shade.
- Remove unnecessary hue reversals or center colors.
- Recheck the legend so it reads in one low-to-high direction.
