---
id: avoid-slope-encodings-for-pairwise-relation-judgments
title: Avoid slope encodings for pairwise relation judgments
bibliography: references.bib
description: For compare tasks on grouped paired quantitative displays, avoid slope
  encoding on paired-value charts to improve fidelity and mitigate slow and inaccurate
  relation judgments for viewers.
labels:
- purpose:refine
- basis:empirical
- task:compare
- scope:grouped-result
- data:quantitative
- quality:fidelity:use
- lever:encoding
- channel:orientation:avoid
---

## Replace slope as the relation carrier <!-- role: advice -->

Avoid slope when the display must support relation-direction judgments across many paired values. For example, remap the same paired relation from slope to position-based marks or bar-length marks when readers must search for one opposite relation or decide which relation direction is more prevalent.

## Why avoiding slope helps these judgments <!-- role: reason -->

In these tasks, slope made the relation harder to judge than the other tested channels. Readers were slower or less accurate when the paired relation was carried by slope.

**Mechanism:** When the same paired relation is mapped to position or length instead of slope, the relation is easier to distinguish across many pairs.

**Evidence:** In the collated record, slope-based variants ranked below position-based and length-based variants for target-relation search time and for prevalence judgments; the original study reports significantly worse performance for slope encodings than for position and length on these relation-direction tasks [@zengReviewCollationGraphical2023; @nothelferMeasuresBenefitDirect2020].

**Notes:** The source limits this finding to the studied displays and tasks.

## Use when slope is carrying the pairwise comparison <!-- role: context -->

- **User Goal:** Judge which paired relation is present or dominant.
- **Task:** Search for a target relation or decide which relation direction is more prevalent.
- **Data:** Paired quantitative values shown repeatedly across many categories or items.
- **Chart Setting:** The display currently uses slope to carry the pairwise relation and can be redrawn with the same relation mapped to position or length.
- **Success Criterion:** Faster relation search or higher accuracy for direction judgments.

## Do not generalize beyond the studied task setting <!-- role: exceptions -->

**Break it when:** The display is not being used for the studied relation-direction judgments across many paired quantitative marks. **Why:** This evidence only establishes the slope penalty for the tested search and prevalence tasks in this display setting.

## Costs of avoiding slope in these views <!-- role: costs -->

**Sacrifice:** You give up using slope as the main carrier of the pairwise relation.
**Risk:** Keeping slope can slow target-relation search and reduce accuracy for majority-direction judgments.
**Mitigation:** Remap the same signed relation to position or length while keeping the pairing structure unchanged.

## Common failure mode with slope encodings <!-- role: mistakes -->

**Mistake:** Keeping paired slope marks for displays whose main question is which relation direction appears or dominates. **Why it fails:** The studied tasks were slower or less accurate with slope than with position or length.

## Check whether slope is hurting relation judgments <!-- role: check -->

**Failure Sign:** Relation-direction questions are slow or error-prone in a slope-based paired display.
**Quick Check:** Redraw the same display with the relation mapped to position or length and compare one target-relation judgment and one majority-direction judgment.
**Stronger Test:** Time both versions or compare accuracy; keep the non-slope version if it performs better.

## Fix the encoding channel <!-- role: fix -->

- Remap the paired relation from slope to position.
- Or remap the same paired relation to bar length.
- Keep the baseline and category positions constant so the encoding channel is the main change under review.
- Reserve slope only for cases outside these studied pairwise relation-judgment tasks.
