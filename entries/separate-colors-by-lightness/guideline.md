---
id: separate-colors-by-lightness
title: Separate encoded colors by lightness
bibliography: references.bib
description: For color-coded charts and maps, prefer distinct color lightness on categorical
  marks to improve distinguishability and mitigate same-brightness color confusion
  for readers with color-vision deficiency.
labels:
- purpose:refine
- basis:heuristic
- quality:accessibility
- lever:encoding
- channel:color-lightness:use
- needs:color-vision-deficiency
- access:contrast:use
- polish:palette
---

## Vary lightness, not just hue <!-- role: advice -->

Make category colors differ in lightness so the chart still works in black and white. For example, darken one category and lighten another, use yellow as a very light contrasting color, and avoid red text or marks that stay low-contrast after hue differences disappear.

## Why lightness matters <!-- role: reason -->

When hue collapses under color-vision deficiency, lightness often remains. A chart that is still readable in grayscale preserves the distinctions that color alone would otherwise lose.

**Mechanism:** Lightness creates a second path for separating marks, so readers can distinguish categories even when the hue contrast weakens.

**Evidence:** The article recommends getting charts right in black and white, states that any colors can work if they vary by lightness, highlights yellow as especially useful because it is so light, and shows that some red text becomes barely visible for colorblind readers. [@muth_colorblindness_2020]

## Use when colors are hard to tell apart <!-- role: context -->

- **User Goal:** Keep color-coded categories distinguishable.
- **Task:** Fast comparison or scanning of colored marks.
- **Data:** Categories or statuses encoded by color.
- **Chart Setting:** Any chart, map, or table where colors might otherwise share similar brightness.
- **Audience:** Readers who may include people with color-vision deficiency.
- **Success Criterion:** The categories remain distinguishable in grayscale or colorblind simulation.

## When lightness alone is not enough <!-- role: exceptions -->

**Break it when:** Brand colors or fixed colors cannot be changed enough to create real lightness separation. **Why:** The article recommends adding a second visual variable such as symbols, shapes, patterns, or line styles when color alone cannot be made readable.

## Costs of using lightness contrast <!-- role: costs -->

**Sacrifice:** You may give up exact brand-color treatment.
**Risk:** Conventional red/green semantics do not survive as intended, because colorblind readers may perceive those colors mostly as darker and lighter olives or oranges.
**Mitigation:** If fixed hues must stay, add a second noncolor encoding.

## Common lightness failure <!-- role: mistakes -->

**Mistake:** Keeping category colors at similar brightness and expecting hue alone to separate them. **Why it fails:** The article shows that same-lightness hues can merge for colorblind readers even when they look distinct to others.

## How to verify lightness separation <!-- role: check -->

**Failure Sign:** The categories become hard to distinguish when the chart is viewed in grayscale.
**Quick Check:** Print or convert the chart to black and white and check whether the colored groups still separate.
**Stronger Test:** Run a colorblind simulation and inspect whether the same categories remain distinct there too.

## What to change <!-- role: fix -->

- Lighten one category color and darken another until they separate in grayscale.
- Use yellow as the light member of a palette when you need a strong brightness contrast.
- Replace low-contrast colored text with a darker or lighter alternative that stays visible without hue.
- If lightness cannot be separated enough, add a second encoding such as symbols, patterns, or line style.
