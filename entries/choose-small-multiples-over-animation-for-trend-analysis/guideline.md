---
id: choose-small-multiples-over-animation-for-trend-analysis
title: Choose small multiples instead of animation for temporal trend analysis
bibliography: references.bib
description: For trend analysis over ordered time, prefer a small multiples layout
  on multidimensional scatter views to improve fidelity and mitigate tracking and
  replay errors for analysts.
labels:
- purpose:select
- basis:empirical
- task:trend
- time:ordered-time
- structure:small-multiples:use
- structure:single-view:avoid
- quality:fidelity:use
- lever:layout-structure
- audience:analyst
---

## Split temporal traces into separate panels <!-- role: advice -->

Choose a small multiples layout instead of a single animated view when analysts must find anomalies in temporal multivariate data. For example, give each item its own shared-axis panel rather than asking analysts to track many moving bubbles in one animated bubble chart.

## Separate panels remove replay and overlap burdens <!-- role: reason -->

Small multiples remove motion tracking from the task and let readers inspect each item's path directly. That makes anomalies visible without repeated playback and reduces the overlap that hides counter-trends in one shared animated view.

**Mechanism:** Separate panels turn a moving tracking task into a static comparison task, so analysts can inspect paths directly instead of replaying motion to recover what happened.

**Evidence:** In analysis tasks, small multiples were significantly faster than animation and significantly more accurate, and participants also judged small multiples less cluttered than animation on large datasets [@robertsonEffectivenessAnimationTrend2008].

**Notes:** The paper also notes that small multiples can require serial scanning across many panels.

## Use when analysts must inspect many item-level trends <!-- role: context -->

- **User Goal:** Find anomalies or counter-trends in unfamiliar data.
- **Task:** Analysis rather than passive presentation.
- **Data:** Many item-level trends changing over time in more than one visual dimension.
- **Chart Setting:** A scatter or bubble view is being used to show temporal movement, and no presenter is directing attention.
- **Audience:** Analysts exploring data on their own.
- **Success Criterion:** Higher answer accuracy with less time spent replaying or tracking motion.

## Do not use when the job is a fast passive walkthrough <!-- role: exceptions -->

**Break it when:** The primary job is a passive presentation and fast audience response matters more than accuracy. **Why:** Animation was the fastest condition in presentation mode and was judged more enjoyable and exciting.

## Tradeoffs of separate panels <!-- role: costs -->

**Sacrifice:** You give up one compact moving overview.
**Risk:** Readers may need to scan across many panels to answer some questions.
**Mitigation:** Use the small multiples view for analysis, then make a separate presentation view if you need a narrated walkthrough.

## Common failure around separate panels <!-- role: mistakes -->

**Mistake:** Keeping all items in one animated panel and expecting anomalies to pop out during analysis. **Why it fails:** Analysts must replay the motion and still lose track of moving points.

## How to test the layout choice <!-- role: check -->

**Failure Sign:** Analysts replay the animation several times or report losing track of points.
**Quick Check:** Run one representative analysis task once with the animated view and once with the small multiples view; if the animated view takes longer or misses anomalies, keep the small multiples layout.
**Stronger Test:** Verify that the answer can be found from the static panel grid without replay.

## What to change <!-- role: fix -->

- Split each item's temporal path into its own panel.
- Keep the axes shared across panels so paths stay comparable.
- Replace the single animated analysis view with the panel grid for exploration.
- If you still need a presentation view afterward, build a separate animated version for the walkthrough.
