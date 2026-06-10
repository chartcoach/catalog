---
id: use-clear-lightness-progression-in-ordered-map-colors
title: Use clear lightness progression in ordered map colors
bibliography: references.bib
description: For overview reading of choropleth values, use clear lightness progression
  in sequential and diverging color schemes to improve readability and mitigate slow
  detection of low and high regions.
labels:
- purpose:refine
- basis:heuristic
- chart:choropleth
- quality:readability
- lever:encoding
- channel:color-lightness:use
- reading-mode:overview
---

## Lightness ordering <!-- role: advice -->

Build ordered choropleth palettes around lightness differences, not just hue changes. For example, make sequential schemes run from light to dark, and make diverging schemes lightest in the middle with darker extremes on both sides.

## Why lightness speeds map reading <!-- role: reason -->

Readers detect low and high regions faster when the palette changes in brightness as well as color.

**Mechanism:** Lightness progression gives an immediate cue to order. It helps viewers spot low and high values quickly without first decoding hue relationships.

**Evidence:** The post says a gradient from a light color to a dark color helps readers quickly spot low and high values, and that diverging schemes should be lightest in the middle and darkest at the extremes [@muth_choroplethmaps_2018].

## Use when color encodes ordered values <!-- role: context -->

- **User Goal:** Let readers spot low and high regions quickly.
- **Task:** Overview reading of ordered values on a map.
- **Data:** Ordered values shown with sequential or diverging color.
- **Chart Setting:** A choropleth is already chosen.
- **Audience:** Readers scanning the map rather than reading exact numbers.
- **Success Criterion:** Low, middle, and high regions separate visually at a glance.

## Do not use when the color scheme is qualitative <!-- role: exceptions -->

**Break it when:** The color scheme represents unordered categories. **Why:** The post says qualitative schemes should not suggest sequential or diverging order when the data is not ordered.

## Costs of emphasizing lightness <!-- role: costs -->

**Sacrifice:** You give up some decorative color variety.
**Risk:** Too much hue variation can overdo the contrast.
**Mitigation:** Let lightness carry the ordering and keep extra hue changes restrained.

## Common hue-only failure <!-- role: mistakes -->

**Mistake:** Use ordered map colors that change hue but not lightness. **Why it fails:** Readers have a harder time locating the lowest and highest values quickly.

## Check whether the palette has visible order <!-- role: check -->

**Failure Sign:** The legend colors do not show a clear progression from low to high.
**Quick Check:** Inspect the color key and verify a visible light-to-dark sequence, or dark-to-light-to-dark around the midpoint.
**Stronger Test:** Compare the current palette to a stronger lightness-ordered version and keep the one that makes extremes easier to spot.

## Edit the palette for stronger ordering <!-- role: fix -->

- Increase the lightness contrast across the ordered scale.
- Set the darkest shades at the extremes of the value range.
- Set the lightest shade at the midpoint of a diverging scale.
- Remove unnecessary hue changes that overpower the lightness order.
