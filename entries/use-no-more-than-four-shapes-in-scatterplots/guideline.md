---
id: use-no-more-than-four-shapes-in-scatterplots
title: Use no more than four shapes in grouped scatterplots
bibliography: references.bib
description: For grouped scatterplots, prefer shape encoding on point marks to improve
  accessibility and mitigate color-only grouping, and avoid large shape sets that
  create visual clutter for readers with color-vision deficiency.
labels:
- purpose:refine
- basis:heuristic
- chart:scatter
- quality:accessibility
- lever:encoding
- channel:shape:use
- group-cardinality:few
- needs:color-vision-deficiency
---

## Replace color-only grouping with a small shape set <!-- role: advice -->

Use distinct point shapes in a scatterplot when color alone separates groups. For example, replace some circles with triangles, rectangles, crosses, or stars, but stop at three or four shapes instead of giving every group a different marker.

## Why a small shape set works <!-- role: reason -->

Shapes provide a noncolor way to separate groups, but too many shape types overwhelm the display. A small, repeated set preserves group identity without turning the plot into visual confetti.

**Mechanism:** Shape differences survive color confusion, while limiting the number of shapes preserves a readable point field.

**Evidence:** The article recommends using different shapes in scatterplots instead of just circles and warns that using all those shapes quickly looks like confetti, advising a limit of three or four. [@muth_colorblindness_2020]

## Use when a scatterplot has a few groups <!-- role: context -->

- **User Goal:** Distinguish grouped points in a scatterplot.
- **Task:** Compare or identify categories in a point cloud.
- **Data:** A few groups encoded on the same scatterplot.
- **Chart Setting:** A scatterplot where color would otherwise be the only group marker.
- **Audience:** Readers who may include people with color-vision deficiency.
- **Success Criterion:** Groups remain distinguishable without the plot becoming cluttered.

## When shape encoding breaks down <!-- role: exceptions -->

**Break it when:** The scatterplot needs more than four distinct group markers. **Why:** The article warns that larger shape sets quickly make the plot look like confetti.

## Costs of adding point shapes <!-- role: costs -->

**Sacrifice:** You give up some visual uniformity in the point field.
**Risk:** Too many shapes create clutter and slow scanning.
**Mitigation:** Keep the shape set small and reuse only a few clearly distinct markers.

## Common scatterplot failure <!-- role: mistakes -->

**Mistake:** Encoding all groups with circles and asking readers to rely on color alone, or adding too many different shapes. **Why it fails:** The first choice depends entirely on color, and the second makes the plot visually noisy.

## How to verify point shapes <!-- role: check -->

**Failure Sign:** The plot either collapses into same-looking colored circles or turns into a field of many unrelated marker types.
**Quick Check:** Count the distinct shapes in the plot and keep the total at four or fewer.
**Stronger Test:** View the plot with color differences reduced and check whether groups still separate by marker shape.

## What to change <!-- role: fix -->

- Replace some circle-only groups with clearly different marker shapes.
- Limit the distinct marker set to three or four shapes.
- Merge or split groups differently if the plot would need more shapes than that.
