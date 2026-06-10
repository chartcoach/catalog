---
id: shift-palette-colors-toward-a-shared-hue-to-unify-them
title: Shift palette colors toward a shared hue to unify them
bibliography: references.bib
description: For revising an existing categorical palette, use a shared hue shift
  on palette colors to improve aesthetics and mitigate colors that feel unrelated
  in one chart.
labels:
- purpose:refine
- basis:heuristic
- data:categorical
- quality:aesthetics
- lever:encoding
- polish:consistency
- channel:color-hue:use
- aesthetic:color:use
---

## Apply a shared hue shift <!-- role: advice -->

Move the palette slightly toward one shared hue when the colors feel disconnected. For example, place a colored layer above the swatches in an image editor, set it to Hue blend mode, then adjust the layer color or opacity; a light Overlay can also work.

## Why a shared hue unifies the palette <!-- role: reason -->

Colors often feel more related when they share some hue character. A small shared hue shift can make a palette feel like one family instead of a loose collection.

**Mechanism:** A shared hue ties disparate colors together visually, but too much shifting also shrinks the hue contrast that keeps categories distinct.

**Evidence:** The article recommends unifying colors by blending them with a colored layer in Hue mode, suggests adjusting transparency and sometimes using Overlay, and warns that the hue contrast between colors will become smaller after the blend [@muth_good_color_palettes_2024].

## Use when a chosen palette feels disjointed <!-- role: context -->

- **User Goal:** Make an existing palette feel more cohesive.
- **Data:** Categorical groups.
- **Chart Setting:** The chosen colors feel unrelated when shown together in one chart.
- **Success Criterion:** The palette looks more unified while categories remain distinguishable.

## Do not use when hue contrast is already barely sufficient <!-- role: exceptions -->

**Break it when:** The hue shift makes categories too hard to tell apart. **Why:** The blend reduces hue contrast between the colors.

## Tradeoffs of hue blending <!-- role: costs -->

**Sacrifice:** You give up some hue contrast.
**Risk:** A strong blend can make once-distinct categories drift too close together.
**Mitigation:** Use a small opacity change and recheck the palette after every adjustment.

## Common blending mistake <!-- role: mistakes -->

**Mistake:** Apply a strong hue blend and assume the palette is better just because it looks more unified. **Why it fails:** The same edit can also erase useful differences between categories.

## Check cohesion without losing distinction <!-- role: check -->

**Failure Sign:** After blending, categories look closer together than before.
**Quick Check:** Compare the before and after palettes side by side in the actual chart.
**Stronger Test:** Run the adjusted colors through the same distinguishability check you use for the original palette.

## Fix an over-blended palette <!-- role: fix -->

- Reduce the blend opacity.
- Change the blend color to a less aggressive shared hue.
- Try a lighter Overlay or revert the blend if the categories no longer separate well.
