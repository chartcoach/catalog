---
id: group-related-marks-with-proximity-and-color
title: Arrange related marks together and give them a shared visual identity
bibliography: references.bib
description: For grouped comparison tasks, use layout structure and shared color on
  grouped charts to improve readability and mitigate hard-to-see group membership
  for readers scanning many categories.
labels:
- purpose:refine
- basis:empirical
- task:compare
- scope:grouped-result
- quality:readability:use
- lever:layout-structure
- channel:color-hue:use
- group-cardinality:many
---

## Make groups visible <!-- role: advice -->

Place items from the same group next to one another and encode that group with a consistent color. For example, reorder bars so all members of a region are contiguous and share a hue instead of scattering same-group bars through a single list.

## Why visible grouping works <!-- role: reason -->

Vision automatically forms groups from proximity and shared appearance. When the chart's layout and color match the real grouping in the data, comparisons between groups become easier to find and hold.

**Mechanism:** Contiguity and shared color let readers perceive collections directly, which reduces the effort needed to discover which marks belong together.

**Evidence:** The paper explains that visual grouping is driven by proximity and shared color, then shows a grouped bar example where color helps somewhat but color plus spatial contiguity makes region comparisons much easier [@zacksDesigningGraphsDecisionMakers2020].

## Use when group comparison is important <!-- role: context -->

- **User Goal:** Compare groups rather than only individual items.
- **Task:** Grouped comparison.
- **Data:** Multiple items belong to a smaller set of groups.
- **Chart Setting:** Same-group marks are currently mixed into one flat arrangement.
- **Audience:** Readers scanning many categories.
- **Success Criterion:** Readers can see group membership and compare groups without tracing item by item.

## Do not use when outliers are the main message <!-- role: exceptions -->

**Break it when:** A member falls far from the rest of its group and that outlier is important to notice. **Why:** Strong grouping can cause that item to be missed, mis-categorized, or never compared with its group.

## Prioritize groups over a flat list <!-- role: costs -->

**Sacrifice:** The layout prioritizes group structure over a single undifferentiated ordering.
**Risk:** An important outlier can disappear inside the grouping logic.
**Mitigation:** Inspect grouped displays for separated or atypical members and make them visible.

## Avoid weak grouping cues <!-- role: mistakes -->

**Mistake:** Using color alone while leaving members of the same group noncontiguous. **Why it fails:** Readers still have to search the full chart to assemble the group.

## Check whether the group can be seen as a collection <!-- role: check -->

**Failure Sign:** Readers must trace labels one by one to tell which items belong together.
**Quick Check:** Look for members of the same group separated by unrelated marks.
**Stronger Test:** Ask someone to compare groups; if they must scan back and forth across the whole display, the grouping is too weak.

## Align the layout with the grouping <!-- role: fix -->

- Reorder the marks so members of each group are contiguous.
- Apply one consistent color to each group.
- If an important outlier sits apart from its group, call attention to it instead of letting the grouping hide it.
