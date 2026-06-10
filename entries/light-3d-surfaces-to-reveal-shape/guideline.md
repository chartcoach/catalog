---
id: light-3d-surfaces-to-reveal-shape
title: Light 3D surfaces to reveal local variation and global form
bibliography: references.bib
description: For compare and overview tasks on 3D surface displays of one quantitative
  measure across two variables, use surface lighting on the mesh to improve insight
  and address flat-shaded views that hide local variation for readers inspecting both
  anomalies and overall shape.
labels:
- purpose:refine
- basis:empirical
- task:compare
- data:quantitative
- quality:insight
- lever:encoding
- channel:color-lightness:use
- reading-mode:overview
---

## Surface lighting and highlights <!-- role: advice -->

Use lighting and shading on a 3D surface when readers need to see both the broad surface shape and subtle local deviations. For example, render a quantitative grid as a lit surface with visible highlights instead of relying on uniformly shaded bar faces that flatten local structure.

## Why lighting helps surface reading <!-- role: reason -->

A lit surface exposes shape continuously across the display, so small bends and local irregularities become visible without losing the broad structure. The paper's comparison shows that flat bar faces conceal variation that surface shading and highlights reveal immediately.

**Mechanism:** Lighting turns the surface itself into a readable shape cue, letting viewers see curvature, smooth trends, and small local departures in the same view.

**Evidence:** The paper states that shading and specular highlights can reveal subtle variations on a surface that are harder to see in a 2D heatmap or a bar grid, and it illustrates that a lit surface exposes both macro form and local day-to-day shifts more clearly than uniformly shaded bars [@brath3DInfoVisHere2014].

## Use when the surface shape is the message <!-- role: context -->

- **User Goal:** Understand the overall form of a quantitative surface while also spotting local anomalies.
- **Task:** Compare local departures against a larger continuous structure.
- **Data:** One quantitative measure defined over two independent variables.
- **Chart Setting:** A 3D surface or other continuous height field where shape is more important than isolated bar faces.
- **Audience:** Readers who need both overview and detail in one display.
- **Success Criterion:** The broad curvature and the small local shifts are both visible without calculating a separate difference view.

## When this breaks <!-- role: exceptions -->

**Break it when:** The lighting is reduced to a badly lit setup such as a headlight or a single poorly chosen directional light. **Why:** The paper explicitly warns that bad lighting makes a 3D scene easy to misread and can hide the very surface variation the technique is supposed to reveal.

## What you trade away <!-- role: costs -->

**Sacrifice:** You give up the simpler literalism of separate bars.
**Risk:** Poor lighting choices can make the surface harder, not easier, to interpret.
**Mitigation:** Treat lighting as an intentional design choice rather than a default renderer effect.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Show the data as a grid of flat-shaded bars and expect local structure to remain visible. **Why it fails:** Uniformly shaded faces mask fine variation and break the continuity of the underlying surface.

## How to check it <!-- role: check -->

**Failure Sign:** The surface looks generally flat, and local bends are only noticeable after deriving a separate difference chart.
**Quick Check:** Scan for highlights and shadows that track small surface changes across neighboring cells.
**Stronger Test:** Compare the lit surface against a flat bar rendering of the same values and see which one reveals both the large-scale shape and the local departures.

## What to change <!-- role: fix -->

- Render the quantitative field as a continuous surface instead of a collection of flat-shaded bars.
- Add lighting that creates readable shading and highlights across the surface.
- Rework the lighting if local variation disappears or if one global light washes the surface flat.
