---
id: use-hue-families-for-parent-groups-and-shades-for-subcategories
title: Use one hue per parent category and shades for its subcategories
bibliography: references.bib
description: For grouped categorical displays with nested categories, use hue for
  the parent groups and lightness variation within each hue for subcategories to improve
  readability and address overly fragmented category palettes for readers separating
  group levels.
labels:
- purpose:refine
- basis:heuristic
- data:hierarchical
- quality:readability
- lever:encoding
- channel:color-hue:use
- channel:color-lightness:use
---

## Nested hue families <!-- role: advice -->

Assign one hue to each parent category and vary the shades within that hue for its subcategories. For example, use blue and yellow for two top-level groups and lighter or darker blue and yellow for the territories, words, or countries that sit inside each group.

## Why nested hue families work <!-- role: reason -->

Hue carries the top-level grouping, while shade differences separate the members inside each group. When subcategories are directly labeled, color is freed from having to identify every item from a legend.

**Mechanism:** Readers first see which items belong together by hue family, then distinguish the members of that family by lightness differences.

**Evidence:** The article recommends using hues for broad categories and shades within those hues for subcategories, illustrating this with grouped areas where blue and yellow mark the main groups and shades distinguish the nested parts [@muth_quantitative_vs_qualitative_2021].

## Use when categories are nested <!-- role: context -->

- **User Goal:** Show both parent groups and their subcategories.
- **Task:** Distinguish hierarchy levels in one display.
- **Data:** Categories are grouped into larger categories.
- **Chart Setting:** Color is available to separate both levels.
- **Success Criterion:** Readers can see the parent grouping and still tell the child categories apart.

## Do not use when all categories are peers <!-- role: exceptions -->

**Break it when:** The main need is to distinguish peer categories rather than nested subcategories. **Why:** Separate hues distinguish peer categories more clearly than shades within the same hue.

## What this choice costs <!-- role: costs -->

**Sacrifice:** Child categories inside one parent are less distinct than if each had its own hue.
**Risk:** A monotone dark-to-light run can look like a value order even when the children are unordered.
**Mitigation:** Directly label the children or mix darker and lighter shades instead of arranging them as a strict sequence when no order is intended.

## Common grouping failure <!-- role: mistakes -->

**Mistake:** Give every subcategory its own unrelated hue. **Why it fails:** The parent grouping disappears and the display becomes harder to scan as groups.

## How to test the hierarchy cue <!-- role: check -->

**Failure Sign:** Reviewers cannot tell which child categories belong to the same parent without reading every label.
**Quick Check:** Step back and see whether each parent still reads as one hue family.
**Stronger Test:** Briefly ignore the labels; if the top-level grouping is no longer obvious, the palette is not carrying the hierarchy.

## How to revise it <!-- role: fix -->

- Assign a base hue to each parent category.
- Lighten and darken within that hue for the child categories.
- Directly label child categories if you do not want readers to infer a dark-to-light order.
- Switch peer categories to separate hues when they are not nested.
