---
id: make-palette-colors-distinguishable-for-color-vision-deficiency
title: Make palette colors distinguishable for color vision deficiency
bibliography: references.bib
description: For charts where color differentiates values or categories, use lightness
  differences in the palette and check color distinguishability to improve accessibility
  and mitigate color confusion for readers with color vision deficiency.
labels:
- purpose:refine
- basis:heuristic
- quality:accessibility
- lever:encoding
- needs:color-vision-deficiency
- channel:color-lightness:use
---

## Colorblind-distinguishable palette <!-- role: advice -->

Separate palette colors with lightness differences so readers with color vision deficiency can still tell them apart. For example, check a gradient or category palette with a color-blindness simulator or an automatic color-blind check and revise it until the colors remain distinguishable.

## Why lightness helps beyond hue <!-- role: reason -->

Readers with color vision deficiency may not separate hues that look different to other readers. Lightness gives them another cue.

**Mechanism:** When palette colors differ in lightness as well as hue, more readers can distinguish the encoded groups or values.

**Evidence:** The post says that using different lightnesses in gradients and palettes helps readers with color vision deficiency distinguish colors, and recommends using an online tool or an automatic colorblind check to verify the palette [@muth_colors_2018].

## When to check for color vision deficiency <!-- role: context -->

- **User Goal:** Distinguish categories or value ranges by color.
- **Data:** Color is carrying important differences.
- **Chart Setting:** The chart uses a palette or gradient that readers must decode.
- **Audience:** Readers may include people with color vision deficiency.
- **Success Criterion:** Important color distinctions remain visible under color-blind simulation.

## When this check is unnecessary <!-- role: exceptions -->

**Break it when:** The colors are decorative and do not need to be distinguished to read the chart. **Why:** The rule applies when color itself encodes values or categories.

## Tradeoffs of colorblind-safe palettes <!-- role: costs -->

**Sacrifice:** Some palette options become unusable.
**Risk:** Chasing hue variety without lightness variety can still fail for color-blind readers.
**Mitigation:** Prioritize distinguishable lightness steps before fine-tuning hue.

## Common accessibility mistake <!-- role: mistakes -->

**Mistake:** Choosing palette colors that differ mainly by hue and not by lightness. **Why it fails:** Readers with color vision deficiency may not be able to separate the colors.

## How to check colorblind distinguishability <!-- role: check -->

**Failure Sign:** Two or more encoded colors collapse into near-sameness under simulation.
**Quick Check:** Run the palette through a color-blindness simulator or automatic color-blind check.
**Stronger Test:** Confirm that each important category or value range remains distinguishable after the check.

## How to fix colorblind palette failures <!-- role: fix -->

- Increase lightness differences between the encoded colors.
- Replace colors that become indistinguishable under simulation.
- Recheck the revised palette until the important distinctions remain visible.
