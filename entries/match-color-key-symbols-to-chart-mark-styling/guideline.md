---
id: match-color-key-symbols-to-chart-mark-styling
title: Match color-key symbols to the chart's mark styling
bibliography: references.bib
description: For lookup in categorical color keys, use symbol styling on legends that
  matches the chart marks to improve accessibility and mitigate color-only matching
  for readers locating colored marks.
labels:
- purpose:refine
- basis:heuristic
- data:categorical
- quality:accessibility
- lever:encoding
- component:legend:use
- access:noncolor:use
- reading-mode:lookup
---

## Mark-form symbols <!-- role: advice -->

Draw the same mark form and styling in the color key that the chart uses. For example, show thick or dashed line samples instead of plain color chips, include hatching or rectangles when the mapped regions use them, and add point outlines in the key when the plotted points have outlines.

## Matching symbols reduce color-only search <!-- role: reason -->

Readers look for the same visual form they see in the chart, not just for a hue. A color key that repeats line style, shape, texture, or outline gives them a second cue for matching.

**Mechanism:** Matching mark styling lets readers locate the corresponding marks faster and reduces dependence on color alone.

**Evidence:** The post recommends showing form, not just color, when the chart uses thick lines, thin lines, dashed lines, or rectangles, and separately recommends adding outlines to the key when the chart marks have outlines because the outline helps accessibility and makes color matching easier. [@muth_color_keys_2023]

## Use when the chart marks differ by more than fill <!-- role: context -->

- **User Goal:** Find the correct colored mark in the chart quickly.
- **Data:** Categories are encoded with color plus another visible form cue.
- **Chart Setting:** Marks differ by line style, hatching, shape, rectangle form, or outlines.
- **Audience:** Readers are matching legend items back to marks in the plot or map.
- **Success Criterion:** The key visually resembles the marks readers must find.

## Do not use when color is the only distinguishing cue <!-- role: exceptions -->

**Break it when:** The marks differ only by fill color and do not use special form or outline styling. **Why:** A simple color sample already represents the chart faithfully.

## Cost of richer legend symbols <!-- role: costs -->

**Sacrifice:** You give up the simplest possible row of generic color chips.\
**Risk:** Plain chips hide the actual distinguishing form and force color-only matching.\
**Mitigation:** Use small but faithful symbol samples that still fit the key.

## Common symbol mismatch failure <!-- role: mistakes -->

**Mistake:** Show plain color swatches when the chart marks use dashed lines, hatching, rectangles, or outlines. **Why it fails:** The key omits the very cue readers need to find the marks.

## Quick review for symbol fidelity <!-- role: check -->

**Failure Sign:** The legend symbol does not look like the corresponding chart mark.\
**Quick Check:** Compare one key item directly with one plotted mark and ask whether the same line style, texture, or outline appears in both.\
**Stronger Test:** Try locating a mark from the key without relying on color alone.

## Concrete edits for symbol mismatch <!-- role: fix -->

- Replace generic chips with symbol samples that match the chart marks.
- Draw line samples with the same thickness or dash pattern used in the chart.
- Include hatching, rectangles, or other region styling when those forms appear in the visualization.
- Add the same outlines to key symbols that the chart marks use.
