---
id: keep-size-shape-combinations-large-enough-to-distinguish-shapes
title: Keep size-shape combinations large enough to distinguish shapes
bibliography: references.bib
description: For multi-encoding marks, use a larger minimum mark size when size and
  shape are combined to improve readability and mitigate shape confusion in small
  marks for viewers reading encoded symbols.
labels:
- purpose:refine
- basis:empirical
- quality:readability:use
- lever:encoding
- channel:size
- channel:shape
- measure:multi
---

## Enforce a minimum size for shape-coded marks <!-- role: advice -->

Keep the smallest marks large enough when one variable is encoded by size and another by shape. For example, if circles, squares, and diamonds also vary in size, raise the minimum rendered size so the smallest shapes do not all collapse into the same-looking mark.

## Why small size destroys shape distinctions <!-- role: reason -->

Shape is only useful if the reader can still tell the shapes apart at every size. Once the smallest marks get too small, the combined encoding stops working because the size channel interferes with the shape channel.

**Mechanism:** Increasing the minimum mark size preserves the visible differences among shapes at the smallest size levels.

**Evidence:** The paper shows that size-shape composition makes the shapes of small objects begin to look the same and states that rendering should make sure the marks do not get too small [@mackinlayAutomatingDesignGraphical1986].

## Use when size and shape encode different variables on the same mark <!-- role: context -->

- **User Goal:** Read both the size-coded and shape-coded variables from one symbol.
- **Task:** Distinguish symbolic categories while also perceiving size differences.
- **Data:** Multiple variables are encoded in the same mark.
- **Chart Setting:** Shape and size are composed into a single plotted symbol.
- **Success Criterion:** The smallest marks still preserve visible shape differences.

## This only matters when the size-shape composition creates very small marks <!-- role: exceptions -->

**Break it when:** The chart does not combine size with shape, or every rendered mark remains large enough for its shape to stay clear. **Why:** Then the specific interference between size and shape does not occur.

## Tradeoffs of raising the minimum mark size <!-- role: costs -->

**Sacrifice:** Larger marks consume more space.
**Risk:** Oversized marks can crowd the display if applied blindly.
**Mitigation:** Increase only the minimum size needed to preserve shape discrimination.

## Common composed-mark failure <!-- role: mistakes -->

**Mistake:** Let the smallest size level shrink until different shapes look the same. **Why it fails:** The shape channel stops carrying reliable information.

## Inspect the smallest marks first <!-- role: check -->

**Failure Sign:** The smallest symbols no longer look like distinct shapes.
**Quick Check:** Compare the smallest instances of each shape side by side and ask whether they are still visually different.
**Stronger Test:** Verify that the category encoded by shape can be read correctly even at the smallest size level.

## Repair the composed marks <!-- role: fix -->

- Increase the minimum rendered mark size.
- Re-render the chart and inspect the smallest size level again for visible shape differences.
- Remove the size-shape combination from the same mark if the display cannot keep the smallest marks large enough.
