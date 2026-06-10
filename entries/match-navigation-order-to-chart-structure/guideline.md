---
id: match-navigation-order-to-chart-structure
title: Match navigation order to the chart's narrative and data structure
bibliography: references.bib
description: For interactive chart exploration, use structure-matched navigation order
  on charts with narrative text and grouped or nested data to improve accessibility
  and mitigate serial focus paths that ignore the chart's organization for keyboard-only
  and screen-reader users.
labels:
- purpose:refine
- basis:accessibility
- scope:grouped-result
- quality:accessibility
- lever:interaction-access
- needs:keyboard-only
- needs:screen-reader
- access:keyboard:use
---

## Structure-matched navigation <!-- role: advice -->

Match keyboard navigation and reading order to the chart's narrative and data structure. For example, make the title, description, and annotations reachable before individual marks, let a stacked bar chart or treemap move across siblings and between levels, and also expose the same information in a linear table or list.

## Why structure-matched navigation works <!-- role: reason -->

Structure-matched navigation gives users the chart's overview before its details and lets them inspect grouped or nested data in the same organization the chart presents visually. This reduces the tedious point-by-point traversal that happens when focus follows only rendering order.

**Mechanism:** Users can move from summary to annotation to detailed data, and can switch across groups or levels instead of being trapped in one serial path.

**Evidence:** Chartability states that charts should be navigable in narrative order and that subgrouped or nested charts need keyboard movement between levels and laterally across levels, plus a linear or tabular path [@elavskyHowAccessibleMy2022]. The linked supporting work also describes navigation based on structure rather than only linear order for accessible diagrams and hierarchical data [@progressiveaccess_accessible_chemistry_2; @unknown_accessible_navigation_2015].

**Notes:** The structural path and the linear table or list path are complementary, not substitutes.

## When to apply it <!-- role: context -->

- **User Goal:** Understand the chart's takeaway and then inspect lower-level values.
- **Data:** The chart contains subgrouping, nesting, hierarchy, or another meaningful internal structure.
- **Chart Setting:** The chart includes navigable text such as a title, description, or annotations, and supports keyboard access.
- **Audience:** People using keyboards, screen readers, or other assistive technologies.
- **Success Criterion:** Users can reach high-level explanation first, then move through detailed data by group, level, or a linear table/list path.

## When not to apply the full pattern <!-- role: exceptions -->

**Break it when:** The chart has no subgrouping or nesting and only exposes a simple single-level sequence. **Why:** Level-switching or lateral controls would not map to a real structure, so only the ordered summary-to-detail path is needed.

## Costs of structure-matched navigation <!-- role: costs -->

**Sacrifice:** You must design more than one navigation path, including a structural path and a linear table or list path.
**Risk:** If every low-level mark is exposed as the main path, keyboard exploration can become unnecessarily tedious.
**Mitigation:** Put summary text and annotations before detailed marks, and provide a table or list for linear lookup.

## Common navigation failures <!-- role: mistakes -->

- **Mistake:** Leaving the default rendering or tab order as the only navigation path. **Why it fails:** Users can only move serially and cannot follow groups, categories, or levels in the chart.
- **Mistake:** Making users traverse detailed marks before they can reach the title, description, or annotations. **Why it fails:** The narrative and important takeaways are hidden behind low-level exploration.
- **Mistake:** Providing structural navigation without a linear table or list alternative. **Why it fails:** Users who need a simple linear path cannot access the same information in a comparable way.

## How to test it <!-- role: check -->

**Failure Sign:** Focus lands on marks in rendering order, and users cannot reach summary text first or move by group or level.
**Quick Check:** Starting at the chart, use only the keyboard and verify that focus reaches the title, description, and annotations before individual data marks.
**Stronger Test:** On a grouped or nested chart, verify that keyboard navigation can move across sibling groups or between levels and that the same information is available in a linear table or list.

## How to fix it <!-- role: fix -->

- Reorder the navigation sequence so the title, description, and annotations come before lower-level data marks.
- Add keyboard navigation that moves laterally across sibling groups and between levels in grouped or nested structures.
- Provide a linear table or list view that exposes the same data for sequential navigation.
- Add summary annotations for important regions so users do not have to inspect every mark one by one.
