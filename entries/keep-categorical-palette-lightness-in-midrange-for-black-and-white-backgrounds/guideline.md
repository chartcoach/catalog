---
id: keep-categorical-palette-lightness-in-midrange-for-black-and-white-backgrounds
title: Keep categorical palette lightness in a midrange when colors must work on black
  and white backgrounds
bibliography: references.bib
description: For categorical comparison on visualizations shown against black and
  white backgrounds, use midrange color lightness on categorical encodings to improve
  readability and address disappearing or washed-out colors for viewers distinguishing
  categories.
labels:
- purpose:refine
- basis:empirical
- data:categorical
- quality:readability
- lever:encoding
- channel:color-lightness:use
- polish:palette
- aesthetic:color:use
---

## Clamp palette lightness <!-- role: advice -->

Keep categorical palette colors in a midrange lightness when the same palette must remain visible on both black and white backgrounds. For example, exclude colors darker than L\*=25 and lighter than L\*=85 so every chosen color stays visible against black and white.

## Why the midrange helps <!-- role: reason -->

Very dark colors collapse into black backgrounds, and very light colors wash out on white backgrounds. A midrange lightness band preserves visibility at both extremes.

**Mechanism:** Removing lightness extremes keeps every palette color separable from the background instead of losing category marks to black or white.

**Evidence:** The palette construction in the paper explicitly removed colors below L\*=25 and above L\*=85 so all colors would remain visible on black and white backgrounds [@gramazioColorgoricalCreatingDiscriminable2017].

## Use when the palette must survive both background extremes <!-- role: context -->

- **User Goal:** Keep all categorical colors visible.
- **Task:** Distinguish categories on charts that may be shown on light or dark backgrounds.
- **Data:** Categorical groups encoded by color.
- **Chart Setting:** A palette intended to work on both black and white backgrounds.
- **Audience:** Viewers who need all categories to remain visible without background-dependent failures.
- **Success Criterion:** No palette color disappears against either background.

## Do not use when a different background requirement defines the target range <!-- role: exceptions -->

**Break it when:** The palette does not need to stay legible on both black and white backgrounds. **Why:** The lightness clamp was chosen specifically to preserve visibility against those two extreme backgrounds.

## Midrange visibility narrows the usable color space <!-- role: costs -->

**Sacrifice:** You lose the brightest and darkest candidate colors.
**Risk:** A smaller color space can limit extreme-looking palette options.
**Mitigation:** Adjust hue and chroma inside the surviving lightness band instead of reaching for lightness extremes.

## Common lightness failure <!-- role: mistakes -->

**Mistake:** Keeping very bright or very dark colors because they seem distinctive in isolation. **Why it fails:** They can disappear against white or black backgrounds even if they look strong as standalone swatches.

## Preview the palette on both extremes <!-- role: check -->

**Failure Sign:** One or more colors nearly vanish on a black or white background.
**Quick Check:** Render the full palette on black and on white and inspect whether any swatch loses visibility.
**Stronger Test:** Verify that every palette color falls within the L\*=25 to L\*=85 band.

## Pull extreme colors back into the band <!-- role: fix -->

- Lighten colors below L\*=25.
- Darken colors above L\*=85.
- Replace extreme colors with RGB-valid alternatives that stay inside the midrange lightness band.
