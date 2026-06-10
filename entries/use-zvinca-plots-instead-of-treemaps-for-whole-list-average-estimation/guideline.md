---
id: use-zvinca-plots-instead-of-treemaps-for-whole-list-average-estimation
title: Use Zvinca plots instead of treemaps for whole-list average estimation
bibliography: references.bib
description: For whole-list average estimation in dense record lists, use Zvinca plots
  on ranked-list views instead of treemaps to improve fidelity and mitigate mean-estimation
  errors for readers making overview judgments.
labels:
- purpose:select
- basis:empirical
- task:distribute
- chart:dotplot:use
- chart:treemap:avoid
- quality:fidelity:use
- lever:chart-family
- reading-mode:overview
---

## Zvinca plots for mean estimation <!-- role: advice -->

Choose a Zvinca plot when readers need an overview estimate of the average across all items in a long ranked list. For example, use a Zvinca plot rather than a treemap when the display must keep the whole list on one screen and the readout is the list's overall mean.

## Why Zvinca plots work here <!-- role: reason -->

The dot-based Zvinca layout supported better whole-list average judgments than the area-based treemap in this study. It also completed faster on the same task.

**Mechanism:** Dots positioned on a common scale make the overall center of the list easier to judge than average tile area in a treemap.

**Evidence:** For whole-list average estimation, Zvinca plots were in the top accuracy tier and significantly outperformed treemaps in both error and time [@zengReviewCollationGraphical2023; @mylavarapuRankedListVisualizationGraphical2019].

**Notes:** The evidence comes from low-level perceptual summary tasks on unlabeled ranked-list charts.

## Use when all of these are true <!-- role: context -->

- **User Goal:** Estimate the average across the full ranked list.
- **Task:** Whole-list summary judgment rather than item lookup.
- **Data:** A sorted ranked list with many items.
- **Chart Setting:** All items should remain visible in a single overview.
- **Success Criterion:** Lower mean-estimation error and faster completion both matter.

## Do not use when any of these are true <!-- role: exceptions -->

**Break it when:** the main task is single-item ranking or two-item comparison instead of whole-list average estimation. **Why:** Zvinca plots were among the weaker layouts for those item-focused tasks.

## Tradeoffs of Zvinca plots here <!-- role: costs -->

**Sacrifice:** You give up stronger performance on item-specific ranking and comparison tasks.
**Risk:** Treating the same Zvinca plot as a general-purpose ranked-list view can hurt accuracy once readers shift from overview to item-specific judgments.
**Mitigation:** Reserve this choice for overview or average-estimation views.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keeping a treemap for average estimation just because it fits the whole list on one screen. **Why it fails:** the treemap was both slower and less accurate than the Zvinca plot for this task.

## How to check the choice <!-- role: check -->

**Failure Sign:** Readers struggle to place the average of the full list consistently.
**Quick Check:** A/B test a Zvinca plot against a treemap with whole-list average questions on representative long lists.
**Stronger Test:** Compare normalized absolute mean-estimation error and completion time across several list sizes.

## What to change <!-- role: fix -->

- Replace the treemap with a Zvinca plot for the overview summary view.
- Encode values as dots on a shared horizontal scale instead of area tiles.
- If the same display must mainly support ranking or pairwise comparison, switch away from the Zvinca plot for that task.
