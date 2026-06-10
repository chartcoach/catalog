---
id: use-ordered-lightness-scales-for-ordered-values
title: Use an ordered lightness scale for values with inherent order
bibliography: references.bib
description: For comparison of ordered values, use a quantitative color scale on chart
  encodings to improve readability and address unordered hue assignments for readers
  scanning low-to-high meaning.
labels:
- purpose:refine
- basis:heuristic
- data:quantitative
- data:ordinal
- quality:readability
- lever:encoding
- channel:color-lightness:use
---

## Ordered lightness scales <!-- role: advice -->

Use a sequential or diverging lightness scale when the color-encoded values have an inherent order. For example, map rates to light-to-dark shades, and treat ordered text labels such as Likert responses or clothing sizes as ordered values rather than as separate hues.

## Why ordered lightness works <!-- role: reason -->

An ordered lightness scale tells readers that the colors represent progression. This works for numbers and for ordered labels, because the cue comes from the order in the data, not from whether the values are written as numerals or words.

**Mechanism:** Lightness variation gives readers a visible low-to-high structure that matches ranked or ordered data.

**Evidence:** The article recommends sequential or diverging color scales whenever the values can be ordered and explicitly extends that advice to ordered labels such as Likert responses and clothing sizes [@muth_quantitative_vs_qualitative_2021].

## Use when color should show rank <!-- role: context -->

- **User Goal:** Show low-to-high or one-side-versus-the-other ordering with color.
- **Task:** Compare ordered values.
- **Data:** Values are numeric or ordinal and can be ranked.
- **Chart Setting:** Color is encoding the value itself.
- **Success Criterion:** Readers can read a progression from the palette.

## Do not use when categories are unordered <!-- role: exceptions -->

**Break it when:** The color-encoded values are peer categories with no inherent order. **Why:** The ramp implies a rank that does not exist.

## What this choice costs <!-- role: costs -->

**Sacrifice:** Neighboring categories may be less distinct than with unrelated hues.
**Risk:** On bright backgrounds, a reversed ramp can feel unintuitive because dark often reads as high.
**Mitigation:** Map the higher end to darker shades on bright backgrounds unless you explicitly explain another direction.

## Common palette failure <!-- role: mistakes -->

**Mistake:** Assign unrelated hues to ordered values. **Why it fails:** Readers lose the low-to-high meaning in the colors.

## How to test the scale direction <!-- role: check -->

**Failure Sign:** The palette cannot be read as a progression without relying on text.
**Quick Check:** Ask whether a reviewer can sort the colors from low to high.
**Stronger Test:** On a bright background, verify that the darker end reads as the higher end unless the chart clearly states otherwise.

## How to revise it <!-- role: fix -->

- Replace unrelated hues with a sequential or diverging lightness ramp.
- Remap the high end to the darker shades on bright backgrounds.
- Put ordered text categories into the same ordered scale instead of treating them as separate hues.
