---
id: space-gridlines-at-least-8-pixels-apart
title: Keep gridlines at least 8 pixels apart
bibliography: references.bib
description: For exact value comparison in static displays, use gridline spacing of
  at least 8 pixels on bar and line charts to improve fidelity and mitigate tracing
  errors from overly dense reference lines for web viewers.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:bar
- chart:line
- quality:fidelity
- lever:layout-structure
- component:axis:use
---

## Gridline spacing <!-- role: advice -->

Space gridlines only as densely as the chart height can support. For example, keep neighboring gridlines at least 8 pixels apart in bar and line charts, instead of packing 10-unit gridlines into a 40-pixel chart.

## Why moderate spacing works <!-- role: reason -->

Gridlines help readers read values, but only until the lines become so dense that they interfere with tracing marks to the scale. Dense reference lines stop acting like guides and start acting like clutter.

**Mechanism:** Moderate gridlines provide landmarks for value reading, while overly dense gridlines make it harder to visually trace a mark to its label.

**Evidence:** Adding gridlines improved accuracy in the chart-size experiment, but there was no meaningful accuracy gain from the densest settings over the next coarser settings. Error rose sharply when a 40-pixel chart used 10-unit gridline spacing, leading the paper to recommend separating gridlines by at least 8 pixels. [@heerCrowdsourcingGraphicalPerception2010]

## Use when gridlines support exact reading <!-- role: context -->

- **User Goal:** Read and compare values accurately.
- **Task:** Exact or near-exact difference reading.
- **Data:** Quantitative values shown on a 0-100 scale.
- **Chart Setting:** Static bar or line chart with visible gridlines in a web display.
- **Audience:** Web viewers using standard displays.
- **Success Criterion:** Lower comparison error without intrusive reference lines.

## Do not overpack short charts <!-- role: exceptions -->

**Break it when:** The available chart height would force gridlines closer than about 8 pixels, or the chart is outside the tested bar/line 0-100 setting. **Why:** The paper found dense gridlines harmful in short charts and only tested this recommendation on those charts and scales.

## Costs of wider gridline spacing <!-- role: costs -->

**Sacrifice:** You may show fewer reference lines.
**Risk:** Removing too many gridlines can also reduce value-reading support.
**Mitigation:** Use gridlines, but stop increasing density once spacing drops below about 8 pixels.

## Common spacing mistake <!-- role: mistakes -->

**Mistake:** Adding more gridlines whenever exact reading matters, without checking the pixel gap between them. **Why it fails:** The chart becomes harder to trace when the reference lines are packed too tightly.

## How to check gridline spacing <!-- role: check -->

**Failure Sign:** Gridlines visually crowd the plot and readers struggle to trace marks to labels.
**Quick Check:** Measure the pixel gap between adjacent gridlines; if it is under about 8 pixels, the spacing is too dense.
**Stronger Test:** Compare reader errors on the current gridline density against a version with fewer lines or more chart height.

## How to fix gridline spacing <!-- role: fix -->

- Reduce the number of gridlines until adjacent lines are at least about 8 pixels apart.
- Increase chart height if you need the same numeric interval but more pixel space.
- Keep gridlines as reading aids, but avoid the densest setting that turns them into visual interference.
