---
id: do-not-add-redundant-class-encodings-just-to-improve-mean-comparison-accuracy
title: Do not add redundant class encodings just to improve mean-comparison accuracy
bibliography: references.bib
description: For grouped comparison tasks with multiclass scatterplots, avoid adding
  redundant class encodings on point marks to prevent unnecessary encoding changes
  and mitigate unsupported attempts to improve fidelity for viewers comparing which
  group is on average higher.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:scatter
- lever:encoding
- quality:fidelity
---

## Keep one primary class cue <!-- role: advice -->

Keep a single clear class encoding when the job is to judge which group is on average higher. For example, do not add matching shapes to a color-coded scatterplot, or matching colors to a shape-coded scatterplot, if the only goal is to improve class-mean comparison accuracy.

## Why redundant cues did not help <!-- role: reason -->

A second matching class cue did not make aggregate mean judgments more accurate once one cue already identified the groups. Readers could already perform the task without a measurable gain from duplicated class encoding.

**Mechanism:** Once one feature is sufficient to separate the classes, duplicating the same grouping in another feature does not improve the average-position readout.

**Evidence:** The collated result records no significant accuracy gain from redundant class encoding, and the source paper's within-subject comparisons found no significant improvement when color was paired with matching shape or when shape was paired with matching color for aggregate mean judgments [@zengReviewCollationGraphical2023; @gleicherPerceptionAverageValue2013].

**Notes:** The source found no significant benefit from redundancy, not a significant penalty.

## Use when a scatterplot already has a clear grouping cue <!-- role: context -->

- **User Goal:** Decide which class is on average higher.
- **Task:** Compare class averages rather than inspect individual points.
- **Data:** Class membership is already encoded by one visible cue.
- **Chart Setting:** Static multiclass scatterplot with point marks that could carry both color and shape.
- **Success Criterion:** Higher mean-comparison accuracy, not just more differentiated styling.

## Do not treat this as a rule about every design goal <!-- role: exceptions -->

**Break it when:** Your goal is something other than improving aggregate mean-comparison accuracy. **Why:** The evidence only tests whether redundancy improves this specific scatterplot task, and it did not.

## What you give up by removing redundancy <!-- role: costs -->

**Sacrifice:** You give up a duplicated class cue.\
**Risk:** Keeping the duplicated cue as an accuracy intervention adds a design change with no measured gain on this task.\
**Mitigation:** Keep one primary cue for the mean-comparison view, and add redundancy only after separate testing for your actual goal.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Add a second matching class cue solely because it seems like it should help readers compare class averages. **Why it fails:** Redundant color-plus-shape versions were not significantly more accurate than single-cue versions.

## How to review the choice <!-- role: check -->

**Failure Sign:** A redundant version looks busier, but reviewers are not more accurate when asked which class is on average higher.\
**Quick Check:** Compare a single-cue and a redundant-cue version with the same point positions on several close-mean cases.\
**Stronger Test:** Use a short forced-choice comparison and keep the simpler version unless the redundant version shows a clear accuracy gain.

## What to change <!-- role: fix -->

- Remove the redundant shape or color cue if it was added only to improve mean-comparison accuracy.
- Keep one primary class cue constant across the whole scatterplot.
- If redundancy must remain for another reason, stop treating it as an accuracy optimization for this task.
