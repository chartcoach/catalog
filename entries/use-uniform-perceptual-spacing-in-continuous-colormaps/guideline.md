---
id: use-uniform-perceptual-spacing-in-continuous-colormaps
title: Use uniform perceptual spacing in continuous colormaps
bibliography: references.bib
description: For equal-interval value reading, prefer uniform perceptual spacing on
  continuous color scales to improve fidelity and mitigate uneven emphasis for viewers
  comparing equal steps across the scale.
labels:
- purpose:refine
- basis:empirical
- quality:fidelity:use
- lever:encoding
- polish:palette
---

## Perceptual spacing <!-- role: advice -->

Use a continuous colormap whose equal data intervals produce equal-looking color steps. For example, redistribute palette stops so equal-value intervals change by similar visible amounts instead of compressing one region and stretching another.

## Why uniform spacing works <!-- role: reason -->

Uneven color spacing makes equal numeric differences look unequal. Some parts of the scale then appear over-emphasized while others lose visible separation.

**Mechanism:** Constant perceptual speed keeps equal data steps visually comparable, so readers do not overread fast regions or underread slow regions of the same scale.

**Evidence:** The collated review includes this paper as theoretical guidance for color-hue and color-saturation encoding, and the paper defines local and global uniformity as constant perceptual speed and evaluates departures from that rule through speed variation [@zengReviewCollationGraphical2023; @bujackGoodBadUgly2018].

## Use when equal steps should look equal <!-- role: context -->

- **User Goal:** Compare equal-sized changes across an ordered color scale.
- **Task:** Read differences or intervals from multiple parts of the same palette.
- **Data:** Ordered values encoded on a continuous scale.
- **Chart Setting:** Static color legend or continuous color encoding where several parts of the scale must carry similar visual weight.
- **Audience:** Viewers interpreting magnitude from the relative size of visible color changes.
- **Success Criterion:** Equal numeric intervals look equally different across the full scale.

## Do not use when another palette property matters more <!-- role: exceptions -->

**Break it when:** The main priority is a different palette property, such as maximizing discriminative power rather than keeping equal steps visually equal. **Why:** The paper treats colormap rules as beneficial qualities that can trade off against each other.

## Tradeoffs of uniform spacing <!-- role: costs -->

**Sacrifice:** You may reduce emphasis in visually dramatic regions of the palette.
**Risk:** Uniformizing the scale can lower separation where you previously had very large color jumps.
**Mitigation:** Check both uniformity and minimum step size so equal spacing does not collapse local discrimination.

## Common failure with unequal spacing <!-- role: mistakes -->

**Mistake:** Keeping equal numeric breaks while allowing one section of the palette to change much faster than another. **Why it fails:** Readers perceive some equal intervals as larger or smaller than others.

## Check spacing consistency <!-- role: check -->

**Failure Sign:** Equal-value intervals produce visibly different jump sizes across the scale.
**Quick Check:** Sample equal numeric intervals and compare whether the color jumps look similar.
**Stronger Test:** Compute the standard deviation of local or global speed and reduce it toward zero.

## Fix uneven palette spacing <!-- role: fix -->

- Move palette stops so equal-value intervals have similar perceptual distances.
- Remove compressed plateaus and overly steep jumps in the scale.
- Replace the scale with one whose local speed varies less across the full range.
