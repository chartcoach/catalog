---
id: use-a-multi-view-recommendation-gallery-for-initial-exploration
title: Use a multi-view recommendation gallery for initial exploration
bibliography: references.bib
description: For early exploration of previously unseen tabular data, prefer a multi-view
  recommendation gallery over a single-view specification workspace to improve coverage
  of unique variable combinations and address narrow early exploration for analysts.
labels:
- purpose:select
- basis:empirical
- structure:multi-view:use
- structure:single-view:avoid
- data:tabular
- quality:insight:use
- lever:layout-structure
- audience:analyst
---

## Recommendation gallery <!-- role: advice -->

Choose a multi-view recommendation gallery when analysts first open an unfamiliar table and need broad coverage. For example, show many recommended charts for different variable sets at once instead of making the analyst construct one chart at a time in a single central workspace.

## Why the gallery works for early exploration <!-- role: reason -->

Seeing many candidate views at once broadens the search space during the first pass through unfamiliar data. It helps analysts encounter more distinct variable combinations without reducing how many interesting views they save.

**Mechanism:** A gallery exposes multiple variable sets in parallel, so the analyst can scan broadly before committing to one path of follow-up analysis.

**Evidence:** In a controlled study against a manual specification tool, the recommendation gallery exposed users to over three times as many unique variable sets and led them to interact with about 1.5 times more unique variable sets. Participants also overwhelmingly preferred the gallery for exploration, while bookmark counts were not significantly lower than with manual specification [@wongsuphasawatVoyagerExploratoryAnalysis2016].

## Use when exploration breadth matters <!-- role: context -->

- **User Goal:** Get a comprehensive first-pass sense of what an unfamiliar dataset contains.
- **Task:** Open-ended exploratory analysis before specific questions are settled.
- **Data:** Multivariate relational table with several possible variable combinations.
- **Chart Setting:** Interactive analysis environment with limited session time.
- **Audience:** Analysts exploring previously unseen data.
- **Success Criterion:** The analyst sees and engages with many distinct variable combinations.

## Do not use when the question is already specific <!-- role: exceptions -->

**Break it when:** The analyst can already state a precise follow-up question and needs to build or refine one view around it. **Why:** The study found that users preferred the manual specification workspace for targeted question answering.

## Tradeoffs of a gallery-first workflow <!-- role: costs -->

**Sacrifice:** You give up some direct control over the exact next chart to build.
**Risk:** Analysts may spend time scanning recommendations instead of refining one chosen view.
**Mitigation:** Let analysts save promising views and return to focused follow-up analysis after the broad scan.

## Common failure mode: one-chart-at-a-time exploration <!-- role: mistakes -->

**Mistake:** Keep the initial exploration workflow centered on a single chart-construction view. **Why it fails:** It narrows exposure to variable combinations during the stage when analysts still need broad coverage.

## Check whether the structure should switch <!-- role: check -->

**Failure Sign:** In a fixed exploration session, users only see or touch a small set of variable combinations.
**Quick Check:** Compare the gallery against a single-view specification workspace on the same dataset and count unique variable sets shown or interacted with.
**Stronger Test:** Under equal time limits, prefer the structure that increases variable-set coverage without reducing the number of views users save for follow-up.

## Fix the exploration structure <!-- role: fix -->

- Replace the single central chart-construction view with a gallery of recommended charts.
- Populate the gallery with views from different variable sets instead of only one view at a time.
- Keep a save or bookmark action so analysts can capture promising views before switching to deeper follow-up work.
