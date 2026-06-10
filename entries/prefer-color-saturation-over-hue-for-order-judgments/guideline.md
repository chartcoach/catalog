---
id: prefer-color-saturation-over-hue-for-order-judgments
title: Prefer color saturation over hue for order judgments
bibliography: references.bib
description: For order judgments, prefer color-saturation over hue on quantitative
  marks in ordered one-dimensional sequences to improve fidelity and mitigate missed
  ordered patterns for viewers scanning static displays.
labels:
- purpose:refine
- basis:empirical
- task:relate
- quality:fidelity:use
- lever:encoding
- reading-mode:overview
- channel:color-saturation:use
- channel:color-hue:avoid
---

## Change the color encoding <!-- role: advice -->

Encode quantitative order with a saturation ramp instead of a hue ramp when readers must judge whether a sequence is ordered. For example, in a left-to-right row of marks with fixed x-position, map increasing values to stronger light-to-dark saturation rather than to a red-to-blue hue progression.

## Why saturation works better here <!-- role: reason -->

Orderedness judgments depend on whether the encoding itself looks monotonic. Saturation gives readers a clearer visual progression than hue, so moderately disordered sequences are less likely to be misread.

**Mechanism:** A saturation ramp preserves a stronger sense of increasing or decreasing magnitude, which supports more accurate judgments about whether the whole sequence forms an ordered pattern.

**Evidence:** In the collated result for the order-judgment task, color saturation ranked first in accuracy and hue ranked last, with significant pairwise differences favoring saturation over hue; the original experiment also reports that hue makes sequences appear less ordered than more orderable channels, especially away from the clearly ordered and clearly unordered extremes [@zengReviewCollationGraphical2023; @chungHowOrderedIt2016].

## Use when order detection is the job <!-- role: context -->

- **User Goal:** Decide whether a sequence shows an ordered pattern.
- **Task:** Judge overall orderedness rather than read exact values.
- **Data:** One quantitative value per mark, with left-to-right position already fixed.
- **Chart Setting:** A static single-view sequence or 1D plot where the non-positional encoding carries the magnitude.
- **Success Criterion:** More accurate ordered versus unordered judgments.

## Do not rely on this contrast at the extremes <!-- role: exceptions -->

**Break it when:** The sequence is already obviously ordered or obviously unordered. **Why:** The study found that different encodings produced nearly the same judgments at those extreme disorder levels.

## Account for the speed tradeoff <!-- role: costs -->

**Sacrifice:** A saturation ramp was not the fastest tested encoding for order judgments.\
**Risk:** If you optimize only for response time, you may miss faster alternatives from the tested set.\
**Mitigation:** Use saturation when correct order detection matters more than shaving off scan time.

## Watch for the hue failure mode <!-- role: mistakes -->

**Mistake:** Keep a hue ramp on quantitative marks when the task is to judge whether the sequence is ordered. **Why it fails:** Hue produced the weakest order-judgment accuracy in the tested set and made orderedness harder to read.

## Test the same sequence both ways <!-- role: check -->

**Failure Sign:** Reviewers disagree about whether moderately noisy sequences look ordered.\
**Quick Check:** Render the same sequence once with saturation and once with hue, and ask readers to rate orderedness.\
**Stronger Test:** Compare accuracy on moderately disordered sequences, where the study observed the clearest encoding differences.

## Make the encoding swap <!-- role: fix -->

- Replace the hue ramp with a monotonic saturation ramp.
- Keep x-position fixed and let saturation carry the quantitative order.
- Re-test the revised view on moderately ordered sequences instead of only on perfectly ordered examples.
