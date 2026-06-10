---
id: do-not-tune-single-hue-sequential-palettes-to-chase-retrieval-performance
title: Do not tune single-hue sequential palettes to chase retrieval performance
bibliography: references.bib
description: For retrieve tasks, avoid switching among single-hue sequential color
  scales on quantitative color encodings to prevent over-interpreting negligible performance
  differences and address unnecessary palette tuning for viewers comparing values
  against a legend.
labels:
- purpose:refine
- basis:empirical
- task:retrieve
- data:quantitative
- quality:fidelity
- lever:encoding
- reading-mode:lookup
- polish:palette
---

## Single-hue palette tuning <!-- role: advice -->

Do not swap one single-hue sequential ramp for another to chase retrieval speed or accuracy. For example, changing between greys, blues, greens, and oranges did not produce a significant performance difference in the tested quantitative retrieval task.

## Why this tuning does not pay off <!-- role: reason -->

Within the tested single-hue family, the palette hue changed the look of the scale more than it changed the retrieval result. Readers performed similarly across the single-hue options, so hue swapping inside that family was not an effective speed-or-accuracy intervention.

**Mechanism:** When the only edit is changing the hue of a single-hue sequential ramp, the retrieval task still relies on the same basic ordered color progression, so performance stays within the same range.

**Evidence:** The review records the single-hue family as a weak ordering for accuracy and a tie for time, with no significant pairs; the original study likewise found no significant differences among greys, blues, greens, and oranges for either error or response time in the retrieval task [@zengReviewCollationGraphical2023; @liuSomewhereRainbowEmpirical2018].

## Use when this is the decision <!-- role: context -->

- **User Goal:** Improve retrieval performance on an existing single-hue quantitative color scale.
- **Task:** Compare relative closeness of encoded values using a legend.
- **Data:** Scalar quantitative values encoded with a single-hue sequential palette.
- **Chart Setting:** The planned revision is only a swap among single-hue ramps.
- **Audience:** Readers decoding magnitude from color.
- **Success Criterion:** A measurable gain in speed or accuracy.

## When not to use this rule <!-- role: exceptions -->

**Break it when:** You are deciding between a single-hue palette and a different palette family. **Why:** This rule only covers within-family swaps among the tested single-hue sequential ramps.

## What this costs <!-- role: costs -->

**Sacrifice:** You give up palette iteration as a primary performance fix within the single-hue family.
**Risk:** Keeping the same palette family can leave a real retrieval problem unresolved.
**Mitigation:** If performance is still weak, compare the current single-hue ramp against a different palette family instead of another single-hue hue.

## Common failure around this change <!-- role: mistakes -->

**Mistake:** Recoloring a single-hue ramp from one hue to another after readers miss value comparisons. **Why it fails:** The tested single-hue ramps were statistically indistinguishable on the retrieval task.

## How to test the tuning decision <!-- role: check -->

**Failure Sign:** The chart still produces retrieval errors after a hue-only swap inside the single-hue family.
**Quick Check:** A/B test the current single-hue ramp against another single-hue ramp on the same chart and retrieval question.
**Stronger Test:** Record time and error for both versions; if the difference stays negligible, stop tuning within the family.

## What to change <!-- role: fix -->

- Stop rotating among single-hue hues as the main retrieval-performance intervention.
- Keep one single-hue ramp and compare it against a different palette family if retrieval remains weak.
- Evaluate any further palette change with the same legend-based retrieval question.
