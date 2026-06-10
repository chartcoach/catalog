---
id: overlay-slope-charts-for-biggest-mover
title: Overlay slope charts for biggest-mover comparison
bibliography: references.bib
description: For comparison of two quantitative series in a biggest-mover task, prefer
  an overlaid layout on slope charts to improve fidelity and mitigate missed largest-change
  judgments for viewers comparing one pair at a time.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:line
- lever:layout-structure
- operator:difference
- group-cardinality:binary
- quality:fidelity:use
---

## Overlaid slope layout <!-- role: advice -->

Overlay the two slope-chart series when the job is to find the largest change. For example, draw both slope sets in the same frame instead of morphing one set of slopes into the other.

## Why overlaid slope charts work for this task <!-- role: reason -->

In slope charts, co-locating the two series makes the change easier to read than turning that change into motion.

**Mechanism:** An overlaid slope view lets viewers compare the two orientations directly in one place instead of following a transient animated transformation.

**Evidence:** In the slope-chart maximum-delta experiment, overlaid slopes outperformed animated slopes and every small-multiple arrangement, while mirrored small multiples showed no benefit [@ondovFaceFaceEvaluating2019].

## Use when all of these are true <!-- role: context -->

- **User Goal:** Identify which slope changed the most between two series.
- **Task:** Compare exactly two slope-chart series.
- **Data:** One quantitative value per item in each of two series.
- **Chart Setting:** A slope-chart representation is already chosen for the comparison.
- **Audience:** Viewers inspect one paired comparison at a time.
- **Success Criterion:** Readers can still pick the largest change when the difference is subtle.

## Do not use when any of these are true <!-- role: exceptions -->

**Break it when:** The same biggest-mover task is shown with bar charts or donut charts instead of slope charts. **Why:** In those chart families, animation rather than overlay was the stronger arrangement.

## Tradeoffs of overlaid slope charts <!-- role: costs -->

**Sacrifice:** Motion as a direct cue to change.
**Risk:** This choice is chart-specific and should not be generalized from slopes to bars or donuts.
**Mitigation:** Keep this rule limited to slope-chart comparisons.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Animate slope charts because animation helped in other chart families. **Why it fails:** The slope-chart results favored static overlay, not motion.

## How to test this choice <!-- role: check -->

**Failure Sign:** Readers miss the largest changing slope in an animated view.
**Quick Check:** Show the same two slope-chart series once overlaid and once animated, then ask readers after a brief glance which slope changed most.
**Stronger Test:** Reduce the winning change across trials and keep the layout that still supports correct answers.

## What to change <!-- role: fix -->

- Superpose both slope-chart series in one frame.
- Remove the animated morph for this task.
- If the comparison is actually a bar or donut version of the same task, test animation instead.
