---
id: use-a-single-view-specification-workspace-for-targeted-follow-up-questions
title: Use a single-view specification workspace for targeted follow-up questions
bibliography: references.bib
description: For targeted follow-up analysis of tabular data, prefer a single-view
  specification workspace over a multi-view recommendation gallery to improve focused
  question answering and address cumbersome scanning for analysts.
labels:
- purpose:select
- basis:empirical
- structure:single-view:use
- structure:multi-view:avoid
- data:tabular
- quality:insight:use
- lever:layout-structure
- audience:analyst
---

## Manual specification workspace <!-- role: advice -->

Choose a single-view specification workspace when the analyst already has a specific follow-up question. For example, let the analyst directly place variables onto encoding shelves and change transformations or mark type on one chosen view instead of scanning a gallery of suggestions.

## Why direct specification works for focused questions <!-- role: reason -->

Once the question is precise, direct control becomes more valuable than breadth. A single-view workspace lets the analyst act on the intended variables and encodings without the extra step of browsing many alternatives.

**Mechanism:** Direct manipulation reduces indirection when the analyst already knows what relationship, summary, or transformation to inspect.

**Evidence:** In the study, participants overwhelmingly preferred the manual specification tool for question answering, and participants described the recommendation browser as good for exploration but cumbersome for specific tasks [@wongsuphasawatVoyagerExploratoryAnalysis2016].

## Use when the follow-up question is already formed <!-- role: context -->

- **User Goal:** Answer a specific question about the data.
- **Task:** Targeted follow-up analysis after an initial overview or after a promising view has been found.
- **Data:** Tabular data where the relevant variables are already known or suspected.
- **Chart Setting:** Interactive environment that can expose direct controls for encodings and transformations.
- **Audience:** Analysts refining one view to answer a precise question.
- **Success Criterion:** The analyst can quickly construct and revise one relevant chart.

## Do not use when the analyst still needs broad coverage <!-- role: exceptions -->

**Break it when:** The analyst does not yet know which variables to inspect and needs a broad first pass through the dataset. **Why:** The study found that the multi-view recommendation gallery produced much wider variable coverage and was preferred for exploration.

## Tradeoffs of a single-view workspace <!-- role: costs -->

**Sacrifice:** You give up automatic breadth across many variable combinations.
**Risk:** Analysts can fixate early on a small subset of variables.
**Mitigation:** Start with broad exploration or return to it when the current question is answered.

## Common failure mode: staying in browse mode too long <!-- role: mistakes -->

**Mistake:** Keep analysts in a recommendation gallery after they can already state the exact follow-up question. **Why it fails:** Browsing suggestions becomes extra work when the task is to refine one specific view.

## Check whether the structure should switch <!-- role: check -->

**Failure Sign:** Users can name the exact variables or relationship they need before they start acting.
**Quick Check:** Compare a single-view specification workspace against a recommendation gallery on the same focused question and see which one reaches a satisfactory chart with less browsing.
**Stronger Test:** Ask users which structure they prefer for the focused task and switch when the single-view workspace is preferred.

## Fix the follow-up workflow <!-- role: fix -->

- Add direct controls for assigning variables to visual encodings on one active view.
- Let analysts change transformations and mark type directly on that view.
- Move from the gallery into the single-view workspace once a specific follow-up question is formed.
