---
id: do-not-rely-on-axis-break-indicators-to-neutralize-truncation
title: Do not rely on axis-break indicators to neutralize truncation
bibliography: references.bib
description: For overview judgments of change, avoid relying on axis-break or continuation
  cues on truncated bar charts to improve fidelity and address the mistaken belief
  that visual warnings remove exaggeration for viewers reading severity from shape.
labels:
- purpose:refine
- basis:empirical
- chart:bar
- data:quantitative
- quality:fidelity:use
- lever:encoding
- component:axis
- reading-mode:overview
---

## Axis-break warnings <!-- role: advice -->

Treat axis-break and continuation styling as disclosure, not as a correction for truncation bias. For example, a broken y-axis with matching breaks in the bars or a gradient that suggests the bars continue below the plot should not be expected to make a truncated bar chart feel less severe.

## Why warning cues do not debias the chart <!-- role: reason -->

Break markers make truncation more explicit, but they do not remove the strong visual impression created by the cropped bars. Readers still judge the visible height above the break, so the chart continues to feel more dramatic than a wider-range view.

**Mechanism:** Axis-break glyphs and continuation cues disclose the missing baseline, but the magnified bar tops remain the dominant cue in subjective effect-size judgments.

**Evidence:** In experiments comparing standard truncated bars, broken-axis bars, and gradient-continuation bars, perceived severity did not decrease reliably for the two warning designs. Truncation level still increased judged severity across these bar-chart variants [@correllTruncatingYAxisThreat2020].

**Notes:** When the y-axis began at 0, the three bar-chart designs were visually identical.

## When this applies <!-- role: context -->

- **User Goal:** Prevent a truncated bar chart from overstating how large a difference feels.
- **Task:** Readers judge how strong or fast a change seems from the chart’s shape.
- **Data:** Quantitative bars sit in a narrow range that invites truncation.
- **Chart Setting:** A static bar chart uses a broken axis, broken bars, or a gradient continuation cue.
- **Audience:** Readers are making quick qualitative judgments rather than careful mathematical corrections.
- **Success Criterion:** The warning treatment materially reduces exaggeration, not just discloses it.

## When to break it <!-- role: exceptions -->

**Break it when:** Your goal is only to disclose that truncation exists, not to neutralize its perceptual effect. **Why:** The paper rejects these cues as debiasing fixes, but it still discusses them as explicit indicators that truncation has taken place.

## Costs of using warning cues alone <!-- role: costs -->

**Sacrifice:** You add visual treatment without reliably reducing the exaggerated effect.
**Risk:** Designers or reviewers may believe the warning solved the problem when the chart still feels too dramatic.
**Mitigation:** Pair disclosure with a wider y-axis range or reconsider whether truncation is necessary.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Replace a standard truncated bar chart with a broken-axis or gradient version while keeping the same truncated range. **Why it fails:** The warning design changes the styling, but the inflated visible bar heights still drive severity judgments.

## How to test it <!-- role: check -->

**Failure Sign:** Standard, broken-axis, and gradient versions with the same truncated range all feel similarly dramatic.
**Quick Check:** Compare the same data and y-axis range in a plain truncated bar chart and in the warning design you plan to use.
**Stronger Test:** Ask reviewers to rate perceived severity across the versions; if the ratings stay close, the warning is not correcting the bias.

## What to change <!-- role: fix -->

- Use the break or gradient only as disclosure, not as the main safeguard against exaggeration.
- Reduce the truncation or restore more y-axis context when neutral effect size matters.
- Compare the disclosed truncated view against a wider-range version before publishing it.
