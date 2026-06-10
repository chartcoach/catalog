---
id: use-split-per-series-rows-for-dispersed-cross-series-comparison
title: Use split per-series rows for dispersed cross-series comparisons
bibliography: references.bib
description: For dispersed cross-series value comparison in ordered time, prefer split
  per-series layouts on multi-series temporal charts to improve readability and mitigate
  slow tracing through overlaid series for readers doing quick overview analysis.
labels:
- purpose:select
- basis:empirical
- task:compare
- time:ordered-time
- structure:multi-view:use
- structure:single-view:avoid
- quality:readability
- lever:layout-structure
---

## Split per-series rows <!-- role: advice -->

Choose split per-series rows when readers must compare series values at different time positions across the span of multiple time series. For example, use small multiples or horizon graphs instead of a single overlaid simple line graph or braided graph for a dispersed cross-series value comparison.

## Why split rows work here <!-- role: reason -->

Split per-series rows separate each series vertically, so readers can trace one series across a long span without overlap from the others. That reduces the clutter and long-range line tracing required in shared overlays.

**Mechanism:** Vertical separation makes dispersed comparisons easier because each series can be followed without interference from overlapping series.

**Evidence:** Controlled comparisons found the split per-series views faster than the shared-space views for the dispersed aggregate/discrimination-style task, and the collated record ranks the row-based designs ahead of the overlaid designs on time for this task family [@javedGraphicalPerceptionMultiple2010; @zengReviewCollationGraphical2023].

**Notes:** The structured record emphasizes the time advantage for this task; it does not report significant accuracy pairs.

## Use when all of these are true <!-- role: context -->

- **User Goal:** Compare values from different series at different marked time positions.
- **Task:** Dispersed cross-series comparison over a broad visual span.
- **Data:** Several series share the same ordered time axis.
- **Chart Setting:** Static, noninteractive overview view with all series shown simultaneously.
- **Audience:** Readers making quick cross-series comparisons.
- **Success Criterion:** Faster completion on dispersed comparison questions.

## Do not use when any of these are true <!-- role: exceptions -->

**Break it when:** Readers only need to identify which series is highest at one shared time point. **Why:** Shared-space layouts were faster for the local find-extremum task.

## What you give up <!-- role: costs -->

**Sacrifice:** Split rows weaken direct same-space comparison across series.
**Risk:** Local same-time comparisons become slower because readers must move between rows.
**Mitigation:** Reserve split rows for dispersed comparisons that span different positions or long visual spans.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keep all series overlaid in one shared plot for a dispersed comparison across different time positions. **Why it fails:** Overlap and clutter make long-range tracing across series slower.

## How to review it <!-- role: check -->

**Failure Sign:** Reviewers must trace lines through overlap to compare values located at different positions.
**Quick Check:** Compare the current shared overlay against a split per-series version on the same dispersed comparison question.
**Stronger Test:** Time a few readers on both layouts and keep the faster one for that question type.

## What to change <!-- role: fix -->

- Split the series into separate aligned rows for the dispersed comparison view.
- Use small multiples when the comparison can rely on common axes across rows.
- Use horizon graphs when you want the same row-based separation in a more compressed per-series view.
- Remove the shared overlay from the dispersed comparison view.
