---
id: remove-unnecessary-3d-from-2d-charts
title: Remove unnecessary 3D from charts shown in 2D media
bibliography: references.bib
description: For quantitative charts shown in 2D media, avoid 3D rendering on charts
  to prevent occlusion and perceptual ambiguity and mitigate projection distortion
  for readers comparing values at a glance.
labels:
- purpose:refine
- basis:empirical
- quality:fidelity
- lever:encoding
- aesthetic:style:avoid
- reading-mode:overview
---

## 3D removal <!-- role: advice -->

Remove 3D depth from charts that will be read on a flat page or screen. For example, replace 3D bars or a tilted 3D pie with a flat 2D chart, and encode any extra variable with color or size instead of depth.

## Why 3D hurts value reading in flat media <!-- role: reason -->

Flat displays remove many depth cues that help people judge real 3D scenes. Once depth is projected onto 2D, marks can hide each other, angles can change, and size can become confused with distance.

**Mechanism:** Removing 3D eliminates occlusion, projection distortion, and depth ambiguity, so more of the data stays visible and comparable. A flat 2D view makes position, size, and angle easier to interpret correctly.

**Evidence:** The paper identifies three problems with 3D charts in 2D media—occlusion, projection, and perceptual ambiguity—and shows how 3D bars and tilted 3D pies distort values or hide data that a 2D alternative reveals more clearly [@szafirGoodBadBiased2018].

## Use when the chart is read from a fixed flat view <!-- role: context -->

- **User Goal:** Compare values, ranks, or parts accurately.
- **Task:** Read quantitative differences from a static view.
- **Data:** Quantitative variables that do not require a literal 3D shape to be understood.
- **Chart Setting:** Slides, papers, or other 2D media where readers cannot freely resolve depth.
- **Audience:** Readers must interpret the chart from one viewpoint.
- **Success Criterion:** Marks remain visible and value judgments do not depend on depth guesswork.

## Do not use when 3D shape is itself necessary context <!-- role: exceptions -->

**Break it when:** The data has an inherent 3D form that provides necessary context, such as spatial structures. **Why:** The source notes that 3D can be useful there, though it is still imperfect and should be paired with 2D summaries.

## What you trade away <!-- role: costs -->

**Sacrifice:** You lose a dramatic or futuristic visual style.
**Risk:** If depth was carrying a third variable, removing it can drop information unless you remap that variable.
**Mitigation:** Encode the third variable with color or size, or pair a required 3D view with a 2D summary.

## Common 3D failure <!-- role: mistakes -->

**Mistake:** Adding perspective depth for style in a chart meant for value comparison. **Why it fails:** Some marks become hidden, projected angles and sizes change with depth, and distant small marks become visually ambiguous.

## How to review a 3D chart <!-- role: check -->

**Failure Sign:** Some marks are partially hidden, harder to read, or visibly distorted by depth.
**Quick Check:** Inspect whether any bar, slice, or mark is occluded or appears changed mainly because it sits farther back.
**Stronger Test:** Compare the chart with a flat 2D version; if values become easier to rank or compare, remove the 3D treatment.

## What to change <!-- role: fix -->

- Remove perspective depth and redraw the chart in 2D.
- Map any extra variable to color or size instead of depth.
- Replace a tilted 3D part-whole chart with a flat part-whole or bar-based alternative.
- If a 3D structure must remain for context, add a 2D summary view beside it.
