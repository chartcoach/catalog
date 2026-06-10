---
id: differentiate-similar-lines-with-line-style
title: Differentiate similarly bright lines with dashes or line width
bibliography: references.bib
description: For line charts with similarly bright series colors, prefer line-style
  variation on series marks to improve distinguishability and mitigate overlap confusion
  for readers with color-vision deficiency.
labels:
- purpose:refine
- basis:heuristic
- chart:line
- quality:accessibility
- lever:encoding
- channel:line-style:use
- needs:color-vision-deficiency
---

## Add a second line encoding <!-- role: advice -->

Use dashes or unequal line widths when two line colors are similarly bright. For example, dot one of two overlapping series or make one line thicker and the other thinner so the reader can separate them where they cross or run together.

## Why line style helps <!-- role: reason -->

Overlapping lines are hard to decode when color differences are subtle. Line style adds a second series identity that remains visible at crossings and during quick scanning.

**Mechanism:** Dashes and width changes make each series visually distinct even when the color contrast is weak.

**Evidence:** The article recommends different line widths and dashes when similarly bright colors must be used in a line chart and shows a confusing overlap that becomes easier to read after one line is dotted. [@muth_colorblindness_2020]

## Use when line colors are close in brightness <!-- role: context -->

- **User Goal:** Keep two or more line series distinct during comparison.
- **Task:** Follow and compare series through overlaps.
- **Data:** Multiple time-based or ordered series in one line chart.
- **Chart Setting:** A line chart where the palette cannot avoid similarly bright colors.
- **Audience:** Readers who may include people with color-vision deficiency.
- **Success Criterion:** The series remain distinguishable where they overlap.

## When a style change is unnecessary <!-- role: exceptions -->

**Break it when:** The line colors can be changed so they are already clearly distinct by hue or lightness. **Why:** The article introduces dashes and width changes specifically for cases where similarly bright colors must remain.

## Costs of line-style encoding <!-- role: costs -->

**Sacrifice:** You give up some visual uniformity across the series.
**Risk:** Adding too many style differences can make the chart feel busy.
**Mitigation:** Change only the line or lines that are hard to distinguish.

## Common line-chart failure <!-- role: mistakes -->

**Mistake:** Leaving similarly bright overlapping series as solid lines with the same width. **Why it fails:** Readers cannot tell which line is which where the series meet or cross.

## How to verify line differentiation <!-- role: check -->

**Failure Sign:** In overlap areas, the two series are easy to confuse.
**Quick Check:** Inspect the densest crossing or overlap area and see whether the series still separate without color alone.
**Stronger Test:** Run a colorblind simulation and check whether the line style still identifies each series.

## What to change <!-- role: fix -->

- Dot one of the confusing lines.
- Make one line thicker and the other thinner.
- Apply the style change to the overlapping series rather than to every line in the chart.
