---
id: use-separate-displays-instead-of-co-plotting-two-series-for-average-position-judgments
title: Use separate displays instead of co-plotting two series for average-position
  judgments
bibliography: references.bib
description: For average-position reports after a short delay, prefer multi-view layouts
  over single-view two-series displays on line or bar charts to improve fidelity and
  mitigate perceptual pull for readers judging each series separately.
labels:
- purpose:select
- basis:empirical
- structure:multi-view:use
- structure:single-view:avoid
- lever:layout-structure
- measure:multi
- group-cardinality:binary
- quality:fidelity:use
---

## Series separation for average-level recall <!-- role: advice -->

Show each data series in its own display instead of co-plotting two series when readers must judge each series' average vertical position after brief viewing. For example, separate two lines, two bar series, or a line-plus-bar pair into different displays rather than placing both series in one shared frame when viewers must reproduce one target series' average height after a short delay.

## Why separation prevents pull <!-- role: reason -->

A second series in the same display shifts the remembered average of the target series toward the non-target series. Splitting the series removes that specific cross-series pull, which otherwise exaggerates or reduces the baseline bias depending on whether the non-target series sits above or below the target.

**Mechanism:** Co-plotted series act like anchors on each other, so the irrelevant series changes where viewers remember the target series' average position to be.

**Evidence:** In compound displays with two lines, two bar series, or a line-plus-bar pair, target average-position estimates were pulled toward the irrelevant series, and the authors advise avoiding plotting two series in the same display when trying to avoid this effect [@xiongBiasedAveragePosition2020].

**Notes:** Changing one of the series from a line to bars does not remove the pull; the effect generalized across same-type and mixed-type pairs.

## When to use this choice <!-- role: context -->

- **User Goal:** Read each of two series separately and reproduce each series' average vertical position accurately.
- **Task:** View a target series briefly, then report its average level from memory.
- **Data:** Two quantitative series.
- **Chart Setting:** A design choice between one shared display and separate displays for the two series.
- **Audience:** Readers making memory-based judgments of one cued target series at a time.
- **Success Criterion:** Smaller cross-series distortion in reproduced average positions.

## When not to use this choice <!-- role: exceptions -->

**Break it when:** The display contains only one series, or the task is not a delayed average-position report for one target series. **Why:** The paper establishes perceptual pull only for two-series displays in the tested average-position task.

## What this choice costs <!-- role: costs -->

**Sacrifice:** Readers no longer see both series in one shared frame.
**Risk:** Splitting the series does not remove the baseline bias of the chosen chart family, because single lines were still underestimated and single bars were still overestimated.
**Mitigation:** After separating the series, test each display for the remaining line or bar bias.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keep both series in one display but change one series to a different mark type and expect the interference to disappear. **Why it fails:** Line-plus-bar displays still showed perceptual pull, not a clean escape from it.

## How to test the choice <!-- role: check -->

**Failure Sign:** Estimates for a target series shift toward the other series when both appear in the same display.
**Quick Check:** Compare a shared two-series display against a version where each series is shown in its own display, using brief viewing, a short delay, and average-position reproduction.
**Stronger Test:** Run the comparison for each pairing you might use, including two lines, two bar series, and a line-plus-bar pair.

## How to fix a failing chart <!-- role: fix -->

- Remove the non-target series from the display used for the average-position readout.
- Put each of the two series in its own display instead of co-plotting both in one frame.
- Do not use a line-plus-bar combination as a workaround for a two-line or two-bar shared display.
