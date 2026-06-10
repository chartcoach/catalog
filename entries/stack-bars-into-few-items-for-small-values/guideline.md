---
id: stack-bars-into-few-items-for-small-values
title: Break short bars into a few stacked items
bibliography: references.bib
description: For exact recall of small quantities, use stacked discrete items on bar-like
  quantitative charts to improve memory fidelity and mitigate loss from relying on
  a single stretched length for viewers reading values up to about five.
labels:
- purpose:refine
- basis:empirical
- task:retrieve
- chart:bar
- quality:fidelity
- lever:encoding
- reading-mode:exact
---

## Segmented value marks <!-- role: advice -->

Break a short bar into a few countable items instead of showing the value as one stretched mark. For example, show values from about 1 to 5 as stacks of circles or pictographs, or divide a solid bar into a few visible segments rather than using one continuous bar.

## Why a few stacked items help <!-- role: reason -->

Small stacks give the reader two cues at once: overall height and countable pieces. That makes the value easier to encode than a single stretched extent when the numbers are small.

**Mechanism:** A few discrete items let viewers use both length and small-number estimation, which improves recall compared with reading only a continuous length.

**Evidence:** Stacked items produced lower recall error than stretched items in the small 1-5 range, and that advantage disappeared when the value ranges became larger [@harozISOTYPEVisualizationWorking2015].

## Use when values stay very small <!-- role: context -->

- **User Goal:** Remember exact category values after a brief view.
- **Task:** Brief-glance encoding and recall.
- **Data:** Quantitative values with maxima around 4 to 5.
- **Chart Setting:** A bar-like chart can be drawn either as one stretched mark or as a stack of discrete items.
- **Audience:** Viewers reading exact small values rather than scanning large ranges.
- **Success Criterion:** Lower recall error for the encoded values.

## Do not use long stacks for larger values <!-- role: exceptions -->

**Break it when:** The values require stacks larger than about five items. **Why:** The advantage of stacking disappeared once the stacks moved beyond the small-number range.

## Tradeoffs of segmenting bars <!-- role: costs -->

**Sacrifice:** You give up some compactness and simplicity.
**Risk:** Large stacks become dense and hard to discern in limited space.
**Mitigation:** Limit the segmented form to small values or coarse intervals.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Extending the same stacked-item design to large values. **Why it fails:** Once the stack grows beyond a few items, the memory benefit over a continuous bar disappears.

## How to test it <!-- role: check -->

**Failure Sign:** The tallest bars require many tiny items or look crowded.
**Quick Check:** Count the maximum visible items per bar; if it exceeds about five, do not expect the stacking advantage.
**Stronger Test:** Compare brief recall between the segmented and continuous versions at your actual value range.

## What to change <!-- role: fix -->

- Split short bars into a few discrete items.
- Add a few visible breaks to a solid bar if full pictographs are unnecessary.
- Switch back to a continuous bar when the values become too large for a short stack.
