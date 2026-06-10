---
id: move-small-slice-labels-outside-the-pie
title: Place small-slice labels outside the pie chart
bibliography: references.bib
description: For pie charts with small slices or long labels, use outside labels on
  the chart to improve readability and mitigate hard-to-label wedges for readers.
labels:
- purpose:refine
- basis:heuristic
- chart:pie-donut
- lever:text-annotation
- component:label:use
- quality:readability
- polish:annotation
---

## Move labels outside small wedges <!-- role: advice -->

Place labels for small slices outside the pie chart. For example, move labels outside when the slice is thin or when the label text is long.

## Why outside labels help pie charts <!-- role: reason -->

Pie charts leave limited room for text inside narrow wedges. Moving small-slice labels outside the circle gives the labels more room and reduces the strain of fitting text into the slices.

**Mechanism:** Outside labels free the slice from carrying both the wedge and the text, which makes small slices and long labels easier to read.

**Evidence:** The source says pie charts are hard to label and recommends labeling smaller pie slices outside the chart, especially when labels are long [@muth_pie_charts_2018].

## Use when slices are thin or labels are long <!-- role: context -->

- **User Goal:** Keep slice labels readable in a pie chart.
- **Data:** A pie chart with one or more small slices.
- **Chart Setting:** Labels are needed on the chart, and some labels are long or hard to fit.
- **Success Criterion:** Labels fit cleanly without being forced into thin wedges.

## Do not use when the labels fit cleanly inside the slices <!-- role: exceptions -->

**Break it when:** The slice labels are short and the wedges are large enough to hold them cleanly. **Why:** The extra outside placement is less necessary.

## Tradeoffs of outside labels <!-- role: costs -->

**Sacrifice:** You use more space around the pie chart.
**Risk:** Keeping labels inside small wedges leaves the pie hard to label.
**Mitigation:** Move only the smaller-slice labels outside.

## Common label placement mistake in pies <!-- role: mistakes -->

**Mistake:** Keeping long labels inside thin slices. **Why it fails:** Pie charts are hard to label that way.

## Check whether labels need to move বাইরে the pie <!-- role: check -->

**Failure Sign:** Labels look cramped inside narrow wedges or do not fit cleanly.
**Quick Check:** Inspect the smallest slices and the longest labels first; if they do not fit comfortably, move them outside.
**Stronger Test:** Compare an inside-label draft with an outside-label draft and keep the version with cleaner labels.

## Fix pie label placement <!-- role: fix -->

- Move the labels for the smallest slices outside the circle.
- Move long labels outside even if the slice is not the smallest.
- Keep inside labels only for wedges that can hold them cleanly.
