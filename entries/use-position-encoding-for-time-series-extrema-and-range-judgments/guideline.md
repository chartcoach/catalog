---
id: use-position-encoding-for-time-series-extrema-and-range-judgments
title: Encode time-series magnitude with position for extrema and range judgments
bibliography: references.bib
description: For extreme-finding tasks in ordered-time displays, prefer position encoding
  on time-series views to improve fidelity and mitigate missed maxima, minima, or
  range judgments for viewers scanning temporal patterns.
labels:
- purpose:refine
- basis:empirical
- task:extreme
- time:ordered-time
- data:temporal
- quality:fidelity:use
- lever:encoding
- channel:position:use
---

## Map extrema-finding to position <!-- role: advice -->

Use position to encode time-series values when viewers must find maxima, minima, or value range. For example, keep a line-like positional time-series view when the main job is to see where the series reaches its highest point, lowest point, or widest span.

## Why position helps temporal extrema and range <!-- role: reason -->

Position preserves the shape boundary of the series and makes highs, lows, and span easier to locate directly. Those judgments depend less on aggregate summary and more on seeing where the series reaches its limits.

**Mechanism:** Positional encoding supports identification of local and global extremes by making the boundary of the series easy to inspect.

**Evidence:** The review collates this paper as covering extremum and summary tasks. In its time-series discussion, the paper reports that extrema and range were more accurately extracted from positional visualizations than from color-based ones [@zengReviewCollationGraphical2023; @szafirFourTypesEnsemble2016].

## Use when the temporal readout is about limits <!-- role: context -->

- **User Goal:** Find the highest point, lowest point, or span over time.
- **Task:** Identify extrema or determine range in an ordered series.
- **Data:** One temporal sequence shown across ordered intervals.
- **Chart Setting:** A static time-series view where the same values could be encoded by position or by color.
- **Success Criterion:** More accurate max, min, or range judgments.

## Do not use this when the task is mean or variance summary <!-- role: exceptions -->

**Break it when:** The viewer must estimate overall mean or variability instead of extrema or range. **Why:** The same discussion reports that color-based views better support those summary tasks.

## Tradeoffs of using position for temporal limits <!-- role: costs -->

**Sacrifice:** You give up the stronger support that color offers for mean and variance summaries.
**Risk:** A position-first view can underserve the task when viewers mainly need overall level or spread.
**Mitigation:** Keep the positional view for extremum and range reading rather than for summary estimation.

## Common failure with positional temporal views <!-- role: mistakes -->

**Mistake:** Using a positional time-series display for a summary task and expecting it to be the best view for average or variability judgments. **Why it fails:** The reported advantage of position is specific to extrema and range.

## Check whether position is serving the intended task <!-- role: check -->

**Failure Sign:** Reviewers struggle to identify the highest point, lowest point, or span from a nonpositional temporal view.
**Quick Check:** Compare the current view with a positional version and ask which better supports max, min, or range reading.
**Stronger Test:** Ask reviewers to point to the highest interval, lowest interval, or widest span in both versions and compare agreement.

## Fix the temporal encoding <!-- role: fix -->

- Remap the time-series values to position when the primary task is to find extrema or range.
- Keep the view centered on the positional trace rather than on a color summary when limits are the main target.
