---
id: use-dot-plots-when-grouped-bars-get-crowded
title: Use a dot plot when grouped bars get crowded
bibliography: references.bib
description: For comparing multiple values within each category, prefer a dot plot
  over grouped bar charts to improve readability and mitigate crowded multi-value
  category displays for general audiences.
labels:
- purpose:select
- basis:heuristic
- chart:dotplot:use
- chart:bar:avoid
- density:dense
- measure:multi
- lever:chart-family
- quality:readability
---

## Dot plots for crowded grouped comparisons <!-- role: advice -->

Switch from grouped bars to a dot plot when each category contains more than a couple of values or when the chart has little room. For example, compare several values within each category with dots rather than clustered bars once the grouped version starts to sprawl.

## Why dots hold up better in crowded grouped comparisons <!-- role: reason -->

Grouped bars work well for small sets, but they become bulky as more values are added or space shrinks. Dots keep the same comparison with less visual bulk.

**Mechanism:** Dots preserve category-by-category comparison while taking less space than repeated grouped bars.

**Evidence:** Grouped bars are described as a great option for comparing two or three values within a category, while dot plots are recommended especially when there are more than just a couple of values per category and/or not much space for a chart [@muth_chart_types_guide_2025].

## Use when grouped bars start to sprawl <!-- role: context -->

- **User Goal:** Compare several values within each category.
- **Task:** Keep within-category comparisons readable as the number of values grows.
- **Data:** Categories with more than a couple of values to compare.
- **Chart Setting:** A grouped comparison with limited space.
- **Audience:** A mainstream audience.
- **Success Criterion:** Each category remains readable without a bulky cluster of bars.

## Do not use when the grouped comparison is still small and roomy <!-- role: exceptions -->

**Break it when:** Each category has only two or three values and the chart has enough space. **Why:** Grouped bars are already a great option in that situation.

## Costs of switching to dots <!-- role: costs -->

**Sacrifice:** You give up the bar-based grouped display.\
**Risk:** If the comparison set is still small, the switch may not improve the chart.\
**Mitigation:** Change to dots only after grouped bars get crowded or space gets tight.

## Common failure with grouped bars <!-- role: mistakes -->

**Mistake:** Keep adding more bars to each grouped cluster after there are more than a couple of values. **Why it fails:** The grouped bars become crowded and take more space than the comparison needs.

## Check whether the grouped bars have become too bulky <!-- role: check -->

**Failure Sign:** Each category contains several narrow clustered bars or the chart is struggling to fit in the available space.\
**Quick Check:** Compare one grouped-bar draft with a dot-plot draft; if the dot plot fits more comfortably and keeps the comparisons clearer, switch to dots.\
**Stronger Test:** Ask whether the grouped bars still read as clear small sets rather than as crowded clusters.

## Fix the crowded grouped comparison <!-- role: fix -->

- Replace each grouped bar cluster with aligned dots.
- Keep one dot per value within each category.
- Retain grouped bars only for the smaller two- or three-value cases.
