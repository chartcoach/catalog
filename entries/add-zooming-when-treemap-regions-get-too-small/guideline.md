---
id: add-zooming-when-treemap-regions-get-too-small
title: Add zooming when treemap regions become too small to inspect
bibliography: references.bib
description: For overview of large hierarchical treemaps on limited-resolution displays,
  use zooming on a treemap to improve readability and address regions that are too
  small to represent for users inspecting many items.
labels:
- purpose:refine
- basis:empirical
- chart:treemap
- data:hierarchical
- quality:readability
- lever:interaction-access
- access:zoom:use
- density:dense
---

## Add zooming for small regions <!-- role: advice -->

Add zooming when many treemap rectangles become too small to inspect at the current display resolution. For example, zoom into a dense portion of the hierarchy to reveal small files that disappear in the full overview.

## Why zooming works here <!-- role: reason -->

Treemaps can fit many items into one view, but resolution still limits how small a visible rectangle can be. Zooming restores inspectability when the overview has already pushed many items below a usable size.

**Mechanism:** Zooming increases the screen area available to a local subtree, so small leaves that were previously too small to represent can become visible and inspectable.

**Evidence:** The paper says a 640 × 480 display is adequate for about one to two thousand files on average, but with smaller displays or larger trees it may be necessary to add zooming to reveal small files because small or zero-byte files become too small to represent [@shneidermanTreeVisualizationTreemaps1992].

## Use when resolution limits the overview <!-- role: context -->

- **User Goal:** Inspect small items that disappear in the full treemap overview.
- **Task:** Move from overview to local detail without abandoning the treemap representation.
- **Data:** Large hierarchical trees with many small leaves or a wide range of sizes.
- **Chart Setting:** Limited display resolution relative to the number of items shown.
- **Audience:** Users inspecting large hierarchical collections on screen.
- **Success Criterion:** Small regions that matter can be brought into view instead of being eliminated or unreadable.

## Do not use when the current view already has enough detail <!-- role: exceptions -->

**Break it when:** The current display resolution and tree size already give adequate detail in the full treemap. **Why:** The paper notes that standard VGA resolution is already quite adequate for roughly one to two thousand files on average.

## Costs of adding zooming <!-- role: costs -->

**Sacrifice:** The user no longer sees the whole hierarchy at the same scale while zoomed in.
**Risk:** If used without need, zooming adds interaction overhead to a view that was already readable.
**Mitigation:** Reserve zooming for cases where small regions are too small to represent in the full overview.

## Common failure mode in this refinement <!-- role: mistakes -->

**Mistake:** Keeping only a fixed full treemap view when many small regions are too small to represent. **Why it fails:** The reader loses access to the small items entirely.

## How to test the zoom need <!-- role: check -->

**Failure Sign:** Many small items are invisible, unreadable, or dropped because their rectangles are too small.
**Quick Check:** Inspect the smallest visible regions in the full treemap; if important items cannot be seen at all, add zooming.
**Stronger Test:** Compare the full view with a zoomed view of a dense subtree and confirm that the zoomed version reveals small items that were previously too small to represent.

## What to change <!-- role: fix -->

- Add zoom controls to the treemap.
- Let the user zoom into dense subtrees until small regions become visible.
- Keep the full overview available as the starting view and use zoom only for local inspection.
- Use a larger display when available if the whole tree must remain visible at once.
