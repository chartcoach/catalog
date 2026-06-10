---
id: use-treemap-for-large-weighted-hierarchies
title: Use a treemap instead of a node-link tree when a weighted hierarchy must fit
  in one view
bibliography: references.bib
description: For overview of large weighted hierarchies, use a space-filling treemap
  instead of a node-link tree on hierarchical data to improve insight and mitigate
  screen-space overload for users scanning many levels at once.
labels:
- purpose:select
- basis:empirical
- chart:treemap:use
- chart:network:avoid
- data:hierarchical
- quality:insight
- lever:chart-family
- reading-mode:overview
- density:dense
---

## Choose a space-filling tree layout <!-- role: advice -->

Replace a full node-link tree with a treemap when the hierarchy is large and the display must show the whole structure at once. For example, use one screen-filling set of rectangles sized by leaf or subtree size instead of a rooted tree with lines when large items can appear at any level and the full node-link view no longer fits.

## Why the space-filling choice works <!-- role: reason -->

A space-filling tree layout turns nearly all available display area into data-carrying area. That lets readers scan the whole hierarchy at once and see large leaves wherever they occur, instead of spending space on links and indentation.

**Mechanism:** Area-proportional rectangles preserve relative size while using the full screen, so overview reading and large-item detection stay possible even when the tree has many levels and many leaves.

**Evidence:** The paper states that conventional rooted tree displays quickly overwhelm available display space so users cannot grasp the entire picture, and presents tree-maps as a 2-d space-filling representation that lets users rapidly recognize larger files anywhere in a large multi-level hierarchy [@shneidermanTreeVisualizationTreemaps1992].

## Use when the whole weighted tree must fit <!-- role: context -->

- **User Goal:** See the entire hierarchy and quickly spot the largest leaves.
- **Task:** Compare relative sizes across many leaves and levels in one view.
- **Data:** Hierarchical data with a meaningful size or weight on leaves or subtrees.
- **Chart Setting:** Limited screen space and a need to show the whole tree simultaneously.
- **Audience:** People inspecting large hierarchical collections.
- **Success Criterion:** The full hierarchy fits in one view and the largest leaves stand out immediately.

## Do not use when area cannot carry the tree information <!-- role: exceptions -->

- **Break it when:** The hierarchy has no meaningful size attribute to map to rectangle area. **Why:** The method depends on each node rectangle having area proportional to an attribute such as size.
- **Break it when:** Many tiny or zero-size leaves must all remain individually visible at the current display resolution. **Why:** The paper notes that very small or zero-byte items become too small to represent and may be eliminated.

## Costs of switching to a treemap <!-- role: costs -->

**Sacrifice:** You give up the explicit node-and-edge drawing of a rooted tree.
**Risk:** Very small leaves can disappear when the size range is large.
**Mitigation:** Add zooming or restrict the view to a selected subtree when small items cannot be shown clearly.

## Common failure mode in this choice <!-- role: mistakes -->

**Mistake:** Keeping a full rooted node-link tree on one screen for a very large weighted hierarchy. **Why it fails:** The links and indentation consume the display before the reader can see the whole hierarchy or quickly spot the largest leaves.

## How to test the chart-family decision <!-- role: check -->

**Failure Sign:** The full node-link tree does not fit comfortably on one screen or the largest leaves are hard to identify across levels.
**Quick Check:** Render the same hierarchy once as a node-link tree and once as a treemap; if only the treemap shows the whole hierarchy while keeping large leaves obvious, choose the treemap.
**Stronger Test:** Ask a reviewer to point out the largest leaves anywhere in the hierarchy from a single screen; prefer the design that supports that overview without scrolling or page turning.

## What to change <!-- role: fix -->

- Replace the full node-link tree view with a treemap.
- Size each treemap rectangle by the stored leaf or subtree total.
- Use the full display area for the treemap instead of reserving space for links and indentation.
- Add zooming or a subtree-focused view if the smallest leaves still disappear.
