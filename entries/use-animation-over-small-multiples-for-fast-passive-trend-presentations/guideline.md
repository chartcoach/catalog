---
id: use-animation-over-small-multiples-for-fast-passive-trend-presentations
title: Use animation instead of small multiples for fast passive trend presentations
bibliography: references.bib
description: For passive presentation of trends over ordered time, prefer a single
  animated view on multidimensional scatter plots to improve insight speed and mitigate
  slow panel scanning for viewers.
labels:
- purpose:select
- basis:empirical
- task:trend
- time:ordered-time
- structure:single-view:use
- structure:small-multiples:avoid
- quality:insight:use
- lever:layout-structure
- communication:workflow
---

## Use one animated overview for passive viewing <!-- role: advice -->

Choose a single animated view instead of a small-multiples grid when viewers are watching a presentation and need a quick read. For example, animate positions over time in one bubble chart rather than asking viewers to scan many static panels during the talk.

## One moving view is faster for passive audiences <!-- role: reason -->

A single animated overview lets the audience watch one place instead of scanning a grid of panels. In the study, that made presentation tasks faster and also made the display feel more exciting, even though accuracy suffered.

**Mechanism:** Animation concentrates attention into one shared view and reduces the time needed to scan across many separate panels during passive viewing.

**Evidence:** In presentation mode, animation was significantly faster than small multiples, and participants rated animation as more enjoyable and exciting, although the paper also reports many participant errors with animation [@robertsonEffectivenessAnimationTrend2008].

**Notes:** This rule is about speed and engagement in passive presentation, not about analytic accuracy.

## Use when the audience is watching, not exploring <!-- role: context -->

- **User Goal:** Follow a narrated temporal story quickly.
- **Task:** Passive presentation rather than analysis.
- **Data:** Ordered-time changes in a multidimensional scatter or bubble view.
- **Chart Setting:** The audience is not controlling playback and is not interacting with the chart.
- **Audience:** Viewers watching a talk or walkthrough.
- **Success Criterion:** Fast audience response and an engaging presentation.

## Do not use when viewers need accurate or unguided answers <!-- role: exceptions -->

**Break it when:** Viewers must answer accurately on their own, or the data contains too many points, reversals, or unsynchronized movement. **Why:** The paper found many errors with animation and concludes that animation becomes confusing when there are too many data points or when paths reverse or do not move in synchrony.

## Tradeoffs of the animated overview <!-- role: costs -->

**Sacrifice:** You give up some answer accuracy.
**Risk:** Viewers may lose track of moving points and miss reversals.
**Mitigation:** Reserve animation for the walkthrough, and switch to a static view when viewers need exact answers.

## Common failure around animation in presentations <!-- role: mistakes -->

**Mistake:** Using animation for exact-answer tasks or unguided analysis because it feels engaging. **Why it fails:** The display is fast and exciting, but participants still made many errors and often lost track of points.

## How to test the presentation choice <!-- role: check -->

**Failure Sign:** Viewers miss answers after one run or say they lost track of moving points.
**Quick Check:** Show one representative task with animation and one with small multiples; if the audience needs the animated view replayed to answer correctly, do not use animation for that task.
**Stronger Test:** Confirm that viewers can answer after a single narrated run without asking to replay the motion.

## What to change <!-- role: fix -->

- Use animation only for the presentation walkthrough, not as the main analysis view.
- Switch to small multiples or traces when the audience must answer accurately.
- Reduce the number of moving points if the animation feels crowded.
- Avoid animated stories built from paths that reverse often or move without synchrony.
