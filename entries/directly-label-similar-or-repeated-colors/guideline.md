---
id: directly-label-similar-or-repeated-colors
title: Directly label categories when colors are similar or repeated
bibliography: references.bib
description: For dense multi-category charts, use direct labels on same-colored or
  similarly colored marks to improve readability and mitigate reliance on a separate
  color key for readers scanning the chart.
labels:
- purpose:refine
- basis:heuristic
- lever:text-annotation
- component:label:use
- component:legend:avoid
- group-cardinality:many
- quality:readability:use
- polish:annotation
---

## Put labels on the marks <!-- role: advice -->

Directly label the marks when colors are the same or very similar. For example, place labels at the ends of same-colored lines or next to emphasized and background categories instead of expecting readers to decode a color key.

## Remove the legend detour <!-- role: reason -->

When many categories share similar colors, readers cannot identify them quickly from hue alone. Direct labels keep identity attached to the mark and avoid the back-and-forth search between chart and legend.

**Mechanism:** On-mark labels let readers recognize a category where they are already looking, which is especially helpful when color differences are weak or repeated.

**Evidence:** The post states that direct labels allow categories to share similar or even identical colors while remaining distinguishable, and it explicitly says a color key would not work in such cases whereas direct labeling does [@muth_fewer_colors_2022].

## Use when category identity must stay visible on the chart <!-- role: context -->

- **User Goal:** Reduce the number of colors without losing category identity.
- **Task:** Let readers identify categories quickly while scanning the chart.
- **Data:** Many categories are shown.
- **Chart Setting:** Colors are repeated, very similar, or intentionally muted.
- **Audience:** Readers who should not have to search a legend repeatedly.
- **Success Criterion:** Readers can identify visible categories directly from the chart.

## Do not use when direct labels do not fit <!-- role: exceptions -->

**Break it when:** There is not enough space to place direct labels on the chart. **Why:** The labels will crowd the display instead of clarifying it.

## Accept some space use for labels <!-- role: costs -->

**Sacrifice:** Direct labels consume space on or around the chart.
**Risk:** Some categories may still remain unlabeled if space is tight.
**Mitigation:** Label the most important categories directly and move only the rest to tooltips.

## Avoid relying on a legend for similar colors <!-- role: mistakes -->

**Mistake:** Using a color key to explain many same-colored or similarly colored categories. **Why it fails:** Readers must constantly jump between the mark and the key to identify what they are seeing.

## Check whether the chart reads without the legend <!-- role: check -->

**Failure Sign:** You must look away from the mark to know what category it is.
**Quick Check:** Cover the legend and see whether the visible categories are still identifiable.
**Stronger Test:** Verify that the most important categories are labeled directly on the chart itself.

## Replace the key with on-mark labels <!-- role: fix -->

- Add direct labels to the important categories on the marks themselves.
- Add direct labels to background categories where space allows.
- Remove reliance on a separate color key for repeated or similar colors.
- If space is too tight, keep direct labels for the key categories and use tooltips for the rest.
