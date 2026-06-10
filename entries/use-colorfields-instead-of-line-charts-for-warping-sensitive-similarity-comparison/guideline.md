---
id: use-colorfields-instead-of-line-charts-for-warping-sensitive-similarity-comparison
title: Use colorfields instead of line charts when similarity should tolerate local
  time warping
bibliography: references.bib
description: For similarity comparison in ordered-time views, use colorfields on time-series
  displays instead of line charts to improve readability and mitigate slower candidate
  scanning for viewers matching temporally warped patterns.
labels:
- purpose:select
- basis:empirical
- task:compare
- time:ordered-time
- chart:heatmap:use
- chart:line:avoid
- quality:readability:use
- lever:chart-family
---

## Choose the time-series chart family for warping-sensitive similarity search <!-- role: advice -->

Use a colorfield instead of a line chart when viewers must quickly choose which candidate time series is most similar to a query and local stretching or shifting in time should still count as similar. For example, show the query and candidates as stacked colorfield strips rather than stacked line traces when the task is to pick the closest match under a dynamic-time-warping style notion of similarity.

## Why the chart swap works <!-- role: reason -->

Colorfields let viewers scan bands of similar color quickly in this task, while line charts require more trace-following across the same time window.

**Mechanism:** A colorfield turns the search into a faster comparison of colored regions across candidates, which speeds up choosing the closest overall pattern when local temporal shifts or stretches are present.

**Evidence:** In the time-warping experiment, colorfields were faster than line charts for choosing the most similar time series to a query, with mean completion times of 15.6 seconds for colorfields versus 20.5 seconds for line charts, and the collated result ranks the colorfield condition ahead of the line-chart condition with a significant pairwise difference [@gogolouComparingSimilarityPerception2019; @zengReviewCollationGraphical2023].

**Notes:** This is a speed guideline, not a blanket claim that colorfields are always the best similarity display.

## Use when these conditions all hold <!-- role: context -->

- **User Goal:** Choose the most similar candidate time series to a shown query.
- **Task:** Visual similarity comparison where local temporal stretching or shifting is part of the intended match.
- **Data:** Multiple time series shown over the same time window and common scale.
- **Chart Setting:** Stacked small-multiple views with comparable vertical space per series.
- **Audience:** Viewers making subjective similarity choices rather than reading exact values.
- **Success Criterion:** Faster selection of the closest matching pattern.

## Do not use when these conditions hold <!-- role: exceptions -->

- **Break it when:** Amplitude or vertical-offset variation is the main deformation you need viewers to ignore. **Why:** The speed advantage over line charts disappeared in the normalization condition.
- **Break it when:** The chart is not being used for query-to-candidate similarity choice. **Why:** The evidence only covers selecting the most similar series from a small set of candidates.

## Know the tradeoffs before you swap <!-- role: costs -->

**Sacrifice:** You give up the direct traced-line view of the signal.
**Risk:** A faster colorfield view can still make stretched or compressed candidates look less similar if viewers focus on the width of colored regions.
**Mitigation:** Test the colorfield on representative similarity prompts before adopting it as the default view.

## Watch for this failure mode <!-- role: mistakes -->

**Mistake:** Switching to a colorfield for every time-series task because it was faster here. **Why it fails:** The evidence is specific to query-based similarity comparison, not to all time-series reading tasks.

## Review the choice with a direct A/B test <!-- role: check -->

**Failure Sign:** Viewers are slower with line charts when picking the closest match to a query under warped patterns.
**Quick Check:** Show the same query-and-candidates set once as line charts and once as colorfields, then compare which version produces a faster confident choice.
**Stronger Test:** Time a short set of representative similarity judgments with both chart families and compare median completion times before standardizing the display.

## Make the revision concretely <!-- role: fix -->

- Replace each line-trace candidate with a colorfield strip for the same time window.
- Keep the query and all candidates on the same scale and comparable display size while testing the swap.
- Re-run a timed query-to-candidate similarity check on representative cases before finalizing the chart family.
- If the speed advantage disappears on your cases, keep the line chart rather than forcing the swap.
