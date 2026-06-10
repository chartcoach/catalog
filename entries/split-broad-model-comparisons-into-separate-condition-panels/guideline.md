---
id: split-broad-model-comparisons-into-separate-condition-panels
title: Split broad model comparisons into separate condition panels
bibliography: references.bib
description: For grouped-result method comparisons spanning several datasets or evaluation
  scores, prefer a multi-view structure over a single aggregate ranking to improve
  insight and mitigate hidden rank reversals for analysts.
labels:
- purpose:select
- basis:empirical
- task:compare
- scope:grouped-result
- structure:multi-view:use
- structure:single-view:avoid
- quality:insight:use
- lever:layout-structure
---

## Condition-separated panels <!-- role: advice -->

Split a broad method comparison into separate panels for each dataset and each score instead of collapsing everything into one overall ranking. For example, show one ranking for each image dataset, one for each video dataset, and separate score panels for CC, NSS, and shuffled AUC when the same models change order across conditions.

## Why separate panels reveal the real comparison <!-- role: reason -->

A single aggregate ranking hides where methods trade places. Separate panels show both the stable leaders and the conditions that change the story.

**Mechanism:** Condition-separated panels make rank shifts visible, so readers can see whether a method is consistently strong or only strong on a particular dataset or score.

**Evidence:** The paper finds that model rankings vary across datasets and evaluation scores, and argues that fair evaluation requires comparison over several datasets because dataset statistics differ and one-score comparisons are hard to interpret directly [@borjiQuantitativeAnalysisHumanModel2013].

## Use when one comparison spans many conditions <!-- role: context -->

- **User Goal:** Summarize the state of the art without hiding condition-specific behavior.
- **Task:** Compare many models across several benchmarks or scoring methods.
- **Data:** Multiple image datasets, video datasets, or multiple evaluation scores for the same models.
- **Chart Setting:** Benchmark figures, review tables, or leaderboard graphics.
- **Audience:** Analysts and reviewers assessing relative performance.
- **Success Criterion:** Readers can see both overall strength and condition-dependent reversals.

## Do not use it when the study is intentionally single-condition <!-- role: exceptions -->

**Break it when:** The comparison is intentionally restricted to one stimulus family and one task-specific score. **Why:** The paper uses a single NSS view for synthetic odd-target displays because that one score matches that one evaluation goal.

## What this costs <!-- role: costs -->

**Sacrifice:** The figure takes more space and is slower to scan at first glance.
**Risk:** Too many panels can bury the main result.
**Mitigation:** Keep each panel to one condition and reserve any overall summary for after the per-condition views.

## Common layout failure <!-- role: mistakes -->

**Mistake:** Collapse several datasets and scores into one average rank. **Why it fails:** The combined view hides cases where models exchange positions across datasets or across scoring methods.

## How to decide between one panel and several <!-- role: check -->

**Failure Sign:** The same model moves noticeably up or down when you switch dataset or score.
**Quick Check:** Compare the top models across conditions before averaging; if the order changes, a single ranking is too coarse.
**Stronger Test:** Build a one-panel aggregate and a condition-separated multi-view; if the headline winner or ordering changes, keep the multi-view.

## What to change <!-- role: fix -->

- Create one panel per dataset instead of averaging datasets into one rank list.
- Create one panel per evaluation score instead of mixing scores into one summary ordering.
- Separate still-image and video results into distinct sections.
- Move any overall average to a secondary summary after the condition-specific panels.
