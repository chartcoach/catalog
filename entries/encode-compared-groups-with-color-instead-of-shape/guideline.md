---
id: encode-compared-groups-with-color-instead-of-shape
title: Encode compared groups with color instead of shape
bibliography: references.bib
description: For grouped comparison tasks with multiclass scatterplots, prefer color
  encoding on class membership to improve fidelity and mitigate mean-position judgment
  errors for viewers comparing which group is on average higher.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:scatter
- lever:encoding
- channel:color-hue:use
- channel:shape:avoid
- quality:fidelity
---

## Prefer color for class grouping <!-- role: advice -->

Encode class membership with color instead of shape when readers must judge which point group is on average higher. For example, use hue or luminance on point marks rather than circle-versus-triangle grouping for multiclass scatterplots used to compare class averages.

## Why color grouping works better here <!-- role: reason -->

A stronger grouping cue makes it easier to isolate one class and judge its average position against another. When the task is to decide which class is on average higher, color-based grouping yields more accurate aggregate judgments than shape-only grouping.

**Mechanism:** Color makes the compared classes easier to separate visually, so readers can form and compare class averages with fewer errors.

**Evidence:** In the collated result, hue- and luminance-based scatterplots formed the higher-accuracy group, and both shape-only variants formed the lower-accuracy group for aggregate mean judgments; the source paper reports a significant main effect where color/luminance conditions outperformed shape conditions [@zengReviewCollationGraphical2023; @gleicherPerceptionAverageValue2013].

**Notes:** Shape-only scatterplots still supported above-chance performance, so this is an accuracy preference rather than a blanket ban on shape.

## Use when mean comparison is the chart's job <!-- role: context -->

- **User Goal:** Decide which class is on average higher.
- **Task:** Compare class averages rather than inspect individual points.
- **Data:** Two or more classes are shown in one scatterplot.
- **Chart Setting:** Static point scatterplot; readers can inspect the view for several seconds.
- **Success Criterion:** More accurate judgments of which class has the higher average position.

## Do not generalize beyond this task <!-- role: exceptions -->

**Break it when:** The chart is not being used to compare class averages in a scatterplot. **Why:** The evidence only covers aggregate judgments of which class is on average higher in multiclass scatterplots.

## What this preference does not claim <!-- role: costs -->

**Sacrifice:** Shape-only grouping can still work, so the change optimizes accuracy rather than unlocking a previously impossible task.\
**Risk:** Treating this as a rule for every scatterplot task overstates the evidence.\
**Mitigation:** Apply it specifically when average-position comparison accuracy matters.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Use shape as the sole class cue when the chart asks readers to decide which group is on average higher. **Why it fails:** Shape-coded conditions were less accurate than color- or luminance-coded conditions for this task.

## How to review the choice <!-- role: check -->

**Failure Sign:** Reviewers hesitate or disagree when asked which class is on average higher in a shape-coded version.\
**Quick Check:** Build a matched color-coded version with the same point positions and compare answers on several close-mean cases.\
**Stronger Test:** Run a short forced-choice review using the same scatterplots in shape-only and color-coded forms, and keep the version with fewer mean-judgment errors.

## What to change <!-- role: fix -->

- Replace shape-only class grouping with hue or luminance on the point marks.
- Keep the point positions unchanged so the grouping cue is the only substantive change.
- Re-test the revised scatterplot on close average separations before finalizing it.
