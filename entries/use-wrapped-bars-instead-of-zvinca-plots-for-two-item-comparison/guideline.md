---
id: use-wrapped-bars-instead-of-zvinca-plots-for-two-item-comparison
title: Use wrapped bars instead of Zvinca plots for two-item comparison
bibliography: references.bib
description: For two-item comparison in dense record lists, use wrapped bars on ranked-list
  views instead of Zvinca plots to improve fidelity and mitigate pairwise size-estimation
  errors for readers making perceptual comparisons.
labels:
- purpose:select
- basis:empirical
- task:compare
- chart:bar:use
- chart:dotplot:avoid
- quality:fidelity:use
- lever:chart-family
- density:dense
---

## Wrapped bars for pairwise comparison <!-- role: advice -->

Choose a wrapped bar layout when readers must decide which of two items is larger and by how much in a long ranked list. For example, use wrapped bars rather than a Zvinca plot when both items need to stay visible on one screen and comparison accuracy matters more than the fastest possible response.

## Why wrapped bars work here <!-- role: reason -->

Bar length supported more accurate two-item size judgments than the dot-based Zvinca layout in this study. The wrapped layout kept the list compact without dropping to the lowest-accuracy condition.

**Mechanism:** Wrapped bars preserve length comparisons for two marked items while keeping all items visible, which helps pairwise magnitude judgments.

**Evidence:** For two-item comparison, wrapped bars were in the top accuracy tier and significantly outperformed Zvinca plots, while Zvinca plots had the fastest completion times [@zengReviewCollationGraphical2023; @mylavarapuRankedListVisualizationGraphical2019].

**Notes:** The evidence comes from low-level perceptual comparison tasks on unlabeled ranked-list charts.

## Use when all of these are true <!-- role: context -->

- **User Goal:** Compare two highlighted items and estimate the difference between them.
- **Task:** Pairwise magnitude comparison inside one ranked list.
- **Data:** A sorted ranked list with many items.
- **Chart Setting:** The full list should remain visible within one display.
- **Success Criterion:** Lower comparison error matters more than minimum response time.

## Do not use when any of these are true <!-- role: exceptions -->

**Break it when:** the main success criterion is fastest completion time for two-item comparison. **Why:** Zvinca plots were the fastest condition on this task.

## Tradeoffs of wrapped bars here <!-- role: costs -->

**Sacrifice:** You give up speed relative to Zvinca plots.
**Risk:** Per-column baselines can still make some across-column judgments less direct.
**Mitigation:** Use this choice when comparison accuracy is the primary requirement, then test it on representative long lists.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Choosing the fastest dot-based layout by default for pairwise comparison. **Why it fails:** the fastest condition here also had the lowest comparison accuracy.

## How to check the choice <!-- role: check -->

**Failure Sign:** Readers answer quickly but often miss which of two highlighted items is larger.
**Quick Check:** A/B test a wrapped-bar version against a Zvinca version using two-item comparison questions.
**Stronger Test:** Compare normalized absolute comparison error and completion time across representative list sizes.

## What to change <!-- role: fix -->

- Replace the Zvinca plot with a wrapped bar layout for the comparison view.
- Keep value encoded by bar length rather than dot position alone.
- Keep the list sorted and wrapped into columns so the full set remains visible without scrolling.
