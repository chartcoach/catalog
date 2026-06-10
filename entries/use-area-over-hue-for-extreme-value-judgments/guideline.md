---
id: use-area-over-hue-for-extreme-value-judgments
title: Use area over hue for extreme-value judgments
bibliography: references.bib
description: For extreme-value judgments, use area instead of hue on quantitative
  marks in ordered one-dimensional sequences to improve fidelity and mitigate missed
  smallest-or-largest values for viewers scanning static displays.
labels:
- purpose:refine
- basis:empirical
- task:extreme
- quality:fidelity:use
- lever:encoding
- reading-mode:lookup
- channel:area:use
- channel:color-hue:avoid
---

## Resize the marks <!-- role: advice -->

Encode quantitative magnitude with area when readers must decide which item is the smallest or largest in a sequence. For example, size circles by value instead of coloring equal-sized marks with a hue ramp when a reader must classify an item as minimum, maximum, or neither.

## Why area helps with extremes <!-- role: reason -->

Extreme-value judgments depend on how directly readers can compare relative magnitude across marks. Area gives a stronger cue for smallest-versus-largest decisions than hue in this ordered-sequence setting.

**Mechanism:** Larger and smaller mark areas make the magnitude ranking of items easier to inspect, which improves minimum and maximum identification.

**Evidence:** In the collated result for the extreme-value task, area ranked first in accuracy and hue ranked last, with significant pairwise differences favoring area over hue and over every other tested encoding; the original experiment likewise reports that size produced fewer min/max errors while hue was error-prone for this task [@zengReviewCollationGraphical2023; @chungHowOrderedIt2016].

## Use when readers must find the extreme <!-- role: context -->

- **User Goal:** Identify the minimum or maximum item in a sequence.
- **Task:** Compare one candidate against the rest or scan the sequence for the extreme.
- **Data:** One quantitative value per mark, with left-to-right position already fixed.
- **Chart Setting:** A static single-view sequence or 1D plot where magnitude is carried by a non-positional encoding.
- **Success Criterion:** Fewer wrong smallest/largest judgments.

## Do not generalize this to order judgment <!-- role: exceptions -->

**Break it when:** The goal is to judge how ordered the whole sequence is rather than to find the smallest or largest value. **Why:** Area led the accuracy ranking for extreme-value judgments, but it did not lead the order-judgment ranking.

## Accept the speed tradeoff <!-- role: costs -->

**Sacrifice:** Area was not the fastest tested encoding for the extreme-value task.\
**Risk:** Using area only to speed up scanning can disappoint even when it improves correctness.\
**Mitigation:** Choose area when correct min/max identification matters more than raw response time.

## Avoid the hue fallback <!-- role: mistakes -->

**Mistake:** Use a hue ramp to encode quantitative magnitude when readers must find the smallest or largest value. **Why it fails:** Hue had the lowest accuracy for the extreme-value task.

## Compare min/max accuracy directly <!-- role: check -->

**Failure Sign:** Readers misclassify likely candidates as not the smallest or largest.\
**Quick Check:** Render the same sequence once with area and once with hue, and count wrong minimum/maximum calls.\
**Stronger Test:** Time and score the task while asking readers to label a candidate as smallest, largest, or neither.

## Replace color with size <!-- role: fix -->

- Resize the marks so larger values take larger area.
- Remove the hue ramp from equal-sized marks and let area carry the quantity.
- Keep the left-to-right position constant so readers compare magnitude through area rather than through color.
