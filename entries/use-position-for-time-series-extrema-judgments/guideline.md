---
id: use-position-for-time-series-extrema-judgments
title: Use position encoding for extrema and range judgments in time-series views
bibliography: references.bib
description: For extrema judgments on ordered-time data, use position encoding on
  time-series views to improve fidelity and mitigate misreading of maxima, minima,
  and range for overview readers.
labels:
- purpose:refine
- basis:empirical
- task:retrieve
- time:ordered-time
- data:temporal
- quality:fidelity
- lever:encoding
- reading-mode:overview
---

## Extrema encoding <!-- role: advice -->

Encode time-series values with position when the main readout is the minimum, maximum, or range across time. For example, keep peaks and troughs in a positional line display rather than a color-only time view when readers must spot the highest period or widest spread.

## Why position helps extrema judgments <!-- role: reason -->

Position makes boundary values and spread easier to see as parts of a visible shape.

**Mechanism:** Positional encodings expose highs, lows, and overall span directly, which supports identification tasks such as finding extrema and range.

**Evidence:** The paper reports time-series studies in which extrema and range were judged more accurately from positional encodings than from color encodings, while color performed better for mean and variance [@szafirFourTypesEnsemble2016].

**Notes:** This is the complementary side of the summary-versus-identification tradeoff.

## Use when identification readout is primary <!-- role: context -->

- **User Goal:** Find the highest, lowest, or widest-spread interval in a time series.
- **Task:** Identify extrema or compare ranges.
- **Data:** Ordered-time values shown across many points or intervals.
- **Chart Setting:** A time-series view can encode the same values with either position or color.
- **Success Criterion:** Readers can accurately locate maxima, minima, or the largest range.

## Do not use when the task is summary estimation <!-- role: exceptions -->

**Break it when:** The primary question is the average level or variability of an interval. **Why:** Color encodings supported those summary judgments more accurately in the reported studies.

## Tradeoffs of positional extrema encoding <!-- role: costs -->

**Sacrifice:** Average level and variability are less directly summarized than in a color encoding.\
**Risk:** Readers may overfocus on peaks and troughs when the intended question is about mean or variance.\
**Mitigation:** Keep this encoding only when extrema or range is the key readout.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Using a positional time-series view as the main display for average or variance judgments. **Why it fails:** The reported tradeoff showed position helping identification tasks more than summary tasks.

## Check extrema-readout fit <!-- role: check -->

**Failure Sign:** Reviewers can describe overall level but struggle to point to the true maximum, minimum, or range.\
**Quick Check:** Show a positional version and a color version of the same series, then ask extrema and range questions; keep the version that yields cleaner answers on those tasks.\
**Stronger Test:** Compare error rates on representative maximum, minimum, and range questions across the two encodings.

## Fix the encoding <!-- role: fix -->

- Re-encode the time-series values with position instead of relying on color alone.
- Restore a line-based view when readers need to see peaks, troughs, and span directly.
- Remove the position-first version from the primary view if the task shifts to mean or variance estimation.
