---
id: animate-the-transition-between-paired-series-for-biggest-delta-comparison
title: Animate the transition between paired series for biggest-delta comparison
bibliography: references.bib
description: For item-to-item comparison of change between two matched series during
  brief inspection, use an animated transition in a single chart to improve fidelity
  and mitigate missed large changes for rapid visual judgments.
labels:
- purpose:refine
- basis:empirical
- task:compare
- quality:fidelity:use
- lever:interaction-access
- operator:difference
- temporal-pattern:dynamic
---

## Animated transition <!-- role: advice -->

Animate the transition between the two matched series when readers must find the item that changed the most. For example, use one chart that morphs from the first series to the second and avoid relying on separated static views for this task.

## Why animation works for largest-change judgments <!-- role: reason -->

Biggest-delta judgments benefit from a cue that makes the largest changing item stand out immediately. Animation turns change into motion, so the item with the largest data change also carries the strongest motion cue.

**Mechanism:** Motion creates a salient local signal that naturally maps to item-level change and pulls attention toward the biggest mover.

**Evidence:** The paper reports earlier comparison results showing that animation provided the most precise performance for biggest-delta comparisons, outperforming separated static arrangements for this task [@jardinePerceptualProxiesVisual2020].

**Notes:** The same paper also notes that animation did not perform as well for correlation comparisons.

## Use when matched items change between two states <!-- role: context -->

- **User Goal:** Find which item changed the most between two matched series.
- **Task:** Item-to-item comparison of change.
- **Data:** Two aligned states of the same set of items.
- **Chart Setting:** A chart can be shown as one state transitioning into the other instead of as two separated static views.
- **Audience:** Readers making a brief visual judgment.
- **Success Criterion:** The largest changer stands out quickly and precisely.

## Do not use when the task is a whole-set summary comparison <!-- role: exceptions -->

**Break it when:** The reader must compare whole-set summaries such as which series has the larger mean or wider range. **Why:** The paper reports that vertically stacked separated charts were more precise than animation or superposition for those set-level comparisons.

## What you trade away with animation <!-- role: costs -->

**Sacrifice:** You give up a purely static presentation.
**Risk:** If applied blindly to other comparison tasks, animation can underperform layouts that better support those tasks.
**Mitigation:** Use animation only when the task is to spot the biggest individual change.

## Common task-layout mismatch <!-- role: mistakes -->

**Mistake:** Reuse the animated transition for strongest-correlation or mean/range judgments. **Why it fails:** The paper reports different arrangements were better for those tasks than animation.

## Test animation against a static alternative <!-- role: check -->

**Failure Sign:** Reviewers cannot quickly point to the biggest changer.
**Quick Check:** Compare an animated version against a separated static version on the same data and ask for a brief biggest-delta decision.
**Stronger Test:** Run repeated timed trials and compare correctness for the biggest-delta task across the animated and static versions.

## Turn the change task into a transition view <!-- role: fix -->

- Replace two separated static views with one chart that transitions from the first series to the second.
- Keep the comparison anchored on matched items across the two states.
- Remove the animated transition if the task changes to mean, range, or correlation comparison.
