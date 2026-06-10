---
id: use-gray-for-less-important-elements-and-reserve-accent-colors-for-highlights
title: Use gray for less important elements and reserve accent colors for highlights
bibliography: references.bib
description: For charts with highlights or context data, use gray on less important
  elements to improve visual hierarchy and mitigate competition with highlight colors
  for readers.
labels:
- purpose:refine
- basis:heuristic
- quality:readability
- lever:encoding
- polish:hierarchy
- aesthetic:color:use
---

## Visual hierarchy with gray <!-- role: advice -->

Color less important marks in gray and save stronger colors for the data you want readers to notice first. For example, use gray for context data, less important annotations, or unselected marks, and keep accent colors for the key data points.

## Why gray strengthens emphasis <!-- role: reason -->

If everything is colorful, nothing stands out. Gray pushes supporting material into the background without removing it.

**Mechanism:** Muting secondary elements increases the contrast between context and highlights, so the intended focal data gets noticed faster.

**Evidence:** The post says gray is often the most important color in data visualization because it makes highlight colors stick out more, and recommends gray for context data, less important annotations, and unselected states [@muth_colors_2018].

## When to use gray as support color <!-- role: context -->

- **User Goal:** Direct attention to a few important data points.
- **Chart Setting:** The chart includes highlights plus supporting context.
- **Data:** Some marks are intentionally more important than others.
- **Success Criterion:** The intended highlights stand out immediately.

## When plain gray should be softened <!-- role: exceptions -->

**Break it when:** A plain gray makes the chart feel too cold. **Why:** The post suggests using a warm gray or another very light color as an alternative.

## Tradeoffs of using gray for context <!-- role: costs -->

**Sacrifice:** The chart may look less colorful overall.
**Risk:** Overusing gray can make secondary information feel too weak.
**Mitigation:** Keep only the most important elements in accent colors, then tune the gray warmer if needed.

## Common hierarchy mistake <!-- role: mistakes -->

**Mistake:** Using strong colors on context marks and highlights at the same time. **Why it fails:** Secondary elements compete with the marks meant to stand out.

## How to check color hierarchy <!-- role: check -->

**Failure Sign:** Many non-key elements are colored as strongly as the highlights.
**Quick Check:** Scan the chart and see whether the intended highlight is visually obvious before you read labels.
**Stronger Test:** Compare the chart before and after graying secondary elements to see whether the highlight becomes clearer.

## How to fix weak hierarchy <!-- role: fix -->

- Recolor context data in gray.
- Recolor less important annotations in gray.
- Reserve accent colors for the few data points you want readers to notice first.
- Shift gray slightly warm or use a very light color if plain gray feels too cold.
