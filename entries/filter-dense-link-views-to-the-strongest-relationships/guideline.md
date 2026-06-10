---
id: filter-dense-link-views-to-the-strongest-relationships
title: Filter dense link views to the strongest relationships
bibliography: references.bib
description: For relationship analysis in dense link-based views, use a filtered subset
  of the strongest links to improve readability and mitigate link overload for analysts
  exploring many possible connections.
labels:
- purpose:refine
- basis:empirical
- task:relate
- operator:association
- density:dense
- quality:readability:use
- lever:interaction-access
---

## Filter link visibility by relationship strength <!-- role: advice -->

Filter the default link view to a salient subset when the number of relationships is large. For example, show only the strongest links in the initial display and let users reveal additional links through interaction instead of drawing every possible connection at once.

## Reduce link clutter so dominant associations stand out <!-- role: reason -->

A dense all-links view turns relationship reading into clutter management. Showing only the strongest subset keeps the major associations visible and makes the display usable as a starting point for exploration.

**Mechanism:** Thresholding lowers visual density, so viewers can detect important associations before asking the display to reveal weaker ones.

**Evidence:** The paper states that when the number of relationships was large, only relationships above the third quantile were encoded in the default view, and it also notes that interaction can be used to increase or decrease how much data is visible [@olaSimpleChartsDesign2016].

## Use when the relationship view is dense <!-- role: context -->

- **User Goal:** Identify the most important relationships first.
- **Task:** Explore associations across many linked items.
- **Data:** The number of possible relationships is large enough to crowd the display.
- **Chart Setting:** A link-based view where showing all connections at once creates heavy overlap.
- **Success Criterion:** The strongest relationships remain visible without the viewer fighting clutter.

## Do not use when the full relationship set is still readable <!-- role: exceptions -->

**Break it when:** The number of relationships is small enough that all links can be shown without clutter. **Why:** Filtering is unnecessary when the full set remains readable.

## Trade off completeness against readability <!-- role: costs -->

**Sacrifice:** You hide weaker relationships in the default state.
**Risk:** Relevant lower-strength associations may be missed if they are never revealed.
**Mitigation:** Let users increase or decrease the amount of visible data through interaction.

## Avoid showing every connection in the default state <!-- role: mistakes -->

**Mistake:** Drawing all possible links in a dense relationship view by default. **Why it fails:** The display becomes visually overloaded and the major associations stop standing out.

## Test whether link density blocks relationship reading <!-- role: check -->

**Failure Sign:** The link field looks like a mesh, and selected items do not reveal dominant associations quickly.
**Quick Check:** Compare the all-links view with a thresholded version and see which one lets a reviewer name the strongest relationships first.
**Stronger Test:** Select one item and ask a reviewer to identify its key connections; if the all-links version slows or blocks that reading, the default view is too dense.

## Apply a salience threshold and reveal more on demand <!-- role: fix -->

- Hide lower-strength links in the default view.
- Keep only the strongest subset visible at first.
- Add interaction that lets users reveal more links when they need a fuller relationship set.
