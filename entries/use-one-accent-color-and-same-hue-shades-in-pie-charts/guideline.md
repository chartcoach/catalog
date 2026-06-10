---
id: use-one-accent-color-and-same-hue-shades-in-pie-charts
title: Use one accent color and same-hue shades in a pie chart
bibliography: references.bib
description: For emphasizing one important share in a pie chart, use a focused slice-color
  palette to improve readability and mitigate distracting rainbow colors for readers.
labels:
- purpose:refine
- basis:heuristic
- chart:pie-donut
- lever:encoding
- quality:readability
- polish:palette
- aesthetic:color:use
- channel:color-hue:use
---

## Refine the slice palette <!-- role: advice -->

Color the most important slice with a standout color and keep the other slices in shades of one color. For example, make one slice pop and avoid using rainbow colors across the remaining wedges.

## Why a focused pie palette works <!-- role: reason -->

The palette can direct attention to the key slice without making the rest of the pie noisy. Using many unrelated hues pulls attention away from comparing the shares.

**Mechanism:** One accent color establishes the focal slice, while same-hue shades keep the other slices comparable instead of competing for attention.

**Evidence:** The source recommends using colors to make the most important value stand out, using shades of one color for the rest, and warns that rainbow colors distract readers from comparing pie shares [@muth_pie_charts_2018].

## Use when one slice matters most <!-- role: context -->

- **User Goal:** Emphasize one important share in a pie chart.
- **Data:** One total split into slices, with one value treated as the key value.
- **Chart Setting:** A pie chart has already been chosen.
- **Success Criterion:** The key slice stands out without making the remaining slices harder to compare.

## Do not use when no slice should be emphasized <!-- role: exceptions -->

**Break it when:** The chart does not have one most important value to highlight. **Why:** The rule is specifically for making one slice stand out against the others.

## Tradeoffs of using a focused palette <!-- role: costs -->

**Sacrifice:** You give up a more varied color scheme.
**Risk:** Many unrelated hues distract from comparing slice sizes.
**Mitigation:** Keep one accent color for the key slice and use same-hue shades for the rest.

## Common misuse of pie colors <!-- role: mistakes -->

**Mistake:** Coloring many slices with rainbow hues. **Why it fails:** The colors distract readers from comparing the shares.

## Check whether the palette is focused enough <!-- role: check -->

**Failure Sign:** Several slices compete equally for attention or the pie reads like a rainbow.
**Quick Check:** Look for one clear accent color and same-hue shades on the other slices.
**Stronger Test:** Compare the current palette with a one-accent version and keep the one where the key slice is clearer.

## Fix the slice palette <!-- role: fix -->

- Pick one standout color for the most important slice.
- Recolor the remaining slices as shades of one color.
- Remove rainbow hues from the non-key slices.
