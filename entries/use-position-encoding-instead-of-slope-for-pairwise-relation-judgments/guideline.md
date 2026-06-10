---
id: use-position-encoding-instead-of-slope-for-pairwise-relation-judgments
title: Use position encoding instead of slope encoding for pairwise relation judgments
bibliography: references.bib
description: For pairwise relation judgments over many quantitative pairs, use position
  encoding on row-aligned comparison charts to improve fidelity and mitigate slow,
  low-accuracy reading from slope encoding for viewers making quick scans.
labels:
- purpose:refine
- basis:empirical
- task:relate
- data:quantitative
- quality:fidelity:use
- lever:encoding
- channel:position:use
- channel:orientation:avoid
---

## Replace slope with position <!-- role: advice -->

Encode the value or delta by position from a common baseline instead of by slope when viewers must judge relations across many pairs. For example, replace a row of angled line segments with baseline-aligned dashes for individual values or with a single delta-position mark when readers must find the opposite relation or judge which direction is more prevalent.

## Why position outperforms slope in these relation tasks <!-- role: reason -->

Row-aligned slopes make viewers parse mirrored configurations rather than a simpler positional readout. Position encoding reduces that bottleneck when viewers scan many pairwise relations.

**Mechanism:** Position encoding lets readers compare distance from a baseline directly, while slope encoding requires interpreting angled segments that can group visually into mirrored shapes in a row.

**Evidence:** In the visual search task and the proportion-judgment task, slope encodings produced significantly worse performance than position encodings. The paper also notes that the row arrangement used here may make slopes appear as grouped `/\` and `\/` shapes, which likely contributes to the poorer relation reading [@nothelferMeasuresBenefitDirect2020].

**Notes:** The source presents this result for the specific displays and tasks tested, not as a universal ranking for all possible slope layouts.

## Use when slopes are arranged in rows for relation reading <!-- role: context -->

- **User Goal:** Find which pair has a target increase or decrease pattern, or decide which relation direction appears more often.
- **Task:** Scan many pairwise relations quickly rather than inspect one pair in isolation.
- **Data:** Quantitative values organized into pairs with directional differences.
- **Chart Setting:** The current design uses row-aligned slope marks or is considering slope as the main encoding for value or delta.
- **Audience:** Viewers making quick scans or brief-glance judgments.
- **Success Criterion:** Faster relation search and higher accuracy than a slope-encoded version.

## Do not generalize beyond the tested row-based setting <!-- role: exceptions -->

**Break it when:** The task is not pairwise relation perception, or the slope display is organized differently from the row-based arrangement tested here. **Why:** The source limits this finding to the tested tasks and explicitly suggests that the row arrangement may be part of why slope performed poorly.

## Tradeoffs of replacing slope with position <!-- role: costs -->

**Sacrifice:** You give up a slope-based visual form.\
**Risk:** Changing slope to position alone does not remove the larger cost of inferring relations from two separate values.\
**Mitigation:** When relation perception is central, combine position encoding with direct delta encoding.

## Common failure mode for row-aligned slope displays <!-- role: mistakes -->

**Mistake:** Using a row of angled line segments for increase-decrease judgments and expecting fast search or reliable majority judgments. **Why it fails:** In the tested row layout, slope marks were harder to parse than position marks.

## Compare the slope version to a position version <!-- role: check -->

**Failure Sign:** Reviewers hesitate or disagree when asked where the lone opposite relation is or which direction appears more often in a row of slopes.\
**Quick Check:** Redraw the same pairs with baseline-aligned positions and compare performance on the same question.\
**Stronger Test:** Run a brief search or majority-direction task on both versions and keep the version that yields faster or more accurate judgments.

## Re-encode the rows with a baseline position readout <!-- role: fix -->

- Replace row-aligned slope marks with marks whose value is encoded by position from a common baseline.
- If the chart must preserve both values in each pair, show the two values as separate baseline-aligned positions rather than as angled segments.
- If the chart can abstract the comparison, show the pairwise difference as a single delta-position mark instead of a slope.
