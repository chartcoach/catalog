---
id: remove-a-conflicting-shape-cue-when-a-third-class-is-present
title: Remove a conflicting shape cue when a third class is present
bibliography: references.bib
description: For grouped comparison tasks with multiclass scatterplots, avoid conflicting
  shape encoding on point marks when an extra class is also present to prevent accuracy
  loss and mitigate compounded visual complexity for viewers comparing which group
  is on average higher.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:scatter
- lever:encoding
- group-cardinality:few
- channel:shape:avoid
- quality:fidelity
---

## Simplify the compared classes when a distractor class is already in view <!-- role: advice -->

Remove a conflicting secondary shape cue when a scatterplot already includes a third class and readers must compare two class averages. For example, keep a color-coded scatterplot with a distractor class free of extra circle-versus-triangle mixing on the compared classes.

## Why the combined complication hurt accuracy <!-- role: reason -->

One added complication alone was tolerated, but the combination of a distractor class and a conflicting cue reduced accuracy. The compounded display complexity made the average-position comparison harder than a simpler color-coded baseline.

**Mechanism:** A third class plus a conflicting secondary cue creates enough extra visual complexity to interfere with separating the compared groups and judging their average positions accurately.

**Evidence:** The collated result records a significant accuracy drop for the scatterplot that combined a distractor class with a conflicting shape cue relative to the simpler color-only baseline, while the source paper reports that neither an added distractor class alone nor a conflicting cue alone produced a significant drop, but the combination did [@zengReviewCollationGraphical2023; @gleicherPerceptionAverageValue2013].

**Notes:** The source did not find significant harm from only one of these two complications by itself.

## Use when both sources of complexity are present <!-- role: context -->

- **User Goal:** Decide which of two classes is on average higher.
- **Task:** Compare class averages in one view.
- **Data:** A third class is visible in the same scatterplot as a distractor.
- **Chart Setting:** The compared classes also carry a secondary shape cue that conflicts with the primary class encoding.
- **Success Criterion:** Preserve accuracy of average-position judgments.

## Do not simplify when only one complication is present <!-- role: exceptions -->

**Break it when:** The scatterplot has only a third class or only a conflicting shape cue, but not both together. **Why:** The source did not find a significant accuracy drop from either one alone.

## What this simplification costs <!-- role: costs -->

**Sacrifice:** You lose a secondary shape distinction on the compared classes.\
**Risk:** Removing more than one complexity source may oversimplify beyond what the evidence requires.\
**Mitigation:** Drop the conflicting shape cue first and re-test before removing the extra class.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keep a conflicting shape pattern on the compared classes after adding a third distractor class. **Why it fails:** The combined condition was less accurate than the simpler color-coded baseline for mean comparison.

## How to review the choice <!-- role: check -->

**Failure Sign:** Reviewers make more mistakes on the version that has both a third class and mixed shapes on the compared classes.\
**Quick Check:** Compare the current chart against a version that keeps the third class but removes the conflicting shape cue.\
**Stronger Test:** Run a short forced-choice review on close-mean cases using the simple baseline and the combined-complexity version, then keep the version with fewer mean-comparison errors.

## What to change <!-- role: fix -->

- Remove the conflicting shape cue from the compared classes.
- If the conflicting shape cue must stay, remove the extra distractor class from the comparison view.
- Return the compared classes to a single primary grouping cue before re-testing the scatterplot.
