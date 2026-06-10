---
id: reorder-discrete-palettes-by-perceptual-distance
title: Reorder discrete palettes by perceptual distance before assigning categories
bibliography: references.bib
description: For categorical encoding assignment, use perceptual-distance-based palette
  order on discrete color, shape, or size palettes to maximize discriminability and
  mitigate early assignment of look-alike symbols for viewers comparing categories.
labels:
- purpose:refine
- basis:empirical
- data:categorical
- quality:fidelity
- lever:encoding
- polish:palette
---

## Reorder the palette for discriminability <!-- role: advice -->

Reorder the discrete palette so the earliest assigned items are the most perceptually distinct from one another. For example, start with the two palette items that are farthest apart perceptually, then keep adding the item whose minimum distance to the already chosen set is largest, so the first few colors or shapes come from different perceptual clusters.

## Why perceptual palette order works <!-- role: reason -->

Discrete palette items are not evenly separated in perception, even when they were manually designed to be distinct. Reordering by perceptual distance spreads the earliest assignments across the available perceptual space instead of leaving similar items adjacent in the assignment order.

**Mechanism:** Early category assignments become easier to tell apart because the palette order is driven by judged perceptual distance rather than by the original palette sequence.

**Evidence:** The paper uses learned perceptual kernels to reorder shape, color, and size palettes so that more perceptually discriminable stimuli are used first, and notes that the first items in the reordered shape palette come from different perceptual clusters [@demiralpLearningPerceptualKernels2014].

**Notes:** The reported construction is stable over time because adding new categories appends new items without replacing already assigned ones.

## Use when palette order controls category assignment <!-- role: context -->

- **User Goal:** Maximize how easily viewers distinguish category encodings.
- **Task:** Assign palette items sequentially to categories.
- **Data:** Categorical values mapped to a finite discrete palette.
- **Chart Setting:** Any chart that uses a fixed set of shapes or colors for category encoding.
- **Audience:** Viewers who need to tell encoded categories apart.
- **Success Criterion:** The first assigned categories are visually well separated.

## Do not use when encoding order must preserve magnitude <!-- role: exceptions -->

**Break it when:** The encoding is being used to show quantitative magnitude rather than category identity. **Why:** The paper notes that size palettes are better suited to quantitative use, so reordering them for categorical discriminability can conflict with magnitude order.

## Tradeoffs of perceptual palette reordering <!-- role: costs -->

**Sacrifice:** You give up the original palette order.
**Risk:** A stable greedy order may not be the globally best order for every possible subset size.
**Mitigation:** Keep the stable order when categories are added over time so existing assignments do not need to change.

## Common palette-order failure <!-- role: mistakes -->

**Mistake:** Assign categories in the default palette order without checking perceptual spacing. **Why it fails:** The first assigned items can come from the same perceptual cluster, so categories that should be easy to distinguish end up looking too similar.

## Check palette order before release <!-- role: check -->

**Failure Sign:** The first few assigned colors or shapes look more similar to each other than later ones.
**Quick Check:** Compare the pairwise perceptual distances among the first n assigned items against a reordered version built from the kernel.
**Stronger Test:** Inspect the kernel or an MDS projection and verify that the first few assigned items span different perceptual clusters instead of one cluster.

## Fix the palette order <!-- role: fix -->

- Compute or obtain a perceptual kernel for the palette you plan to use.
- Initialize the order with the pair of items that has the largest perceptual distance.
- Add each next item by maximizing its minimum perceptual distance to the already chosen set.
- Keep existing assignments fixed and append new items when new categories appear.
