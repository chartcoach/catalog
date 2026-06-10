---
id: use-color-rather-than-shape-for-group-mean-comparisons-in-scatterplots
title: Use color rather than shape to distinguish groups for mean comparisons in scatterplots
bibliography: references.bib
description: For mean-comparison tasks, prefer color grouping on scatterplots to improve
  fidelity and mitigate less accurate group mean judgments for viewers comparing the
  average positions of two point sets.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:scatter
- quality:fidelity:use
- lever:encoding
- channel:color-hue:use
- channel:shape:avoid
---

## Put the group split on color <!-- role: advice -->

Use color rather than shape to distinguish groups when a scatterplot must support comparison of group mean position. For example, encode the two point sets with different hues instead of circles versus triangles when readers need to judge which group sits higher on average.

## Why color helps mean comparison in scatterplots <!-- role: reason -->

Mean comparison in a scatterplot depends on quickly separating the groups and then summarizing each cloud’s position. Color provides a cleaner group split for this task than shape, which supports more accurate judgments of average group position.

**Mechanism:** Color makes the groups easier to separate before the viewer estimates each group’s mean position.

**Evidence:** The review collates this paper as covering aggregate and correlate tasks on scatterplot-like designs. In its summary-task discussion, the paper reports that using color to distinguish two groups in a scatterplot led to higher accuracy in mean judgments than using shape [@zengReviewCollationGraphical2023; @szafirFourTypesEnsemble2016].

## Use when the scatterplot’s job is comparing group averages <!-- role: context -->

- **User Goal:** Decide which group has the higher or lower average position.
- **Task:** Mean comparison between two point sets.
- **Data:** Two groups displayed together in one scatterplot.
- **Chart Setting:** A scatterplot where group membership could be encoded by color or by shape.
- **Success Criterion:** More accurate judgments of which group mean is higher or lower.

## Do not generalize this beyond the reported task <!-- role: exceptions -->

**Break it when:** The chart is not being used for mean-position comparison in a scatterplot. **Why:** The reported advantage is specific to that task and display context.

## Tradeoffs of color-first group encoding <!-- role: costs -->

**Sacrifice:** You give up a shape-first grouping scheme for the mean-comparison task.
**Risk:** Keeping shape as the main group cue can lower mean-comparison accuracy relative to color.
**Mitigation:** Keep group membership on color when average-position comparison is the main job.

## Common failure with group encoding in scatterplots <!-- role: mistakes -->

**Mistake:** Using shape as the main group cue and expecting the same mean-comparison accuracy as color. **Why it fails:** The paper reports lower accuracy for mean judgments under shape-based grouping.

## Check whether the group cue supports the mean judgment <!-- role: check -->

**Failure Sign:** Reviewers disagree about which group has the higher average position.
**Quick Check:** Compare a color-coded and a shape-coded version of the same scatterplot.
**Stronger Test:** Ask reviewers which group mean is higher in both versions and compare agreement.

## Fix the group encoding <!-- role: fix -->

- Remap group membership from shape to color when the scatterplot’s job is mean comparison.
- Keep the mean-comparison groups separated by hue rather than by shape.
