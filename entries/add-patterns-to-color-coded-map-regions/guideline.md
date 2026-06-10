---
id: add-patterns-to-color-coded-map-regions
title: Add patterns to map regions when confusing colors must remain
bibliography: references.bib
description: For color-coded maps, prefer texture encoding on filled regions to improve
  accessibility and mitigate confusing hue distinctions for readers with color-vision
  deficiency.
labels:
- purpose:refine
- basis:heuristic
- chart:map
- data:geospatial
- quality:accessibility
- lever:encoding
- channel:texture:use
- needs:color-vision-deficiency
---

## Layer pattern over region color <!-- role: advice -->

Add a pattern to a map region when adjacent areas would otherwise differ only by a hard-to-distinguish color pair. For example, keep the existing fills but overlay one region with a line pattern so neighboring countries or areas remain distinguishable even when the hues collapse.

## Why patterns help on maps <!-- role: reason -->

Filled geographic regions often depend on area color, and neighboring regions make confusion obvious. Pattern adds a second region identity that does not depend on hue alone.

**Mechanism:** Texture survives hue confusion and gives each filled area a visible difference even when the base colors look similar.

**Evidence:** The article shows a map that is unreadable to red-blind readers when adjacent regions differ only by color, then shows that adding a pattern solves the problem while keeping the same colors. [@muth_colorblindness_2020]

## Use when adjacent regions are color-only <!-- role: context -->

- **User Goal:** Distinguish neighboring regions on a map.
- **Task:** Identify or compare geospatial categories.
- **Data:** Filled geographic areas differentiated by color.
- **Chart Setting:** A map where confusing colors must stay in place.
- **Audience:** Readers who may include people with color-vision deficiency.
- **Success Criterion:** Neighboring regions remain clearly separate without relying only on hue.

## When the pattern needs adjustment <!-- role: exceptions -->

**Break it when:** The added pattern makes a region look falsely lighter or darker than intended. **Why:** The article warns that patterns change how bright or dark the colors are perceived.

## Costs of adding patterns <!-- role: costs -->

**Sacrifice:** You give up a fully smooth fill appearance.
**Risk:** The pattern can alter perceived lightness and distort the apparent color balance.
**Mitigation:** Recheck the region fills after the pattern is added and adjust the base colors if needed.

## Common map-pattern failure <!-- role: mistakes -->

**Mistake:** Adding a pattern without checking how it changes the apparent brightness of the fill. **Why it fails:** The map may become distinguishable but still mislead readers about which region looks lighter or darker.

## How to verify region patterns <!-- role: check -->

**Failure Sign:** The patterned region now appears much lighter or darker than the unpatterned region for reasons unrelated to the data.
**Quick Check:** Compare the map before and after the pattern to see whether the pattern has shifted perceived lightness.
**Stronger Test:** Run a colorblind simulation and confirm that both the region identity and the apparent lightness still make sense.

## What to change <!-- role: fix -->

- Overlay one of the confusing regions with a clear pattern.
- Rebalance the base fill colors if the pattern changes perceived brightness too much.
- Keep the pattern only where it solves a real color-confusion problem.
