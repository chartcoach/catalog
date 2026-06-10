---
id: separate-same-colored-categories-with-strokes
title: Add separating strokes between same-colored categories
bibliography: references.bib
description: For charts that group multiple categories with one shared color, use
  separating strokes on adjacent or overlapping marks to improve readability and mitigate
  lost boundaries for readers tracking individual categories.
labels:
- purpose:refine
- basis:heuristic
- lever:encoding
- group-cardinality:many
- quality:readability:use
- polish:hierarchy
---

## Outline same-colored marks <!-- role: advice -->

Add visible strokes between categories that share the same color. For example, draw white outlines around same-colored treemap cells or around overlapping same-colored lines so readers can still follow the individual categories inside each color group.

## Restore boundaries without adding more colors <!-- role: reason -->

Shared color can communicate a higher-level grouping, but it also makes neighboring categories blend together. A contrasting stroke restores the boundaries so readers can track the smaller units without breaking the color grouping.

**Mechanism:** The outline separates touching or overlapping marks while preserving the shared hue that signals the larger group.

**Evidence:** The post recommends keeping original categories visible inside same-colored groups by separating them with a stroke and shows examples that use white strokes around same-colored areas and lines [@muth_fewer_colors_2022].

## Use when shared color hides category boundaries <!-- role: context -->

- **User Goal:** Reduce the number of colors while keeping individual categories visible.
- **Task:** Let readers follow categories inside a higher-level color group.
- **Data:** Many categories are present within grouped totals.
- **Chart Setting:** Same-colored marks touch, overlap, or sit directly adjacent to one another.
- **Audience:** Readers trying to trace individual categories through the grouped display.
- **Success Criterion:** Shared-color groups stay readable as both groups and individual categories.

## Do not use when categories are already clearly separated <!-- role: exceptions -->

**Break it when:** Categories already have distinct colors or do not touch or overlap. **Why:** The stroke is solving a boundary problem that is not present.

## Accept a little extra visual structure <!-- role: costs -->

**Sacrifice:** The chart gains an additional visible styling layer.
**Risk:** Heavy strokes can compete with the data if overused.
**Mitigation:** Keep the stroke strong enough to separate boundaries without making it the main visual feature.

## Avoid same-color grouping without boundaries <!-- role: mistakes -->

**Mistake:** Giving several touching categories the same color without any separating stroke. **Why it fails:** The categories merge visually and become hard to follow.

## Hide the stroke to see whether it is needed <!-- role: check -->

**Failure Sign:** Adjacent or overlapping same-colored marks blend together.
**Quick Check:** Temporarily remove the stroke and see whether the categories become harder to trace.
**Stronger Test:** Inspect the places where same-colored marks touch or overlap and confirm that each category boundary remains visible.

## Add the boundary treatment <!-- role: fix -->

- Add a contrasting stroke between adjacent same-colored categories.
- Outline overlapping same-colored lines so each line can still be followed.
- Keep the shared color for the higher-level grouping instead of adding more hues.
