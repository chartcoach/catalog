---
id: keep-hypothetical-outcome-plot-playback-slow-enough-to-perceive-samples
title: Keep hypothetical outcome plot playback slow enough to perceive individual
  samples
bibliography: references.bib
description: For trend judgment in ordered-time displays, use a cognitively trackable
  animation rate on hypothetical outcome plots to improve fidelity and mitigate loss
  of sensitivity from over-fast playback for novice public audiences.
labels:
- purpose:refine
- basis:empirical
- task:trend
- time:ordered-time
- quality:fidelity
- lever:encoding
- operator:uncertainty
- temporal-pattern:dynamic
- literacy:novice
---

## Slow the HOP to a trackable pace <!-- role: advice -->

Set hypothetical outcome plots to a rate that still lets viewers cognize individual samples. For example, use a regular pace around 400 ms per sample rather than a very fast pace around 100 ms per sample when animating uncertain lines for ambiguous trend judgments.

## Preserve the benefit of animated sampling <!-- role: reason -->

Very fast playback can turn the animation into a blur of change rather than a readable stream of sampled outcomes. When viewers can still pick up individual samples, the animation more reliably supports the uncertainty judgment.

**Mechanism:** A trackable rate preserves viewers' ability to integrate repeated outcomes over time, while over-fast playback weakens that readout and reduces the consistency of the benefit.

**Evidence:** Regular-rate line HOPs with 400 ms per sample produced lower JNDs than static line ensembles, while fast HOPs with 100 ms per sample showed only a smaller and unreliable advantage. The paper interprets this attenuation as a sign that very fast playback can outrun viewers' ability to process the animated samples [@kaleHypotheticalOutcomePlots2019].

**Notes:** The paper treats 400 ms as a supported starting point, not a settled universal optimum.

## Use when the chart already relies on animated samples <!-- role: context -->

- **User Goal:** Infer which trend is more likely from a noisy time series.
- **Task:** Integrate multiple hypothetical outcomes over time.
- **Data:** Quantitative ordered-time series with uncertainty shown as repeated sampled outcomes.
- **Chart Setting:** The chart already uses an animated HOP instead of a static uncertainty view.
- **Audience:** Untrained readers who need to notice variation without training.
- **Success Criterion:** The HOP improves judgments consistently across viewers.

## Do not use when viewers will not watch the animation <!-- role: exceptions -->

**Break it when:** The setting cannot rely on viewers to watch several frames of animation. **Why:** Even a well-paced HOP depends on temporal attention, so the benefit disappears if the animation is not actually seen.

## Trade off speed for perceptibility <!-- role: costs -->

**Sacrifice:** Slower playback shows fewer samples per second.
**Risk:** If the animation is slowed too much, viewers may become impatient.
**Mitigation:** Slow the HOP only enough to preserve recognition of individual samples.

## Do not compress frames just to show more samples faster <!-- role: mistakes -->

**Mistake:** Shortening HOP playback to a very fast rate so more frames fit into less time. **Why it fails:** The performance gain weakened at 100 ms per sample, so extra speed can erase the benefit of the animated uncertainty display.

## Compare the planned speed against a faster version <!-- role: check -->

**Failure Sign:** Speeding up the HOP stops improving decisions or lowers confidence on ambiguous samples.
**Quick Check:** Show the same ambiguous samples at the planned rate and at a much faster rate; if the faster version removes the advantage, playback is too fast.
**Stronger Test:** Run repeated forced-choice judgments and check whether the evidence needed for correct decisions rises as the per-sample duration is shortened.

## Lengthen per-sample dwell time <!-- role: fix -->

- Increase per-sample dwell time until viewers can still perceive individual observations.
- Use a regular-rate HOP around 400 ms per sample as the starting point for this task, not 100 ms-like rapid playback.
- Re-test the speed on ambiguous samples after any change.
