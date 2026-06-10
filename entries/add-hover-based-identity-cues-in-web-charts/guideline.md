---
id: add-hover-based-identity-cues-in-web-charts
title: Add hover-based identity cues in interactive color-coded charts
bibliography: references.bib
description: For interactive web charts, prefer hover-based highlighting and tooltips
  on color-coded marks to improve identification and mitigate color-only decoding
  for readers with color-vision deficiency.
labels:
- purpose:refine
- basis:heuristic
- quality:accessibility
- lever:interaction-access
- component:tooltip:use
- needs:color-vision-deficiency
- access:noncolor:use
---

## Reveal identity on hover <!-- role: advice -->

Add hover behavior that identifies the hovered color-coded item without relying on color alone. For example, highlight matching marks from the legend, fade the nonhovered series, or show the color-coded category information inside a tooltip.

## Why hover cues help <!-- role: reason -->

Interactive charts can reveal identity at the moment the reader needs it. A hover state turns ambiguous color into an explicit label or highlight, which makes same-looking colors easier to decode.

**Mechanism:** Hover interaction creates a temporary noncolor cue that links the mark, its label, and related elements during inspection.

**Evidence:** The article recommends hover effects for web charts, gives examples where hovering over a legend highlights matching elements, hovering over a chart element highlights matching elements and the key, and tooltips include the color-coded information. [@muth_colorblindness_2020]

## Use when the chart is interactive and web-based <!-- role: context -->

- **User Goal:** Identify a hovered mark or series precisely.
- **Task:** Interactive lookup of color-coded categories.
- **Data:** Categories or regions encoded by color.
- **Chart Setting:** A web chart with hover interaction available.
- **Audience:** Readers who may include people with color-vision deficiency.
- **Success Criterion:** Hovering makes the category identity explicit even when the colors look similar.

## When hover cannot carry the fix <!-- role: exceptions -->

**Break it when:** The chart is static or printed. **Why:** The article presents hover cues specifically as a web-only aid.

## Costs of hover-based identity cues <!-- role: costs -->

**Sacrifice:** The chart depends on interaction for full clarity.
**Risk:** Readers may not discover the identity cue until they hover.
**Mitigation:** Make the hover state obvious by visibly highlighting the hovered mark and dimming the rest.

## Common hover failure <!-- role: mistakes -->

**Mistake:** Adding a tooltip that omits the color-coded identity or keeping hover effects too subtle to reveal which marks belong together. **Why it fails:** The interaction does not actually solve the color-decoding problem.

## How to verify hover behavior <!-- role: check -->

**Failure Sign:** Hovering a mark does not clearly identify the category or related marks.
**Quick Check:** Hover one mark and confirm that the matching legend entry, related marks, or label become obvious.
**Stronger Test:** Use a colorblind simulation while hovering and verify that the interaction still reveals identity.

## What to change <!-- role: fix -->

- Highlight the matching chart elements when a legend item is hovered.
- Highlight the matching legend entry and fade unrelated marks when a chart element is hovered.
- Add the color-coded category information to the tooltip content.
