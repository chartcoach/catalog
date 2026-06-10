---
id: add-boundaries-between-same-colored-treemap-neighbors
title: Add boundary lines between adjacent treemap regions that share the same color
bibliography: references.bib
description: For overview of dense hierarchical treemaps, use boundary lines on same-colored
  adjacent regions in a treemap to improve readability and prevent neighboring areas
  from visually merging for users scanning many small rectangles.
labels:
- purpose:refine
- basis:empirical
- chart:treemap
- data:hierarchical
- quality:readability
- lever:layout-structure
- density:dense
---

## Outline same-colored neighbors <!-- role: advice -->

Draw a boundary line wherever two adjacent treemap rectangles use the same color or gray shade. For example, if neighboring tiles share the same file-type color, outline their shared edge so the two regions remain visibly separate.

## Why the extra boundary works <!-- role: reason -->

Color can separate neighboring regions only when the fills differ. When adjacent regions repeat the same fill, the partition becomes hard to see and the reader can misread multiple rectangles as one block.

**Mechanism:** A boundary line restores the lost partition cue when color no longer distinguishes neighboring regions.

**Evidence:** The paper says that different colors or gray shading are needed for visual clarity in tree-maps and that if adjacent areas have the same color, a boundary line will be necessary [@shneidermanTreeVisualizationTreemaps1992].

## Use when repeated colors touch <!-- role: context -->

- **User Goal:** Distinguish neighboring regions in a dense treemap.
- **Task:** Separate adjacent items while still using color to encode another attribute.
- **Data:** Hierarchical data with repeated attribute values mapped to color.
- **Chart Setting:** A treemap with many rectangles and at least one pair of adjacent same-colored regions.
- **Audience:** Readers scanning many small tiles.
- **Success Criterion:** Every neighboring region remains visibly distinct even when color repeats.

## Do not use when color already separates the neighbors <!-- role: exceptions -->

**Break it when:** Adjacent regions already differ in color or shading. **Why:** The paper makes the boundary line necessary specifically when adjacent areas have the same color.

## Costs of adding boundaries <!-- role: costs -->

**Sacrifice:** You add one more visible mark inside the treemap.
**Risk:** If applied everywhere, boundary lines can add unnecessary visual clutter where color already separates regions.
**Mitigation:** Limit the lines to adjacencies where the neighboring fills are the same.

## Common failure mode in this refinement <!-- role: mistakes -->

**Mistake:** Relying on color alone when same-colored treemap rectangles touch. **Why it fails:** The touching regions visually merge and the partition between items is lost.

## How to test the boundary treatment <!-- role: check -->

**Failure Sign:** Two neighboring rectangles with the same fill look like one larger block.
**Quick Check:** Scan every shared edge where adjacent regions have the same color; if the partition disappears, add a line.
**Stronger Test:** Compare the same treemap before and after outlining same-colored adjacencies and verify that each partition remains visible in the outlined version.

## What to change <!-- role: fix -->

- Draw a boundary line along every shared edge where neighboring rectangles use the same color or shade.
- Keep the existing color mapping for the encoded attribute and use the line only to separate touching same-colored regions.
- Review the final treemap after color assignment and outline every repeated-color adjacency that still visually merges.
