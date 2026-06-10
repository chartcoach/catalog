---
id: show-treemap-details-on-demand
title: Show item details on demand for dense treemap regions
bibliography: references.bib
description: For lookup in dense treemaps, use on-demand detail readouts on selected
  treemap regions to improve readability and address the lack of space for persistent
  item labels for users inspecting item metadata.
labels:
- purpose:refine
- basis:empirical
- chart:treemap
- quality:readability
- lever:interaction-access
- reading-mode:lookup
- density:dense
- component:tooltip:use
---

## Use cursor-triggered detail readouts <!-- role: advice -->

Show the selected region's details only when the user points to or clicks a treemap rectangle. For example, display the item name, extension, or date at the bottom of the screen or just above the cursor, and expose item actions through a pop-up menu when needed.

## Why on-demand detail works <!-- role: reason -->

Dense treemaps cannot carry full item labels inside every rectangle without consuming the space needed for the overview. On-demand detail lets the reader inspect a candidate region without turning the whole display into text.

**Mechanism:** Interactive readout separates overview from lookup, so the treemap can stay space-filling while still supporting access to names and metadata.

**Evidence:** The paper says users need to inspect names and metadata in treemap regions and gives a cursor-plus-click readout at the bottom line of the screen or above the cursor as the interaction, with pop-up menus for operations as the next step [@shneidermanTreeVisualizationTreemaps1992].

## Use when overview and lookup must coexist <!-- role: context -->

- **User Goal:** Inspect the name or metadata of a specific treemap region after spotting it in the overview.
- **Task:** Lookup of item details such as name, extension, or date.
- **Data:** Many small hierarchical leaves packed into one treemap.
- **Chart Setting:** Cursor-based interaction is available and persistent labels would consume too much space.
- **Audience:** Users exploring dense hierarchical collections.
- **Success Criterion:** A user can inspect a small region's details without cluttering the full treemap with text.

## Do not use when labels must stay visible in the layout <!-- role: exceptions -->

**Break it when:** The design must keep container names or levels visible continuously inside the treemap. **Why:** The paper suggests nested containing frames for that need, even though they reduce effective display space.

## Costs of using on-demand detail <!-- role: costs -->

**Sacrifice:** Details are not visible until the user points or clicks.
**Risk:** Important metadata can remain hidden if the readout behavior is hard to find.
**Mitigation:** Put the readout in a consistent place such as the bottom line of the screen or just above the cursor.

## Common failure mode in this refinement <!-- role: mistakes -->

**Mistake:** Leaving dense treemap regions without any way to retrieve names or metadata. **Why it fails:** Users can see a candidate region but cannot examine the information needed to act on it.

## How to test the detail interaction <!-- role: check -->

**Failure Sign:** A user can identify a region visually but cannot retrieve its name or metadata from the display.
**Quick Check:** Move the cursor onto a small rectangle and click; the relevant details should appear at the bottom of the screen or near the cursor.
**Stronger Test:** Inspect several small rectangles in sequence and confirm that the details appear without adding persistent labels to the treemap.

## What to change <!-- role: fix -->

- Add a cursor-triggered readout for the selected rectangle.
- Place the readout at the bottom line of the screen or just above the cursor.
- Include the specific metadata users need, such as name, extension, or date.
- Add a pop-up menu if the workflow also requires actions such as deletion, copying, or marking.
