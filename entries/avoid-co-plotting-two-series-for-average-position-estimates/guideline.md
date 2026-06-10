---
id: avoid-co-plotting-two-series-for-average-position-estimates
title: Avoid plotting two series in the same display for average-position estimates
bibliography: references.bib
description: For short-delay average-position judgments, avoid multi-series layout
  structure on quantitative line and bar displays to prevent perceptual pull and mitigate
  biased average-position estimates for readers estimating averages from memory.
labels:
- purpose:refine
- basis:empirical
- data:quantitative
- quality:fidelity
- lever:layout-structure
- channel:position
- measure:multi
- group-cardinality:binary
---

## Series arrangement for average-position judgments <!-- role: advice -->

Keep the target series in its own display when readers must estimate its average position from memory. For example, avoid line-plus-line, bar-plus-bar, and line-plus-bar compound displays for this task, because any second series can pull the target estimate toward itself.

## Why separation matters here <!-- role: reason -->

A second series becomes a competing positional reference. The remembered average of the target shifts toward that other series, which can either exaggerate or reduce the baseline underestimation of lines and overestimation of bars depending on whether the added series sits above or below.

**Mechanism:** Removing the second series prevents perceptual pull, so the target average is not dragged toward an irrelevant positional anchor in the same frame.

**Evidence:** In the multi-series experiments, adding a second line, a second set of bars, or a mixed line-bar pair changed target average estimates in the direction of the other series; the pull strength did not depend on whether the non-target series was a line or bars [@xiongBiasedAveragePosition2020; @zengReviewCollationGraphical2023].

## Use when all of these are true <!-- role: context -->

- **User Goal:** Judge the average position of one target series accurately.
- **Task:** Recall the target average after a brief view and short delay.
- **Data:** Two quantitative series in the same frame, with one series relevant and the other irrelevant to the judgment.
- **Chart Setting:** Compound line-plus-line, bar-plus-bar, or line-plus-bar displays.
- **Audience:** Readers making target-series average judgments from memory.
- **Success Criterion:** The target estimate stays stable when another series is present.

## Do not use when any of these are true <!-- role: exceptions -->

- **Break it when:** the display contains only one graphed series. **Why:** perceptual pull requires a second series, although single-series line and bar biases can still remain.
- **Break it when:** the task is not recalling a series average after a brief view and short delay. **Why:** the evidence does not test every other reading task or viewing condition.

## Costs of separating the series <!-- role: costs -->

**Sacrifice:** Removing the second series addresses pull from the competing series, not the baseline bias of the remaining line or bars.
**Risk:** If applied blindly, you may assume the single-series display is unbiased.
**Mitigation:** After removing the second series, still test whether the remaining line or bars are under- or overestimated for the target task.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Assuming perceptual pull only occurs when both series use the same mark type. **Why it fails:** line-plus-line, bar-plus-bar, and mixed line-plus-bar displays all produced pull.

## How to test for perceptual pull <!-- role: check -->

**Failure Sign:** The target average shifts upward or downward when a second series is added to the same frame.
**Quick Check:** Compare readers’ average-position estimates for a target shown alone versus with a second series above or below it; if the estimate moves toward the added series, pull is present.
**Stronger Test:** Test both same-type and mixed-type pairings, because any second series can act as the pulling reference.

## What to change <!-- role: fix -->

- Remove the non-target series from the display when the job is to estimate one series average.
- Show the target series alone and re-test the average-position judgment.
- If the paired display must remain, do not rely on that shared display for recalled average-position estimates.
