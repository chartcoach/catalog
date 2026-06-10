---
id: do-not-tune-perceptually-uniform-multi-hue-palettes-to-chase-retrieval-performance
title: Do not tune perceptually uniform multi-hue palettes to chase retrieval performance
bibliography: references.bib
description: For retrieve tasks, avoid switching among perceptually uniform multi-hue
  sequential color scales on quantitative color encodings to prevent over-interpreting
  negligible performance differences and address unnecessary palette tuning for viewers
  comparing values against a legend.
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

## Multi-hue palette tuning <!-- role: advice -->

Do not switch among perceptually uniform multi-hue sequential ramps to chase retrieval speed or accuracy. For example, viridis, plasma, and magma did not produce a significant performance difference in the tested quantitative retrieval task.

## Why this tuning does not pay off <!-- role: reason -->

Within the tested perceptually uniform multi-hue family, the alternatives produced very similar retrieval behavior. That means family choice mattered more than fine-grained switching inside the family.

**Mechanism:** When readers are already using an ordered perceptually uniform multi-hue ramp, changing to another member of the same family does not substantially alter how they recover relative value distance from color.

**Evidence:** The review records a weak accuracy ordering among viridis, plasma, and magma and a tie for time, with no significant pairs; the original study likewise found no significant differences among these multi-hue palettes for either response time or error in the retrieval task [@zengReviewCollationGraphical2023; @liuSomewhereRainbowEmpirical2018].

## Use when this is the decision <!-- role: context -->

- **User Goal:** Improve retrieval performance on an existing perceptually uniform multi-hue quantitative color scale.
- **Task:** Compare relative closeness of encoded values using a legend.
- **Data:** Scalar quantitative values encoded with a perceptually uniform multi-hue sequential palette.
- **Chart Setting:** The planned revision is only a swap among the tested multi-hue ramps.
- **Audience:** Readers decoding magnitude from color.
- **Success Criterion:** A measurable gain in speed or accuracy.

## When not to use this rule <!-- role: exceptions -->

**Break it when:** You are deciding between a perceptually uniform multi-hue palette and a different palette family. **Why:** This rule only covers within-family swaps among the tested multi-hue sequential ramps.

## What this costs <!-- role: costs -->

**Sacrifice:** You give up palette iteration as a primary performance fix within the tested multi-hue family.
**Risk:** A real retrieval problem can persist if the issue lies outside this family-level choice.
**Mitigation:** If performance is still weak, compare the current multi-hue ramp against a different palette family instead of another within-family variant.

## Common failure around this change <!-- role: mistakes -->

**Mistake:** Replacing one perceptually uniform multi-hue ramp with another after readers struggle, without changing anything else. **Why it fails:** The tested multi-hue ramps were statistically indistinguishable on the retrieval task.

## How to test the tuning decision <!-- role: check -->

**Failure Sign:** Retrieval performance does not improve after a swap between multi-hue variants.
**Quick Check:** A/B test the current multi-hue ramp against another multi-hue ramp on the same chart and retrieval question.
**Stronger Test:** Record time and error for both versions; if the difference stays negligible, stop tuning within the family.

## What to change <!-- role: fix -->

- Stop rotating among perceptually uniform multi-hue variants as the main retrieval-performance intervention.
- Keep one multi-hue ramp and compare it against a different palette family if retrieval remains weak.
- Evaluate any further palette change with the same legend-based retrieval question.
