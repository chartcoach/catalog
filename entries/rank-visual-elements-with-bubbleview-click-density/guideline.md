---
id: rank-visual-elements-with-bubbleview-click-density
title: Rank visual elements with BubbleView click density
bibliography: references.bib
description: For element-level evaluation of static visual designs, use BubbleView
  click density on annotated elements to improve insight and mitigate reliance on
  full eye-tracking studies in importance-ranking workflows.
labels:
- purpose:refine
- basis:empirical
- quality:insight
- lever:interaction-access
---

## Element scoring from click maps <!-- role: advice -->

Score annotated visual elements with BubbleView click density when you need an importance ranking across titles, labels, legends, or other design parts. For example, overlay the click map with element boxes or segmentations and assign each element the maximum click-map value inside its boundary before ranking the elements.

## Why element-level aggregation makes the map actionable <!-- role: reason -->

Raw click maps show where attention concentrates, but design decisions often depend on comparing named elements. Aggregating the map to element boundaries turns the spatial signal into a ranking that can guide revision.

**Mechanism:** Element-level scoring converts local click density into a comparable value per design component. That makes it easier to compare which parts of the visual drew the most deliberate attention.

**Evidence:** The paper shows that BubbleView click maps can rank labeled visualization elements similarly to eye fixations and can reasonably approximate explicit importance rankings on graphic design elements when element boundaries are overlaid on the map and scored [@kimBubbleViewInterfaceCrowdsourcing2017].

## Use when you have explicit element boundaries <!-- role: context -->

- **User Goal:** Compare which components of a visualization or graphic design are most important.
- **Task:** Evaluate element importance without running a full eye-tracking study.
- **Data:** Static visuals with annotated element boxes or segmentations.
- **Chart Setting:** BubbleView click map plus element annotations available for overlap.
- **Success Criterion:** The resulting ranking distinguishes which elements attracted the strongest deliberate attention.

## Do not use when blur changes element visibility too much <!-- role: exceptions -->

**Break it when:** Elements differ so much in scale or appearance that blur makes some disappear or leaves others visible without clicking. **Why:** The click map then reflects the blur artifact as much as the element's true importance.

## Tradeoffs of element scoring <!-- role: costs -->

**Sacrifice:** You need element annotations before you can compute the ranking.
**Risk:** A single highly clicked spot can dominate the score for a large element.
**Mitigation:** Inspect the overlaid map and element boxes to confirm that the maximum-value readout matches the design question you care about.

## Common failure mode with importance ranking <!-- role: mistakes -->

**Mistake:** Reading the raw click map without converting it into element-level scores. **Why it fails:** The map shows hotspots, but it does not directly tell you how whole design components rank against each other.

## How to check whether the ranking is usable <!-- role: check -->

**Failure Sign:** The click map is interpretable by eye, but you still cannot say whether one labeled element outranks another.
**Quick Check:** Overlay the click map with the annotated element boundaries and verify that every target element receives a score.
**Stronger Test:** Compare the ranked list from the scored elements with a second importance source, such as another participant batch or an explicit annotation set.

## What to change if it is not working <!-- role: fix -->

- Add bounding boxes or segmentations for the elements you want to compare.
- Compute one score per element from the click map instead of reading hotspots informally.
- Revisit the blur setting if critical elements disappear or stay visible without clicking.
- Narrow the element set to the specific design components you actually need to rank.
