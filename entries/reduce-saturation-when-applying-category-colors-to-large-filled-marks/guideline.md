---
id: reduce-saturation-when-applying-category-colors-to-large-filled-marks
title: Reduce saturation when applying category colors to large filled marks
bibliography: references.bib
description: For categorical color encoding on charts with large filled marks, prefer
  lower-saturation category colors on the filled areas to improve readability and
  mitigate palettes that become overpowering when reused from lines or points.
labels:
- purpose:refine
- basis:heuristic
- data:categorical
- quality:readability
- lever:encoding
- polish:palette
- channel:color-saturation:use
---

## Match saturation to mark size <!-- role: advice -->

Reduce color saturation when the same category colors move from thin marks to large fills. For example, a palette that works on lines or points may feel too intense on bars, areas, or other big filled regions, so soften the fills before reusing it.

## Why mark size changes the palette <!-- role: reason -->

A color that feels lively on a thin line can become overwhelming when it covers a large area. The mark type changes how strong the same saturation looks.

**Mechanism:** Large filled marks amplify the visual force of saturated colors, so lower saturation keeps the chart readable without abandoning category contrast.

**Evidence:** The article notes that some palettes are too saturated for big areas because they were designed for lines and points [@muth_good_color_palettes_2024].

## Use when colors fill large shapes <!-- role: context -->

- **User Goal:** Reuse or adapt an existing categorical palette.
- **Data:** Categorical groups.
- **Chart Setting:** Colors will fill bars, areas, regions, or other large shapes rather than thin lines or points.
- **Success Criterion:** The filled marks stay distinct without overpowering the chart.

## Do not use when the marks stay thin <!-- role: exceptions -->

**Break it when:** The palette is used on thin lines or points. **Why:** Stronger saturation can help those smaller marks stay visible and distinct.

## Tradeoffs of lowering saturation <!-- role: costs -->

**Sacrifice:** You give up some punchiness.
**Risk:** If you lower saturation too far, categories can become harder to tell apart.
**Mitigation:** Soften the fills incrementally and review them in the actual chart.

## Common saturation mistake <!-- role: mistakes -->

**Mistake:** Reuse a line or point palette unchanged as a fill palette. **Why it fails:** Colors that are comfortable on thin marks can become overpowering on large filled marks.

## Check saturation on filled marks <!-- role: check -->

**Failure Sign:** Large filled marks look uncomfortably vivid or dominate the page.
**Quick Check:** Judge the colors on the actual filled chart, not just as isolated swatches.
**Stronger Test:** Compare the palette on a thin-mark version and a filled-mark version before deciding to reuse it.

## Fix an over-saturated fill palette <!-- role: fix -->

- Lower the saturation of the fill colors.
- Preview the adjusted palette on the intended filled chart instead of on line samples alone.
- If the palette still feels too strong, start from colors chosen for filled areas rather than from line colors.
