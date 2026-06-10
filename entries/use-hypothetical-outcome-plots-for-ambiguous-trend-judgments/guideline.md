---
id: use-hypothetical-outcome-plots-for-ambiguous-trend-judgments
title: Use hypothetical outcome plots for ambiguous trend judgments
bibliography: references.bib
description: For trend judgment in ordered-time displays, use animated hypothetical
  outcome samples on time-series uncertainty charts to improve fidelity and mitigate
  misreading of sampling variability for novice public audiences.
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

## Animate hypothetical outcomes <!-- role: advice -->

Encode uncertainty as animated hypothetical outcome samples when readers must decide which trend most likely produced noisy observations. For example, replace bar-chart error bars with a bar HOP, or replace a static line ensemble with a line HOP, when the chart asks viewers to choose between competing trends.

## Lower the evidence threshold for correct trend judgments <!-- role: reason -->

Animated hypothetical outcomes let readers experience variability as repeated sampled cases instead of decoding a summary statistic. That makes the uncertainty part of the comparison rather than a separate abstraction that readers may ignore or misread.

**Mechanism:** Sequential samples expose how noisy observations can still come from different underlying trends, so readers can judge the likelihood of each trend with less evidence.

**Evidence:** In experiment 1, bar HOPs produced lower JNDs than bar charts with error bars, meaning participants could identify the underlying trend with less evidence. In experiment 2, regular-rate line HOPs also produced lower JNDs than static line ensembles for the same trend-inference task [@kaleHypotheticalOutcomePlots2019].

## Use when readers must compare noisy trends <!-- role: context -->

- **User Goal:** Decide which of a small number of alternative trends is more likely.
- **Task:** Compare uncertain trends and infer which one produced a noisy sample.
- **Data:** Quantitative ordered-time samples with visible sampling error or other process noise.
- **Chart Setting:** The chart can show uncertainty as repeated samples on the same bars or lines used for the main series.
- **Audience:** Untrained readers with limited statistical background.
- **Success Criterion:** Readers make correct trend judgments from more ambiguous samples.

## Do not use when motion will not be attended <!-- role: exceptions -->

**Break it when:** Viewers cannot or will not watch the display long enough to integrate several frames. **Why:** HOPs depend on temporal integration, so the uncertainty cue weakens when the motion is not actually read.

## Trade off static glanceability for experiential uncertainty <!-- role: costs -->

**Sacrifice:** A HOP needs time to play repeated samples instead of showing everything in one static glance.
**Risk:** Readers who ignore the motion may miss the variability cue.
**Mitigation:** Keep the motion focused on the uncertainty comparison and use a trackable playback rate.

## Do not fall back to summary uncertainty marks for this task <!-- role: mistakes -->

**Mistake:** Adding error bars or another summary-only uncertainty layer for the same ambiguous trend judgment. **Why it fails:** Summary marks hide the sampled process that readers need to compare, so viewers need stronger evidence before they can make the correct call.

## Test the same ambiguous sample both ways <!-- role: check -->

**Failure Sign:** Readers succeed only when the slope is obvious and fail on borderline samples.
**Quick Check:** Show the same ambiguous sample with the current uncertainty display and with a HOP; if correct choices appear only with the HOP, the current encoding is under-communicating variability.
**Stronger Test:** Run repeated forced-choice judgments across samples with different evidence levels and check whether the HOP lowers the evidence needed for correct decisions.

## Replace summary uncertainty with sampled outcomes <!-- role: fix -->

- Draw repeated plausible outcomes from each model or trend and animate them as the same bars or lines used in the chart.
- Remove summary uncertainty marks such as error bars for this judgment task.
- If the current uncertainty view is a static line ensemble, convert those sampled lines into a sequential HOP.
