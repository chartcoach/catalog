---
id: use-parallel-coordinates-instead-of-scatter-for-cluster-identification
title: Use a parallel coordinates plot instead of a scatter plot for cluster identification
bibliography: references.bib
description: For cluster-identification tasks on sparse multivariate quantitative
  data, prefer a parallel coordinates plot over a scatter plot to improve fidelity
  and mitigate missed group structure in static views.
labels:
- purpose:select
- basis:empirical
- chart:parallel:use
- chart:scatter:avoid
- data:quantitative
- quality:fidelity:use
- lever:chart-family
- measure:multi
- density:sparse
---

## Choose the clustering view <!-- role: advice -->

Use a parallel coordinates plot when the job is to identify a cluster in multivariate quantitative data. For example, replace a scatter plot view with a parallel coordinates plot when readers must choose the subset of records that forms a cluster in a 4-attribute, 8-record display.

## Why parallel coordinates help clustering <!-- role: reason -->

A parallel coordinates plot lets readers judge similarity across all shown variables as one line pattern, while a scatter plot view requires balancing separate pairwise patterns.

**Mechanism:** Parallel coordinates put each record into one polyline across shared axes. This makes multivariate similarity easier to inspect than splitting the same records across scatter plots.

**Evidence:** The collated record ranks the parallel coordinates plot above the scatter plot on clustering accuracy, and the original experiment concluded that parallel coordinates plots outperformed scatter plots for clustering in the studied multivariate setup [@zengReviewCollationGraphical2023; @kanjanaboseMultitaskComparativeStudy2015].

**Notes:** The supported advantage over the scatter plot is strongest on accuracy.

## Use when multivariate grouping is the job <!-- role: context -->

- **User Goal:** Choose the subset of records that forms a cluster.
- **Data:** 8 records with 4 quantitative attributes.
- **Chart Setting:** Static representations of the same records and attributes with no interaction.
- **Success Criterion:** More correct cluster choices.

## Do not use this choice for exact lookup <!-- role: exceptions -->

**Break it when:** The user goal is exact value retrieval rather than cluster identification. **Why:** In the same study, the table was faster for value lookup, and the visual representations did not show an accuracy advantage there.

## Tradeoffs of replacing a scatter plot with parallel coordinates <!-- role: costs -->

**Sacrifice:** You should not expect a large speed gain from the switch alone.
**Risk:** Changing to parallel coordinates only to save time may disappoint.
**Mitigation:** Use this change when cluster-identification accuracy matters most.

## Common clustering failure <!-- role: mistakes -->

**Mistake:** Keeping a scatter plot view when cluster-identification accuracy is the main success criterion. **Why it fails:** The scatter plot view was less accurate than the parallel coordinates plot in the studied setup.

## Check the clustering choice <!-- role: check -->

**Failure Sign:** Reviewers choose the wrong subset of records even after inspecting the scatter plot view.
**Quick Check:** Show the same clustering prompt in a scatter plot view and in a parallel coordinates plot, and compare which version gets the correct subset more often.
**Stronger Test:** Repeat matched clustering prompts and compare accuracy first, then completion time.

## Fix the clustering view <!-- role: fix -->

- Replace the scatter plot view with a parallel coordinates plot for clustering tasks.
- Show each record as one polyline across shared attribute axes instead of splitting the same records across scatter plots.
- Switch back to a table only when the task changes to exact value retrieval.
