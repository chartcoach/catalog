---
id: vary-lightness-across-categorical-hues
title: Vary the lightness of categorical hues so categories still separate in grayscale
bibliography: references.bib
description: For categorical color palettes that must remain distinguishable in grayscale,
  use lightness differences across hues to improve accessibility and mitigate category
  collisions for readers with color-vision deficiencies.
labels:
- purpose:refine
- basis:heuristic
- data:categorical
- quality:accessibility
- lever:encoding
- channel:color-lightness:use
- needs:color-vision-deficiency
- access:contrast:use
---

## Separate categorical hues by lightness <!-- role: advice -->

Give categorical hues different lightness levels instead of relying on hue alone. For example, make one category noticeably lighter and another darker so the palette still works when viewed in greyscale.

## Why lightness variation helps <!-- role: reason -->

Lightness adds a second cue beyond hue. Categories stay separable when readers cannot rely on hue differences alone.

**Mechanism:** When categorical colors differ in both hue and lightness, readers can distinguish categories in grayscale and in color-deficient viewing conditions.

**Evidence:** The article says to give hues different lightnesses so they work in greyscale, look better, and become easier to distinguish, especially for colorblind readers [@muth_which_color_scale_2021].

## Use when category colors must remain distinct beyond hue <!-- role: context -->

- **User Goal:** Keep categories distinguishable under more than one viewing condition.
- **Task:** Tell categorical groups apart even when hue is weakened or unavailable.
- **Data:** The color scale is categorical rather than quantitative.
- **Chart Setting:** A hue palette is already being used to encode categories.
- **Audience:** Readers with color-vision deficiencies or readers seeing the chart in greyscale.
- **Success Criterion:** Each category remains visually distinct without relying on hue alone.

## Do not use this as a palette rule for quantitative gradients <!-- role: exceptions -->

**Break it when:** The color scale is a quantitative gradient rather than a set of categorical hues. **Why:** This rule is about separating categorical colors, not defining ordered value gradients.

## Tradeoffs of adding lightness variation <!-- role: costs -->

**Sacrifice:** Palette choices become more constrained because hue alone is not enough.
**Risk:** Colors with similar lightness collapse into the same gray tone.
**Mitigation:** Inspect the palette in greyscale and widen the lightness gaps where categories merge.

## Common palette mistake <!-- role: mistakes -->

**Mistake:** Choose category colors that differ mostly by hue while staying at nearly the same lightness. **Why it fails:** The categories become harder to distinguish, especially for colorblind readers.

## Check the palette without hue <!-- role: check -->

**Failure Sign:** Two or more category colors turn into nearly the same shade of gray.
**Quick Check:** View the palette in greyscale and see whether every category still separates.
**Stronger Test:** Compare categories by lightness alone; if two categories depend only on hue difference, revise the palette.

## Fix the palette <!-- role: fix -->

- Increase the lightness differences between category hues.
- Replace hues that only differ by hue with lighter or darker alternatives.
- Recheck the palette in greyscale until each category still separates.
