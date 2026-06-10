---
id: avoid-perfect-square-targets-in-rectangle-area-comparisons
title: Avoid perfect-square targets when readers must compare rectangle areas
bibliography: references.bib
description: For exact area comparison in area-based displays, avoid 1:1 aspect ratios
  on compared rectangles to improve fidelity and mitigate side-length heuristics for
  web viewers.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:treemap
- quality:fidelity
- lever:layout-structure
- channel:area:use
- reading-mode:exact
---

## Rectangle aspect ratio <!-- role: advice -->

Do not force compared rectangles to perfect squares when readers must judge area. For example, in treemaps and other rectangular area displays, allow slight deviations from 1:1 such as near-square rectangles instead of optimizing every compared rectangle to exact 1:1.

## Why non-square comparisons work better <!-- role: reason -->

Readers appear to use side lengths as cues when judging area, and that shortcut becomes least informative when both shapes are squares. Slight aspect-ratio differences give the eye more usable evidence for the area comparison.

**Mechanism:** When compared rectangles are both perfect squares, side-length comparison is a weaker proxy for area, which raises estimation error.

**Evidence:** In the rectangular area experiment, comparisons involving 1:1 aspect ratios produced the worst performance across both isolated rectangles and treemap displays. The paper interprets this result as evidence that viewers use one-dimensional length comparisons to help estimate area. [@heerCrowdsourcingGraphicalPerception2010]

**Notes:** The paper found no significant accuracy difference between isolated rectangle displays and treemap displays for this task.

## Use when rectangle area comparison matters <!-- role: context -->

- **User Goal:** Compare one rectangle's area against another accurately.
- **Task:** Exact or near-exact area judgment.
- **Data:** Quantitative values encoded as rectangular areas.
- **Chart Setting:** Treemap or other rectangular area display with near-square aspect ratios.
- **Audience:** Web viewers using standard displays.
- **Success Criterion:** Lower area-estimation error.

## Do not generalize this to extreme shapes <!-- role: exceptions -->

**Break it when:** Achieving the design would require extreme aspect ratios outside the tested near-square range. **Why:** The study tested moderate aspect ratios around square, and the paper explicitly notes that extreme aspect-ratio variation is expected to hamper area judgments.

## Costs of relaxing square optimization <!-- role: costs -->

**Sacrifice:** You give up the strict goal of making every rectangle as square as possible.
**Risk:** Blindly pushing away from 1:1 can create skinny rectangles that are also hard to compare.
**Mitigation:** Allow only moderate deviations from square, not extreme ones.

## Common aspect-ratio mistake <!-- role: mistakes -->

**Mistake:** Optimizing compared rectangles toward exact 1:1 when accurate area comparison is important. **Why it fails:** The study found square-vs-square comparisons to be the least accurate case.

## How to check rectangle aspect ratios <!-- role: check -->

**Failure Sign:** The rectangles being compared are both perfect squares.
**Quick Check:** Inspect the target rectangles; if the important comparison is square against square, expect higher error.
**Stronger Test:** Compare reader estimates on a 1:1 version against a version where the same rectangles are slightly non-square.

## How to fix rectangle aspect ratios <!-- role: fix -->

- Relax layout rules that force compared rectangles to exact 1:1.
- Allow moderate near-square aspect ratios instead of perfect squares for the compared rectangles.
- Avoid compensating by creating extreme skinny rectangles elsewhere.
