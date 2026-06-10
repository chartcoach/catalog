---
id: prefer-discriminability-weighted-hue-palettes-for-aggregate-color-comparisons
title: Prefer discriminability-weighted hue palettes for aggregate color comparisons
bibliography: references.bib
description: For aggregate color comparisons, prefer a discriminability-weighted hue
  palette on nominal color encodings to improve fidelity and address confusion between
  similar categories for readers scanning many colored marks.
labels:
- purpose:refine
- basis:empirical
- data:categorical
- quality:fidelity:use
- lever:encoding
- channel:color-hue:use
- aesthetic:color:use
---

## Weight the palette toward discrimination <!-- role: advice -->

Use a categorical hue palette that gives more weight to discrimination than to pairwise liking when readers must compare aggregates by color. For example, choose a low-error or discrimination-weighted palette for a many-region display instead of a palette tuned mainly for Pair Preference when readers must decide which side or area contains more of a target category.

## Why discrimination weighting works <!-- role: reason -->

Readers make fewer mistakes when the weakest color pair in the palette is easier to tell apart. Pushing the palette too far toward pairwise liking can make the overall palette more appealing while making target-versus-distractor color judgments less reliable.

**Mechanism:** Increasing palette discriminability improves separation between the most confusable category colors, which helps readers identify the target color and compare aggregate counts more accurately and often more quickly.

**Evidence:** The collated review records this paper as evidence about nominal color-hue design for aggregate tasks. In the paper, errors and response times generally improved as discriminability scores increased, while higher Pair Preference increased liking but reduced discrimination performance; low-error palettes also outperformed more preferable palettes on error in key conditions. [@zengReviewCollationGraphical2023; @gramazioColorgoricalCreatingDiscriminable2017]

## Use when all of these are true <!-- role: context -->

- **User Goal:** Decide which side, area, or group contains more of a target category.
- **Task:** Compare aggregates by color rather than admire the palette.
- **Data:** Nominal categories are distinguished by hue.
- **Chart Setting:** Many small colored regions or marks are shown at once, and a legend or label identifies the target color.
- **Audience:** Readers are making quick color-based judgments.
- **Success Criterion:** Fewer errors, and preferably faster responses.

## Do not use when any of these are true <!-- role: exceptions -->

**Break it when:** The main goal is to maximize how much viewers like the palette and some loss of discrimination is acceptable. **Why:** Pair-preference-heavy palettes were judged more preferable on average, but that gain came with worse discrimination.

## Costs of weighting toward discrimination <!-- role: costs -->

**Sacrifice:** Some palette liking.
**Risk:** A purely discrimination-driven palette can feel less preferable than a pair-preference-heavy palette.
**Mitigation:** Keep some preference weight if the display must also feel appealing, but validate that the aggregate comparison still stays accurate.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Optimizing a categorical hue palette mainly for pairwise liking when readers must compare counts by color. **Why it fails:** The palette may look better but make the target color harder to separate from its nearest distractor.

## How to test the palette choice <!-- role: check -->

**Failure Sign:** Reviewers hesitate or disagree about which side or area has more of the target category.
**Quick Check:** Compare the current palette against a more discrimination-weighted version on the same aggregate color task and look for fewer errors.
**Stronger Test:** Test the weakest color pair directly by using one as the target and the other as the main distractor in a timed left-versus-right count comparison.

## What to change <!-- role: fix -->

- Shift palette weighting away from Pair Preference and toward discrimination.
- Regenerate the palette and compare it on the same aggregate color task.
- Inspect the most confusable color pair first and keep the version that lowers confusion on that pair.
