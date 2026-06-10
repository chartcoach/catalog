---
id: overlay-paired-slope-series-for-largest-change-comparisons
title: Overlay paired slope series to improve largest-change comparison
bibliography: references.bib
description: For difference comparison between two paired quantitative series, use
  an overlaid layout on slope charts to improve fidelity and mitigate missed largest-change
  judgments for brief visual comparison.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:line
- quality:fidelity:use
- lever:layout-structure
- operator:difference
- group-cardinality:binary
---

## Overlay the paired slopes <!-- role: advice -->

Place the two slope series in one shared panel when the goal is to spot the biggest absolute change. For example, replace stacked, adjacent, or mirrored slope-chart small multiples with one overlaid slope view.

## Why overlay helps slope comparison <!-- role: reason -->

A shared slope panel keeps the compared lines together, so readers can judge the largest change directly instead of comparing across separate panels.

**Mechanism:** Overlay removes cross-panel lookup and makes the largest slope difference easier to see in one place.

**Evidence:** In the collated record, the overlaid slope arrangement ranked above the stacked, adjacent, and mirrored slope arrangements for the largest-change task; the original experiment reported the same advantage for the tested slope-chart layouts [@zengReviewCollationGraphical2023; @ondovFaceFaceEvaluating2019].

## Use when finding the biggest change <!-- role: context -->

- **User Goal:** Identify which item changed the most between two series.
- **Task:** Compare absolute change across paired values.
- **Data:** Two paired quantitative series.
- **Chart Setting:** Slope charts shown under brief viewing.
- **Success Criterion:** Readers can pick the biggest mover with subtler differences.

## Do not use as a general slope-layout rule <!-- role: exceptions -->

**Break it when:** The task is not locating the single biggest change between the two series. **Why:** The study did not establish one arrangement as universally best across tasks.

## Tradeoffs of overlaid slopes <!-- role: costs -->

**Sacrifice:** Separate panels for each series.
**Risk:** This advantage was established for the largest-change task, not as a universal slope-chart rule.
**Mitigation:** Use the overlaid slope layout specifically when the task is to find the largest change.

## Common slope-layout mistake <!-- role: mistakes -->

**Mistake:** Keep the slope series in separated small-multiple panels for biggest-mover reading. **Why it fails:** All tested small-multiple slope arrangements ranked below the overlaid layout.

## Check the slope-layout choice <!-- role: check -->

**Failure Sign:** Readers miss the biggest mover unless the largest change is obvious.
**Quick Check:** Compare the overlaid slope view against any split slope layout on a brief biggest-change judgment.
**Stronger Test:** Keep the version that supports correct picks with smaller deltas.

## Repair the slope layout <!-- role: fix -->

- Collapse the two slope panels into one shared plotting area.
- Keep both slope series visible at the same time.
- If the view must stay split, do not expect stacked, adjacent, or mirrored small multiples to match the overlaid advantage for this task.
