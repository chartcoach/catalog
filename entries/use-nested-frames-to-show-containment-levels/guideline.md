---
id: use-nested-frames-to-show-containment-levels
title: Use nested containing frames when the treemap must show parent levels
bibliography: references.bib
description: For overview of hierarchical treemaps, use nested containing frames on
  a treemap to improve readability and address hidden containment when users need
  parent levels or container names visible.
labels:
- purpose:refine
- basis:empirical
- chart:treemap
- data:hierarchical
- quality:readability
- lever:layout-structure
- reading-mode:overview
---

## Add containing frames for parent levels <!-- role: advice -->

Draw nested containing frames when the treemap must show parent levels instead of only leaf rectangles. For example, surround each parent region with a visible frame so three or four hierarchy levels remain visible in the same display.

## Why nested frames work <!-- role: reason -->

A plain treemap emphasizes the leaf rectangles, but it can hide the parent containers unless the hierarchy is drawn into the layout. Nested frames restore the visible containment structure without abandoning the space-filling view.

**Mechanism:** Parent frames make containment readable directly in the layout, so the viewer can see which leaves belong together and where levels change.

**Evidence:** The paper says nested rectangles showing a containing frame can be used when directory names are desired, and Figure 3 is described as using nested boxes to show levels in the treemap [@shneidermanTreeVisualizationTreemaps1992].

## Use when containment must remain visible <!-- role: context -->

- **User Goal:** See both leaf sizes and the parent grouping that contains them.
- **Task:** Read containment levels from the treemap layout.
- **Data:** Hierarchical data with named interior nodes that matter to the reading task.
- **Chart Setting:** A treemap where level visibility is required in addition to leaf-size overview.
- **Audience:** Readers who need to identify parent groupings while scanning the treemap.
- **Success Criterion:** The viewer can tell which leaves belong to the same parent and where levels change.

## Do not use when display area is the dominant constraint <!-- role: exceptions -->

**Break it when:** Preserving the maximum effective display space for the data regions is more important than showing parent levels. **Why:** The paper notes that nested containing frames reduce the effective display space.

## Costs of adding containing frames <!-- role: costs -->

**Sacrifice:** Some of the screen area is taken by the containing frames instead of the data regions.
**Risk:** If overused, the frames can reduce the space available for leaf rectangles.
**Mitigation:** Use the framed version only when parent levels or container names are required.

## Common failure mode in this refinement <!-- role: mistakes -->

**Mistake:** Showing only leaf rectangles when the reading task also depends on seeing the parent containers. **Why it fails:** The viewer cannot easily recover the containment levels from the layout alone.

## How to test the need for containing frames <!-- role: check -->

**Failure Sign:** A reviewer can see leaf areas but cannot tell which leaves share the same parent.
**Quick Check:** Ask whether a reader can identify the containing group for a chosen leaf directly from the treemap.
**Stronger Test:** Compare the plain treemap with a framed version and verify that the framed version makes the parent levels visible without changing the leaf-size encoding.

## What to change <!-- role: fix -->

- Draw a visible containing frame around each parent region that must remain legible.
- Use the nested-frame version when the task depends on reading hierarchy levels from the layout.
- Remove or simplify the frames again if they reduce the effective display space too much.
