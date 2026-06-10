---
id: use-a-multi-view-slope-summary-for-task-classification
title: Use a multi-view slope summary for task classification
bibliography: references.bib
description: For grouped-result comparison of search-task classes, use a multi-view
  structure on slope summary figures to improve fidelity and mitigate false classification
  from slope magnitude alone for domain experts.
labels:
- purpose:select
- basis:empirical
- task:compare
- scope:grouped-result
- structure:multi-view:use
- structure:single-view:avoid
- quality:fidelity
- lever:layout-structure
---

## Add a second slope diagnostic <!-- role: advice -->

Use a multi-view summary instead of a single slope-only view when the figure is meant to classify or diagnose search tasks. For example, pair mean target-present and target-absent slopes with a target-absent-versus-target-present scatter or a slope-ratio panel rather than showing one average slope alone.

## Why two views classify better <!-- role: reason -->

A single slope view hides the fact that task classes overlap strongly on target-present slope while still differing in how target-absent trials behave. Adding a second view of the present-absent relationship exposes those task-specific differences.

**Mechanism:** A multi-view figure lets readers see both overall efficiency and the structure of unsuccessful-search termination, so they are less likely to mistake one slope value for a full task diagnosis.

**Evidence:** The paper shows that overall slope distributions are unimodal and overlapping, that different task types have different mean slopes, and that tasks with similar target-present slopes can still differ systematically in target-absent slopes and slope ratios [@wolfeWhatCan11998].

**Notes:** The paper explicitly argues that slopes and ratios together can support diagnostic comparisons better than slope magnitude alone.

## Use when task class is the question <!-- role: context -->

- **User Goal:** Classify a search task or compare how known task classes differ.
- **Task:** Distinguish whether a task behaves more like a feature, conjunction, or spatial-configuration search.
- **Data:** Target-present and target-absent slopes are both available across many observations or conditions.
- **Chart Setting:** A results figure or summary panel with room for more than one view.
- **Audience:** Researchers or analysts interpreting visual-search behavior.
- **Success Criterion:** Readers can see both slope overlap and task differences in target-absent behavior.

## Do not use when efficiency alone is enough <!-- role: exceptions -->

**Break it when:** The figure only needs to show that one search is easier or harder than another, without claiming a task category or a serial-parallel status. **Why:** The paper states that slope differences still convey search efficiency even when they cannot support categorical classification.

## Tradeoffs of multi-view slope summaries <!-- role: costs -->

**Sacrifice:** A multi-view summary uses more space than one slope panel.
**Risk:** The added diagnostic can still mislead if it relies on unstable raw ratios from very small target-present slopes.
**Mitigation:** Transform or restrict ratio views before adding them to the figure.

## Common single-view failure <!-- role: mistakes -->

**Mistake:** Use one slope panel as the entire argument for task classification. **Why it fails:** Tasks can overlap in target-present slope yet differ in target-absent slope and slope ratio.

## How to choose between one view and two <!-- role: check -->

**Failure Sign:** The figure supports a classification claim even though it only shows slope magnitude.
**Quick Check:** Ask whether the reader can see both target-present and target-absent behavior in the figure.
**Stronger Test:** Compare the single-view conclusion with a two-view version; if the added view changes the interpretation of task class, keep the multi-view design.

## Edits that add the missing diagnostic <!-- role: fix -->

- Add a scatter of target-absent slope versus target-present slope next to the main slope summary.
- Add a slope-ratio panel grouped by target-present slope range when task diagnosis depends on unsuccessful-search behavior.
- Keep a distribution view beside any mean-slope summary when you compare multiple task classes.
