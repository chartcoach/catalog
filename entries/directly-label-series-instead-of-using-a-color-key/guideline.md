---
id: directly-label-series-instead-of-using-a-color-key
title: Directly label colored series instead of relying on a color key
bibliography: references.bib
description: For color-coded series identification, prefer direct labels on chart
  marks to improve readability and mitigate color-key decoding for readers with color-vision
  deficiency.
labels:
- purpose:refine
- basis:heuristic
- quality:accessibility
- lever:text-annotation
- component:label:use
- component:legend:avoid
- needs:color-vision-deficiency
- polish:annotation
---

## Move labels onto the marks <!-- role: advice -->

Label colored series directly on the chart instead of making readers decode them through a color key. For example, place series names next to lines or areas, or label pie slices directly so readers do not have to match colors back and forth with a legend.

## Why direct labels work <!-- role: reason -->

A color key forces readers to translate color into identity before reading the data. Direct labels remove that lookup step and keep identity attached to the mark itself.

**Mechanism:** Direct labels reduce back-and-forth scanning between the chart and the legend, making category identity readable even when colors are hard to distinguish.

**Evidence:** The article calls color keys a problem for colorblind people, recommends getting rid of them when possible, and specifically recommends direct labels for line, area, and pie charts. [@muth_colorblindness_2020]

## Use when the chart can carry labels on the marks <!-- role: context -->

- **User Goal:** Identify colored series or slices quickly.
- **Task:** Lookup and comparison of labeled series.
- **Data:** A small enough set of categories to label directly.
- **Chart Setting:** Chart types such as line, area, or pie where labels can sit on or near the marks.
- **Audience:** Readers who may include people with color-vision deficiency.
- **Success Criterion:** Readers can identify each series without consulting a color key.

## When not to force direct labels <!-- role: exceptions -->

**Break it when:** The chart type cannot place labels directly on the marks. **Why:** The article gives this recommendation for chart types where direct mark labeling is feasible, such as line, area, and pie charts.

## Costs of direct labeling <!-- role: costs -->

**Sacrifice:** You give up some empty space near the marks.
**Risk:** Keeping both direct labels and the old color key preserves the same split-attention problem.
**Mitigation:** Remove the color key once the direct labels carry the identity.

## Common labeling failure <!-- role: mistakes -->

**Mistake:** Leaving colored series unlabeled and expecting the legend to do all identification work. **Why it fails:** Readers must decode the legend before they can read the chart, and that is especially hard when colors are confusable.

## How to verify direct labeling <!-- role: check -->

**Failure Sign:** A reader still has to look at the legend to identify a line, area, or slice.
**Quick Check:** Cover the legend and see whether each marked category is still identifiable.
**Stronger Test:** Run a colorblind simulation and check whether the labels, not just the colors, still carry the identity.

## What to change <!-- role: fix -->

- Place a label directly next to each line or area.
- Label each pie slice directly instead of relying only on a legend.
- Remove the color key once direct labels provide the category names.
