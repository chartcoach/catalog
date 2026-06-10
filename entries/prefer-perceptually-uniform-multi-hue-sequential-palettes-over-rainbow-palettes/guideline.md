---
id: prefer-perceptually-uniform-multi-hue-sequential-palettes-over-rainbow-palettes
title: Prefer a perceptually uniform multi-hue sequential palette over a rainbow palette
bibliography: references.bib
description: For retrieve tasks, prefer a perceptually uniform multi-hue sequential
  color scale on quantitative color encodings to improve fidelity and mitigate slower,
  more error-prone relative-value judgments for viewers comparing values against a
  legend.
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

## Sequential palette replacement <!-- role: advice -->

Replace a rainbow quantitative palette with a perceptually uniform multi-hue sequential palette when people must retrieve values from color. For example, switch from a rainbow ramp such as jet to a perceptually uniform sequential ramp such as viridis when readers must judge which encoded value is closer to a reference.

## Why the sequential replacement works <!-- role: reason -->

A perceptually uniform multi-hue sequential palette preserves an ordered scale while giving readers cleaner distance cues across the legend. A rainbow palette made the same retrieval task slower and more error-prone.

**Mechanism:** The palette change improves how reliably readers map color distance back to value distance, so they make fewer wrong closeness judgments and spend less time resolving the comparison.

**Evidence:** In the assorted-palette comparison, viridis had the best accuracy and significantly outperformed jet, while jet was the slowest and most error-prone option overall; the review collates the same pattern from this study into an actionable ranking for quantitative color retrieval [@liuSomewhereRainbowEmpirical2018; @zengReviewCollationGraphical2023].

## Use when this is the task <!-- role: context -->

- **User Goal:** Retrieve which of two encoded values is closer to a reference.
- **Task:** Value retrieval from a continuous quantitative color scale.
- **Data:** Scalar quantitative values mapped to color.
- **Chart Setting:** A static chart with a visible color legend.
- **Audience:** Readers who must decode value differences from color rather than another channel.
- **Success Criterion:** Lower retrieval error and faster response time.

## When not to use this palette swap <!-- role: exceptions -->

**Break it when:** The color scale is not a single ordered quantitative ramp and instead must encode a different structure such as a midpoint-centered scheme. **Why:** This guideline is supported by the study's sequential-versus-rainbow retrieval comparison, not by all possible color-scale semantics.

## What this costs <!-- role: costs -->

**Sacrifice:** You give up the familiar rainbow look.
**Risk:** Treating every non-rainbow palette as equally good can overstate the evidence.
**Mitigation:** Compare the current rainbow palette directly against a perceptually uniform sequential alternative on the same retrieval question.

## Common failure around this change <!-- role: mistakes -->

**Mistake:** Replacing a rainbow palette with another non-sequential-looking palette and assuming the retrieval problem is solved. **Why it fails:** The supported benefit is tied to an ordered perceptually uniform sequential ramp, not to any arbitrary palette change.

## How to test the palette change <!-- role: check -->

**Failure Sign:** Readers hesitate or miss closest-value judgments when using the rainbow scale.
**Quick Check:** Show the same chart once with the rainbow palette and once with a perceptually uniform sequential palette, then ask which of two colored values is closer to a reference.
**Stronger Test:** Compare both error rate and response time across several legend locations before keeping the new palette.

## What to change <!-- role: fix -->

- Replace the rainbow ramp with a perceptually uniform multi-hue sequential ramp.
- Keep the same legend and rerun the same closest-to-reference check on the revised palette.
- Keep the new palette only if it reduces retrieval errors or time on the same chart task.
