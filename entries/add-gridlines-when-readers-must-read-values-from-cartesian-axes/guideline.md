---
id: add-gridlines-when-readers-must-read-values-from-cartesian-axes
title: Add gridlines when readers must read values from Cartesian axes
bibliography: references.bib
description: For value lookup, use axis grids on charts with Cartesian position scales
  to improve readability and mitigate axis-alignment mistakes for novice readers.
labels:
- purpose:refine
- basis:empirical
- task:retrieve
- lever:encoding
- component:axis:use
- channel:position
- quality:readability
- literacy:novice
---

## Add axis grids for value reading <!-- role: advice -->

Add gridlines when readers must read values against Cartesian axes. For example, include grids in line charts, bar charts, scatterplots, area charts, and stacked area charts so readers can align marks to ticks more easily.

## Why gridlines help axis reading <!-- role: reason -->

Position-based charts often require the reader to map a mark back to a scale. Gridlines provide a reference scaffold for that alignment.

**Mechanism:** The grid gives the eye a visible path from the mark to the axis. This reduces guesswork when the task depends on reading a value from position.

**Evidence:** When building the VLAT, charts with Cartesian coordinate systems were given grids specifically to help readers read values on the axes [@leeVLATDevelopmentVisualization2017].

## Use when axis lookup is part of the task <!-- role: context -->

- **User Goal:** Read or compare values from a plotted position.
- **Task:** Value retrieval from a Cartesian scale.
- **Chart Setting:** A chart with x and y axes where marks must be aligned to ticks.
- **Audience:** Novice or non-expert readers.
- **Success Criterion:** Readers can map marks to axis values without guessing.

## Do not use when there is no Cartesian axis to read <!-- role: exceptions -->

**Break it when:** The chart does not use a Cartesian coordinate system. **Why:** Gridlines do not support axis lookup when there is no axis-position readout to align against.

## Tradeoffs of adding gridlines <!-- role: costs -->

**Sacrifice:** You add visible reference lines to the chart.\
**Risk:** Unneeded grids can add visual weight when exact axis reading is not part of the task.\
**Mitigation:** Use them where the reader must align marks to a scale, not as a default on every chart.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Omitting gridlines from a Cartesian chart that asks readers to read values from axes. **Why it fails:** The reader has fewer references for aligning the mark to the correct tick value.

## How to test the chart <!-- role: check -->

**Failure Sign:** Readers hesitate between adjacent tick values or approximate by eye without confidence.\
**Quick Check:** Ask a reviewer to read several values directly from the chart; if alignment to ticks feels uncertain, add grids.\
**Stronger Test:** Compare the same value-reading task with and without gridlines and keep the version that makes axis lookup more direct.

## What to change <!-- role: fix -->

- Add gridlines aligned to the axis ticks used for the reading task.
- Keep the grid only on charts with Cartesian axes where value lookup matters.
- Use the grid to support the specific axis readouts readers must make.
