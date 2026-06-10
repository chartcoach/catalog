---
id: limit-same-hue-category-palettes-to-a-few-shades
title: Limit same-hue category palettes to a few shades
bibliography: references.bib
description: For comparison of a few unordered categories, prefer a same-hue lightness
  palette on category encodings to improve accessibility and address overly colorful
  or grayscale-ambiguous palettes for readers with color-vision differences.
labels:
- purpose:refine
- basis:heuristic
- quality:accessibility
- lever:encoding
- channel:color-lightness:use
- group-cardinality:few
- needs:color-vision-deficiency
- polish:palette
---

## Few-shade category palettes <!-- role: advice -->

Use only a few shades of one hue when category colors need to be less colorful or easier to separate in grayscale. For example, use two or three shades of blue for a small category set when you want a restrained chart and more reliable black-and-white differentiation.

## Why a few same-hue shades work <!-- role: reason -->

A single hue makes brightness differences easier to judge, which helps the chart survive in black and white. But the same strategy stops working when too many unordered categories must be distinguished.

**Mechanism:** Readers can more easily separate lightness steps within one hue than judge the relative lightness of different hues, especially when the display is viewed in grayscale.

**Evidence:** The article recommends shades of one hue as a way to make a chart less colorful and easier for colorblind readers, while warning that readers give up when four, five, or six unordered categories are encoded with different shades [@muth_quantitative_vs_qualitative_2021].

## Use when the category count is small <!-- role: context -->

- **User Goal:** Reduce colorfulness and keep category colors distinguishable in black and white.
- **Task:** Show a small set of categories.
- **Data:** Categories are unordered.
- **Chart Setting:** Color is being used for category identity, not magnitude.
- **Audience:** Some readers may have color-vision limitations.
- **Success Criterion:** The few categories remain distinguishable without relying on hue contrast alone.

## Do not use when the category count grows <!-- role: exceptions -->

**Break it when:** You need four or more unordered categories or maximum category separation. **Why:** Same-hue shades become hard to tell apart and readers stop distinguishing them reliably.

## What this choice costs <!-- role: costs -->

**Sacrifice:** You lose some category distinctness.
**Risk:** Readers may invent a reason for the darker shade, such as higher value or greater importance.
**Mitigation:** Do not assign shades randomly; if one binary category is more important, make that category darker, otherwise switch to separate hues.

## Common palette failure <!-- role: mistakes -->

**Mistake:** Use many shades of one hue for unordered categories. **Why it fails:** Readers cannot reliably separate four, five, or six same-hue categories.

## How to test the shade count <!-- role: check -->

**Failure Sign:** Several categories collapse together or look the same in black and white.
**Quick Check:** Convert the palette to grayscale and see whether the few categories still separate.
**Stronger Test:** Count the shades; if the palette needs four or more unordered categories, expect the same-hue approach to fail.

## How to revise it <!-- role: fix -->

- Reduce the palette to two or three shades.
- Keep the palette inside one hue family.
- If you need more categories, switch the encoding to distinct hues.
- Put the darker shade on the more important category when a binary contrast needs emphasis.
