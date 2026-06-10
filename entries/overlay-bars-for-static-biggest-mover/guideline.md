---
id: overlay-bars-for-static-biggest-mover
title: Use overlaid bars for static biggest-mover comparison
bibliography: references.bib
description: For comparison of two quantitative series in a biggest-mover task when
  the view must stay static, use an overlaid single-view layout on bar charts to improve
  fidelity and mitigate cross-panel comparison errors for viewers inspecting one pair
  at a time.
labels:
- purpose:select
- basis:empirical
- task:compare
- chart:bar
- structure:single-view:use
- structure:small-multiples:avoid
- lever:layout-structure
- operator:difference
---

## Overlaid bar comparison <!-- role: advice -->

Overlay the two bar series when a biggest-mover comparison must stay static. For example, draw both series in the same bar-chart frame instead of separating them into adjacent or stacked bar-chart panels.

## Why overlaid bars work for this task <!-- role: reason -->

A single overlaid view keeps corresponding values in one place, which reduces the need to store one panel in memory while inspecting another.

**Mechanism:** Co-locating the two series lets viewers compare differences directly within one region instead of making cross-panel matches.

**Evidence:** In the bar-chart maximum-delta experiment, overlaid bars outperformed every small-multiple arrangement, and the paper identifies overlay as the best static alternative when animation is not feasible for this task [@ondovFaceFaceEvaluating2019].

## Use when all of these are true <!-- role: context -->

- **User Goal:** Identify which category changed the most by absolute amount.
- **Task:** Compare exactly two bar-chart series in a static display.
- **Data:** One quantitative value per category in each of two series.
- **Chart Setting:** Motion is unavailable or inappropriate, such as a fixed comparison view.
- **Audience:** Viewers inspect one paired comparison at a time.
- **Success Criterion:** Readers can detect the biggest mover without needing very large changes.

## Do not use when any of these are true <!-- role: exceptions -->

**Break it when:** Motion is feasible and the task is still to find the single largest change. **Why:** Animated bar transitions performed even better than static overlays for this task.

## Tradeoffs of overlaid bars <!-- role: costs -->

**Sacrifice:** A layout that keeps the two series in separate panels.
**Risk:** This recommendation is only established here for two bar-chart series in the biggest-mover task.
**Mitigation:** Keep the overlay limited to one paired comparison and this specific task.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Use adjacent or stacked bar small multiples for a static biggest-mover view and expect the same comparison accuracy as a co-located display. **Why it fails:** The viewer must compare across panels instead of reading the difference in one shared frame.

## How to test this choice <!-- role: check -->

**Failure Sign:** Readers hesitate or disagree about the biggest mover in a static side-by-side comparison.
**Quick Check:** Show the same data once as an overlaid bar chart and once as adjacent bar small multiples, then ask readers after a brief glance which bar changed most.
**Stronger Test:** Lower the size of the winning change and keep the layout that still produces correct answers.

## What to change <!-- role: fix -->

- Superpose the two bar series in one plotting area.
- Remove the separate adjacent or stacked panels for this task.
- If motion becomes available, upgrade the same comparison to an animated transition.
