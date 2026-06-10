---
id: use-shared-space-layout-for-local-timepoint-extrema
title: Use a shared-space layout for local time-point extrema
bibliography: references.bib
description: For local extremum comparison in ordered time, prefer a shared-space
  layout on multi-series temporal charts to improve readability and mitigate slow
  cross-row scanning for readers doing quick overview analysis.
labels:
- purpose:select
- basis:empirical
- task:extreme
- time:ordered-time
- structure:single-view:use
- structure:multi-view:avoid
- quality:readability
- lever:layout-structure
---

## Shared-space layout <!-- role: advice -->

Choose a shared-space layout when readers must identify which series is highest at one time point across several time series. For example, use a simple line graph or braided graph instead of per-series rows such as small multiples or horizon graphs for a highest-at-a-time-point comparison.

## Why shared space works here <!-- role: reason -->

A shared-space layout keeps the compared values in one vertical region on a common baseline. That lets readers compare one time point directly instead of shifting their gaze between separate rows.

**Mechanism:** One shared plotting area reduces row-to-row eye movement for a local same-time comparison.

**Evidence:** Controlled comparisons of simple line, braided, small-multiples, and horizon views found the shared-space views faster than the split per-series views for the local maximum/find-extremum task, and the collated record summarizes the same shared-space advantage for this task family [@javedGraphicalPerceptionMultiple2010; @zengReviewCollationGraphical2023].

**Notes:** The reported advantage for this task is in completion time; the structured record does not report significant accuracy pairs here.

## Use when all of these are true <!-- role: context -->

- **User Goal:** Find which series has the highest value at a specified time point.
- **Task:** Local extremum comparison across several simultaneous time series.
- **Data:** Several series share the same ordered time axis.
- **Chart Setting:** Static, noninteractive overview view with all series visible at once.
- **Audience:** Readers making quick cross-series comparisons.
- **Success Criterion:** Faster completion on a same-time highest-value question.

## Do not use when any of these are true <!-- role: exceptions -->

**Break it when:** Readers must compare values at different marked time positions across series or across a long span of the display. **Why:** Split per-series layouts were faster for the dispersed aggregate/discrimination-style comparison task.

## What you give up <!-- role: costs -->

**Sacrifice:** A shared-space layout keeps overlap in one plot.
**Risk:** Line identity and clutter can become harder to follow than in separated rows.
**Mitigation:** Keep the shared-space layout for local same-time questions rather than dispersed cross-series comparisons.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keep each series in separate rows for a same-time highest-value question. **Why it fails:** Separate rows add vertical scanning to a comparison that can be made in one shared position.

## How to review it <!-- role: check -->

**Failure Sign:** Reviewers look up and down between rows to answer one same-time highest-value question.
**Quick Check:** Compare the current per-series-row view against a shared-space view on the same highest-at-this-time question.
**Stronger Test:** Time a few readers on the same question in both layouts and keep the faster one.

## What to change <!-- role: fix -->

- Replace per-series rows with one shared plot for the local comparison view.
- If a plain line overlay is hard to follow, try a braided shared-space view before returning to split rows.
- Keep the compared time point aligned in the same shared plotting region for all series.
