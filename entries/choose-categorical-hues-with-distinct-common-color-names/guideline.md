---
id: choose-categorical-hues-with-distinct-common-color-names
title: Choose categorical hues with distinct common color names
bibliography: references.bib
description: For aggregate color comparisons, prefer hue categories with distinct
  common color names on nominal color encodings to improve fidelity and address confusion
  between neighboring named hues for readers identifying categories by color.
labels:
- purpose:refine
- basis:empirical
- data:categorical
- quality:fidelity:use
- lever:encoding
- channel:color-hue:use
- aesthetic:color:use
---

## Separate hue categories by common names <!-- role: advice -->

Choose categorical hues that differ clearly in the everyday names people are likely to use for them. For example, replace ambiguous intermediate hues that may be called by overlapping names with hues whose common names separate more cleanly, and inspect the most confusable pair first.

## Why distinct color names help <!-- role: reason -->

People do not rely only on perceptual distance when they identify category colors. If two hues are likely to be called by the same or neighboring names, readers can confuse them even when the colors are not especially close in color space.

**Mechanism:** Larger name difference makes category colors easier to identify and refer to, which improves discrimination when readers must track or compare categories by hue.

**Evidence:** The collated review associates this paper with nominal color-hue guidance. In the paper, Name Difference was a strong predictor of discrimination behavior and was reported as potentially more useful than Perceptual Distance for predicting discriminability; the paper also gives the concrete risk that an intermediate hue can be perceptually distinct yet still be called by the same neighboring names as other colors. [@zengReviewCollationGraphical2023; @gramazioColorgoricalCreatingDiscriminable2017]

## Use when all of these are true <!-- role: context -->

- **User Goal:** Help readers quickly identify and compare nominal categories by color.
- **Task:** Make aggregate or target-color judgments without category-name confusion.
- **Data:** Categories are encoded only by hue.
- **Chart Setting:** The palette will be referenced through a legend, labels, or verbal color names.
- **Audience:** Readers may identify colors using everyday color names.
- **Success Criterion:** Lower confusion between category colors and fewer discrimination errors.

## Do not use when any of these are true <!-- role: exceptions -->

**Break it when:** Aesthetic liking is the main goal and exact category discrimination is less important. **Why:** Increasing name difference can work against the preference patterns favored by Pair Preference.

## Costs of emphasizing name difference <!-- role: costs -->

**Sacrifice:** Some palette liking.
**Risk:** A strongly name-separated palette can be less preferred than a palette built around pair preference.
**Mitigation:** Balance name difference with preference after confirming that the key category pairs remain easy to tell apart.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Treating perceptual distance alone as enough for a nominal hue palette that readers will identify by name. **Why it fails:** Two colors can still attract overlapping everyday names and be confused in use.

## How to test the naming separation <!-- role: check -->

**Failure Sign:** Reviewers use the same or neighboring everyday names for two different category colors.
**Quick Check:** Ask several reviewers to name each palette color; if two categories attract overlapping names, revise that pair.
**Stronger Test:** Compare the current palette against a more name-distinct version on the same aggregate color task, focusing on the most confusable named pair.

## What to change <!-- role: fix -->

- Replace ambiguous intermediate hues with hues that attract more distinct common names.
- Revise the smallest-gap pair first rather than changing the whole palette at once.
- Keep the revised palette only if it reduces confusion on the same aggregate color task.
