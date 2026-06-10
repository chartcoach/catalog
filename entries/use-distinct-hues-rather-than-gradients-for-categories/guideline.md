---
id: use-distinct-hues-rather-than-gradients-for-categories
title: Use distinct hues rather than gradients for categories
bibliography: references.bib
description: For category-coded charts, use distinct hues on the categorical encoding
  to improve fidelity and mitigate unintended ranking of categories for readers.
labels:
- purpose:refine
- basis:heuristic
- data:categorical
- quality:fidelity
- lever:encoding
- channel:color-hue:use
- aesthetic:color:use
---

## Categorical color choice <!-- role: advice -->

Assign categorical groups distinct hues instead of light-to-dark shades of one hue. For example, replace several blues used for different categories with clearly different category colors so the palette does not imply a low-to-high ranking.

## Why gradients mislead in categorical charts <!-- role: reason -->

A same-hue gradient suggests order even when no order exists. That false ranking changes how readers interpret the categories.

**Mechanism:** Distinct hues signal separate identities, while light-to-dark shades of one hue suggest less-to-more or low-to-high structure.

**Evidence:** The post warns against using gradient palettes for categories because readers associate dark colors with more and bright colors with less, which implies a ranking of the categories, and recommends using different hues instead [@muth_colors_2018].

## When to use distinct hues <!-- role: context -->

- **User Goal:** Distinguish unordered categories.
- **Data:** Groups are categorical rather than ordered values.
- **Chart Setting:** Color is the main encoding for category identity.
- **Success Criterion:** Readers treat the groups as separate categories, not as ranked levels.

## When a gradient is appropriate instead <!-- role: exceptions -->

**Break it when:** The colors are meant to encode low-to-high magnitude. **Why:** In that case, a gradient is the intended signal rather than a misleading one.

## Tradeoffs of distinct hues <!-- role: costs -->

**Sacrifice:** The chart may look more colorful.
**Risk:** One category can seem emphasized if its color is much darker or more saturated without explanation.
**Mitigation:** If a category color stands out, make sure the chart explains why.

## Common categorical-color mistake <!-- role: mistakes -->

**Mistake:** Using a same-hue light-to-dark palette for different categories. **Why it fails:** Readers infer an order that the data does not have.

## How to check categorical color use <!-- role: check -->

**Failure Sign:** One category looks like “more” only because its color is darker.
**Quick Check:** Look for several category colors that are just lighter and darker versions of one hue.
**Stronger Test:** Ask whether the palette would make sense if the category names were removed; if it still reads like a ranking, the palette is misleading.

## How to fix misleading category gradients <!-- role: fix -->

- Replace same-hue shades with distinct hues for the categories.
- Remove unnecessary light-to-dark ordering from the category palette.
- Explain any intentional standout category color in the chart.
- Change the chart form if a distinct-hue palette makes the chart too colorful.
