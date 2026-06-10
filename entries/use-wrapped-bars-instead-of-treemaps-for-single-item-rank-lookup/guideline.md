---
id: use-wrapped-bars-instead-of-treemaps-for-single-item-rank-lookup
title: Use wrapped bars instead of treemaps for single-item rank lookup
bibliography: references.bib
description: For single-item rank lookup in dense record lists, use wrapped bars on
  ranked-list views instead of treemaps to improve fidelity and mitigate item-rank
  errors for readers making perceptual rank judgments.
labels:
- purpose:select
- basis:empirical
- chart:bar:use
- chart:treemap:avoid
- quality:fidelity:use
- lever:chart-family
- operator:rank
- density:dense
---

## Wrapped bars for rank lookup <!-- role: advice -->

Choose a wrapped bar layout when readers need to judge where one item falls in a long ranked list. For example, use wrapped bars rather than a treemap when a list of roughly 75-300 items must stay on one screen and the main readout is the selected item's rank.

## Why wrapped bars work here <!-- role: reason -->

Length-encoded bars in wrapped columns keep the full list visible while preserving an ordered reading path for rank judgments. Area-coded treemap tiles stay compact, but they gave less accurate single-item ranking in this study.

**Mechanism:** Wrapped bars preserve length judgments and visible order cues for one marked item while avoiding scroll-driven interruption.

**Evidence:** In the collated results, wrapped bars had the lowest error on the single-item rank task and significantly outperformed treemaps in accuracy, while treemaps were among the faster conditions on the same task [@zengReviewCollationGraphical2023; @mylavarapuRankedListVisualizationGraphical2019].

**Notes:** The evidence comes from low-level perceptual tasks on unlabeled ranked-list charts.

## Use when all of these are true <!-- role: context -->

- **User Goal:** Find where one highlighted item sits in the full ordering.
- **Data:** A sorted ranked list with many items.
- **Chart Setting:** The full list should fit within one screen without scrolling.
- **Audience:** Readers are relying on visual marks more than text labels.
- **Success Criterion:** Lower rank-estimation error matters more than raw speed.

## Do not use when any of these are true <!-- role: exceptions -->

**Break it when:** the main success criterion is faster single-item ranking rather than more accurate ranking. **Why:** treemaps completed faster than wrapped bars on this task.

## Tradeoffs of wrapped bars here <!-- role: costs -->

**Sacrifice:** You give up some speed relative to faster compact layouts.
**Risk:** Multiple column baselines reduce horizontal resolution and can make across-column reading less direct.
**Mitigation:** Use this choice specifically for single-item rank lookup, then validate it on representative long lists.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Replacing a treemap with any compact ranked-list layout. **Why it fails:** packed bars, piled bars, and Zvinca plots were all less accurate than wrapped bars for this task.

## How to check the choice <!-- role: check -->

**Failure Sign:** Reviewers frequently misplace a highlighted item's position in the ranking.
**Quick Check:** A/B test a wrapped-bar version against a treemap version with one-item rank questions on representative long lists.
**Stronger Test:** Compare normalized absolute rank error across several list sizes and keep the lower-error option.

## What to change <!-- role: fix -->

- Replace the treemap with a wrapped bar layout.
- Split the sorted bars into columns so the whole ranked list stays visible on one screen.
- Re-test the design if speed becomes the main requirement for this task.
