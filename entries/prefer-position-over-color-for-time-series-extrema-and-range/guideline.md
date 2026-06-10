---
id: prefer-position-over-color-for-time-series-extrema-and-range
title: Prefer position encoding over color encoding for time-series extrema and range
  comparisons
bibliography: references.bib
description: For point-level extremum and range comparisons in ordered time, prefer
  position encoding on time-series displays to maximize fidelity and mitigate missed
  interval highs and lows for exact interval judgments.
labels:
- purpose:refine
- basis:empirical
- task:extreme
- time:ordered-time
- quality:fidelity
- lever:encoding
- channel:position:use
- channel:color-saturation:avoid
---

## Choose the value channel <!-- role: advice -->

Encode values with position when readers must find interval maxima, minima, or ranges in a time series. For example, use a line-based or box-plot position display instead of a colorfield or color-stock display when the question is which interval contains the highest point, lowest point, or widest within-interval span.

## Why position works better here <!-- role: reason -->

Point comparisons require readers to recover specific values before they compare intervals. Position supports that recovery more faithfully than color saturation, which is less accurate for exact point lookup.

**Mechanism:** Position makes local highs, lows, and gaps easier to read directly, so readers do less inferential work before making the interval comparison.

**Evidence:** In the time-series study collated by the review, position-based displays outperformed color-based displays on maxima, minima, and range questions, and the review summarizes the same paper as showing position-based charts beating color-based charts for find-extremum and determine-range tasks. [@albersTaskdrivenEvaluationAggregation2014; @zengReviewCollationGraphical2023]

## Use when point values drive the decision <!-- role: context -->

- **User Goal:** Pick the interval with the highest point, lowest point, or largest within-interval range.
- **Task:** Point comparison across repeated time intervals.
- **Data:** Ordered time series partitioned into repeated intervals such as months.
- **Chart Setting:** Static time-series display where values could be encoded by either vertical position or color saturation.
- **Success Criterion:** Higher answer accuracy on interval-level extrema or range questions.

## Do not use when the task is summary-first <!-- role: exceptions -->

**Break it when:** The primary question is interval average or spread rather than point maxima, minima, or range. **Why:** the same study found summary-oriented designs performed better on those summary tasks than raw point extraction alone.

## What you give up <!-- role: costs -->

**Sacrifice:** Some fast field-level summarization that color-based views can support.
**Risk:** A position-first view can be a worse fit for average and spread judgments.
**Mitigation:** Switch to interval summary encodings when the task changes from point lookup to summary comparison.

## Common channel mistake <!-- role: mistakes -->

**Mistake:** Keep a colorfield as the main value encoding for a max, min, or range task. **Why it fails:** Readers must infer exact point values from color, and accuracy drops on point comparisons.

## How to check the choice <!-- role: check -->

**Failure Sign:** Reviewers hesitate or disagree about which interval contains the highest point, lowest point, or widest range when reading a color-encoded series.
**Quick Check:** Show the same series once with position encoding and once with color encoding, then ask three forced-choice interval questions on max, min, and range.
**Stronger Test:** Keep the position version if it yields more accurate answers on brief interval extrema and range questions.

## How to fix it <!-- role: fix -->

- Replace color-saturation value encoding with vertical position for views whose main job is max, min, or range comparison.
- If interval summaries must stay visible, add position marks that expose interval highs and lows directly.
- Remove color-only value views from tasks that depend on exact point extraction.
