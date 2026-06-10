---
id: reorder-discrete-shape-or-color-palettes-by-perceptual-distance
title: Reorder discrete shape or color palettes by perceptual distance
bibliography: references.bib
description: For cluster-oriented reading of categorical groups, prefer perceptually
  reordered shape or color palettes on categorical mark encodings to maximize readability
  and mitigate confusable default palette orderings for viewers distinguishing groups.
labels:
- purpose:refine
- basis:empirical
- task:cluster
- data:categorical
- quality:readability:use
- lever:scale-order
- polish:palette
---

## Palette order <!-- role: advice -->

Reorder a discrete shape or color palette so the earliest assigned entries are maximally separated in perceptual distance. For example, start with the most dissimilar pair, then add each next color or shape that maximizes its minimum distance to the already used set, instead of assigning categories in the palette's default order.

## Why reordered palettes help <!-- role: reason -->

Perceptually reordered palettes spread early assignments across distinct perceptual clusters. That makes neighboring category assignments less confusable when viewers need to separate groups by shape or color alone.

**Mechanism:** Reordering by perceptual distance increases the minimum separation among the symbols or colors that appear first, so early category assignments are easier to tell apart.

**Evidence:** The paper estimates perceptual kernels for discrete shape and color values and then reorders those palettes to maximize perceptual discriminability, noting that sequential assignments from the reordered palettes should better promote discrimination. A later review collates this paper as evidence on nominal shape, color-hue, and area encodings for cluster-oriented visualization decisions [@zengReviewCollationGraphical2023; @demiralpLearningPerceptualKernels2014].

**Notes:** The paper includes a size palette for completeness, but notes that size is better suited to quantitative than categorical use.

## Use when categories must stay distinct <!-- role: context -->

- **User Goal:** Distinguish categorical groups or clusters quickly.
- **Task:** Separate groups by their assigned symbol or color.
- **Data:** Discrete categories with a fixed finite palette.
- **Chart Setting:** A chart already uses categorical color or shape encodings, and categories will be assigned sequentially from a palette.
- **Audience:** Viewers must tell groups apart from the marks themselves.
- **Success Criterion:** The first several assigned categories are perceptually easy to distinguish.

## Do not use when the channel must show order <!-- role: exceptions -->

**Break it when:** The encoding channel is being used to show ordered magnitude rather than nominal group membership. **Why:** The paper explicitly notes that size is better suited to quantitative use than categorical palette assignment.

## Costs of palette reordering <!-- role: costs -->

**Sacrifice:** You need a perceptual distance matrix or kernel before you can derive the order.
**Risk:** A poor similarity model can produce a misleading order.
**Mitigation:** Base the order on the perceptual kernel for the exact palette you plan to use.

## Common palette-order mistakes <!-- role: mistakes -->

**Mistake:** Keep the original off-the-shelf palette order and assign categories straight through it. **Why it fails:** Early assignments can come from the same perceptual cluster and reduce discrimination.

## Check palette separation <!-- role: check -->

**Failure Sign:** The first few assigned colors or shapes look noticeably similar or clustered.
**Quick Check:** Inspect the first four assigned entries and see whether they spread across distinct perceptual groups rather than repeating one visual family.
**Stronger Test:** Verify that each added entry maximizes its minimum perceptual distance to the entries already in use.

## Fix the palette order <!-- role: fix -->

- Start the ordered palette with the most perceptually distant pair.
- Add each next entry by choosing the item whose minimum distance to the used set is largest.
- Replace sequential use of the default palette order with the reordered sequence.
- Re-test the first several assignments, not just the full palette, because early entries do most of the work in categorical separation.
