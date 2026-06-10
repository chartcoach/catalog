---
id: use-color-for-time-series-summary-judgments
title: Use color encoding for mean and variance judgments in time-series views
bibliography: references.bib
description: For summary judgments on ordered-time data, use color encoding on time-series
  views to improve fidelity and mitigate misreading of mean and variance for overview
  readers.
labels:
- purpose:refine
- basis:empirical
- task:distribute
- time:ordered-time
- data:temporal
- quality:fidelity
- lever:encoding
- reading-mode:overview
---

## Summary encoding <!-- role: advice -->

Encode time-series values with color when the main readout is the average level or variability across an interval. For example, use a color-coded time view rather than relying only on line position when readers need to judge which period has the higher mean or greater variance.

## Why color helps summary judgments <!-- role: reason -->

Color lets readers treat an interval as an aggregate instead of tracing individual highs and lows one by one.

**Mechanism:** Color supports ensemble-style summary judgments, which helps readers estimate average value and variability across many time points.

**Evidence:** The paper reports time-series studies in which mean and variance were judged more accurately from color encodings than from positional encodings, while the reverse pattern held for extrema and range [@szafirFourTypesEnsemble2016].

**Notes:** This is a task tradeoff, not a claim that color is always better than position.

## Use when summary readout is primary <!-- role: context -->

- **User Goal:** Compare average level or variability across time intervals.
- **Task:** Estimate mean or variance from a time-series display.
- **Data:** Ordered-time values shown across many points or intervals.
- **Chart Setting:** A time-series view can encode the same values with either color or position.
- **Success Criterion:** Readers can accurately tell which interval is higher on average or more variable.

## Do not use when extrema are the question <!-- role: exceptions -->

**Break it when:** The primary question is the minimum, maximum, or range in the series. **Why:** Positional encodings supported those identification judgments more accurately in the reported time-series studies.

## Tradeoffs of color summary encoding <!-- role: costs -->

**Sacrifice:** Peaks, troughs, and range become less direct than in a positional display.\
**Risk:** Readers may miss the highest point or widest spread if the chart is asked to do both summary and extrema work at once.\
**Mitigation:** Keep this encoding only when mean or variance is the main readout.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keeping a positional time-series view as the primary display when the real task is average or variability judgment. **Why it fails:** Position helped extrema and range more than summary statistics in the reported tradeoff.

## Check summary-readout fit <!-- role: check -->

**Failure Sign:** Reviewers can find peaks and range but struggle to answer which interval is higher on average or more variable.\
**Quick Check:** Show a color version and a positional version of the same series, then ask mean and variance questions; keep the version that yields cleaner answers on those tasks.\
**Stronger Test:** Compare error rates on representative mean and variance questions across the two encodings.

## Fix the encoding <!-- role: fix -->

- Re-encode the time-series values with color instead of relying only on y-position.
- Replace a line-first summary view with a color-coded time view for the same ordered intervals.
- Remove the color-first version from the primary view if the task shifts to maxima, minima, or range.
