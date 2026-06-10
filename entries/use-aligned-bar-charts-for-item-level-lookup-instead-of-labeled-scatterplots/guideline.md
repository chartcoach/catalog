---
id: use-aligned-bar-charts-for-item-level-lookup-instead-of-labeled-scatterplots
title: Use aligned bar charts instead of labeled scatter plots for item-level lookup
bibliography: references.bib
description: For item-level lookup in multi-measure record lists, prefer aligned bar
  charts over scatter plots to improve lookup fidelity and mitigate label-search problems
  for readers of static graphics.
labels:
- purpose:select
- basis:empirical
- task:retrieve
- scope:record-list
- chart:bar:use
- chart:scatter:avoid
- quality:fidelity:use
- lever:chart-family
- reading-mode:lookup
---

## Switch from labeled scatter to aligned bars for item lookup <!-- role: advice -->

Choose aligned bar charts when readers need to find values attached to individual items. For example, replace a labeled scatter plot with aligned bar charts that share the item axis so each row makes one item's values easy to locate and read.

## Why aligned bars help with item details <!-- role: reason -->

A scatter plot is strong for seeing general relationships, but it is weak when every point needs a readable identity. Aligned bars move the task from searching a field of labels to scanning a shared item axis.

**Mechanism:** The shared item axis gives each record a stable row, so readers can find one item and then read its values without fighting overlapping labels.

**Evidence:** The paper states that labeled scatter plots obscure point positions and make a given item difficult to find, and it presents aligned bar charts as the more effective alternative when the item details are important [@mackinlayAutomatingDesignGraphical1986].

## Use when item identities must stay visible <!-- role: context -->

- **User Goal:** Find the values for specific named items.
- **Task:** Retrieve item-level details rather than inspect only the global relationship.
- **Data:** Two or more measures share the same set of items.
- **Chart Setting:** A labeled scatter plot is a candidate, but the labels are needed to show item identities.
- **Success Criterion:** Readers can locate one item quickly and read its values directly.

## Keep the scatter plot when the overview matters more than the item details <!-- role: exceptions -->

**Break it when:** The details about the items can be omitted and the main goal is to see the general relationship among the measures. **Why:** Then the scatter plot shows the overall relationship more easily.

## Tradeoffs of choosing aligned bars <!-- role: costs -->

**Sacrifice:** The overall relationship among the measures is less immediate than in a scatter plot.
**Risk:** Readers may miss the broad pattern while focusing on row-by-row values.
**Mitigation:** Use aligned bars only when item lookup is the primary success criterion.

## Common wrong fix for detail-heavy scatter plots <!-- role: mistakes -->

**Mistake:** Keep the scatter plot and add labels to every point instead of changing the chart family. **Why it fails:** The labels create clutter while still leaving item lookup difficult.

## Compare the two chart choices directly <!-- role: check -->

**Failure Sign:** A reader must hunt through many point labels to find one item's values.
**Quick Check:** Mock both versions and ask which one lets you find one item's paired values with less scanning: the labeled scatter plot or the aligned bar charts.
**Stronger Test:** Verify that the chosen design gives each item a stable row or position that supports direct lookup without overlapping text.

## Replace the chart structure <!-- role: fix -->

- Rebuild the display as aligned bar charts that share the item axis.
- Put each measure in its own aligned bar panel rather than attaching labels to scatter plot points.
- Remove the per-point labels from the scatter plot if the item details are no longer required.
