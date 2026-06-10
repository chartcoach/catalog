---
id: use-color-encoding-for-time-series-mean-and-variance-judgments
title: Encode time-series magnitude with color for mean and variance judgments
bibliography: references.bib
description: For overview summary tasks in ordered-time displays, prefer color encoding
  on time-series views to improve fidelity and mitigate inaccurate mean or variance
  estimation for viewers scanning aggregated temporal patterns.
labels:
- purpose:refine
- basis:empirical
- time:ordered-time
- data:temporal
- quality:fidelity:use
- lever:encoding
- operator:distribution
- reading-mode:overview
---

## Map the summary judgment to color <!-- role: advice -->

Use color to encode time-series values when viewers must judge overall mean or variance across intervals. For example, switch from a position-traced time-series display to a color-field style display when the job is to summarize average level or variability across months or other ordered periods.

## Why color helps these temporal summaries <!-- role: reason -->

Color-based temporal displays support rapid visual summarization of the collection rather than point-by-point tracing. That makes them better matched to judgments about overall level and spread than to local extrema lookup.

**Mechanism:** Color supports aggregation of many values into an overall summary, which improves mean and variance judgments over time.

**Evidence:** The review collates this paper as a source on temporal aggregate and extremum-related tasks. In its summary-task discussion, the paper reports that mean and variance were more accurately extracted from time-series data encoded using color than from positional visualizations [@zengReviewCollationGraphical2023; @szafirFourTypesEnsemble2016].

## Use when the temporal readout is a summary <!-- role: context -->

- **User Goal:** Judge average level or variability over time.
- **Task:** Estimate mean or variance from an ordered series.
- **Data:** One temporal sequence shown across ordered intervals.
- **Chart Setting:** A static time-series view where the same values could be encoded by position or by color.
- **Success Criterion:** More accurate mean or variance judgments.

## Do not use this when the task is about extrema or range <!-- role: exceptions -->

**Break it when:** The viewer must find maxima, minima, or value range in the time series. **Why:** The same discussion reports that position-based views better support those identification tasks.

## Tradeoffs of using color for temporal summaries <!-- role: costs -->

**Sacrifice:** You give up strength on local extrema and range reading.
**Risk:** A color summary view can underserve tasks that depend on locating highs, lows, or span.
**Mitigation:** Use the color-encoded version only when mean or variance is the primary readout.

## Common failure with color summary views <!-- role: mistakes -->

**Mistake:** Keeping a color-encoded temporal view when the real task is to spot maxima, minima, or range. **Why it fails:** The reported advantage of color applies to summary judgments, not to those identification judgments.

## Check whether the chart is serving the intended temporal task <!-- role: check -->

**Failure Sign:** Reviewers can describe overall level poorly or disagree about which period is more variable.
**Quick Check:** Compare the current position-based view with a color-encoded version using the same data and ask which better supports mean or variance judgments.
**Stronger Test:** Ask reviewers which of two intervals has the higher average or greater variability and compare agreement across the two encodings.

## Fix the temporal encoding <!-- role: fix -->

- Replace the position-traced summary view with a color-encoded temporal view when mean or variance is the main task.
- Keep the temporal summary task tied to color rather than to positional tracing.
