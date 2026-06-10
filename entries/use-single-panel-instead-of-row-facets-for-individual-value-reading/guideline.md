---
id: use-single-panel-instead-of-row-facets-for-individual-value-reading
title: Use a single panel instead of row facets for individual-value reading
bibliography: references.bib
description: For exact value lookup and pairwise comparison, prefer a single-panel
  layout on point-based multivariate views to improve fidelity and mitigate slow cross-panel
  scanning for readers inspecting individual values.
labels:
- purpose:select
- basis:empirical
- quality:fidelity:use
- lever:layout-structure
- operator:lookup
- reading-mode:exact
- structure:single-view:use
- structure:small-multiples:avoid
---

## Keep individual-value tasks in one panel <!-- role: advice -->

Use one panel instead of stacked row facets when readers must read or compare individual values quickly. For example, keep the category field in a single view rather than splitting the plot into row facets when the task is exact lookup or pairwise value comparison.

## Why a single panel is faster here <!-- role: reason -->

Row facets add cross-panel scanning and can force scrolling, which slows simple value-reading tasks. The single-panel versions avoided that penalty while maintaining better performance on these tasks.

**Mechanism:** A single panel keeps the comparison in one visual frame, while row facets require the reader to move between panels and sometimes scroll to see the needed scale.

**Evidence:** In the experiment, row-faceted point plots were notably slower than single-view alternatives for value tasks, and the paper attributes this slowdown to comparing across multiple charts and scrolling to offscreen elements [@zengReviewCollationGraphical2023; @kimAssessingEffectsTask2018].

## Use when all values must be read directly <!-- role: context -->

- **User Goal:** Read exact values or decide which of two points is larger or smaller.
- **Task:** Individual-value lookup or pairwise comparison.
- **Data:** One categorical field and two quantitative fields shown in a point-based view.
- **Chart Setting:** A row-faceted layout is being considered for the category field.
- **Success Criterion:** Faster answers without losing accuracy on individual-value questions.

## Do not use this as a dense-summary default <!-- role: exceptions -->

**Break it when:** The task is a group summary task and the display has many categories or heavy overplotting. **Why:** Under dense summary conditions, row facets can recover accuracy that single-view displays lose to congestion.

## What you give up <!-- role: costs -->

**Sacrifice:** You lose the separation that row facets provide between categories.
**Risk:** A single panel can become congested as category count or point count grows.
**Mitigation:** Use the single-panel form when individual-value reading is the main task and visual congestion is still manageable.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Split a point plot into row facets even though the reader only needs to read or compare individual values. **Why it fails:** The extra panel-to-panel scanning slows the task without providing the main benefit that facets offer in dense summary situations.

## Test the layout choice head-to-head <!-- role: check -->

**Failure Sign:** Readers must move between panels or scroll before answering simple value questions.
**Quick Check:** Compare the row-faceted version against a single-panel version on one exact lookup question and one pairwise comparison question.
**Stronger Test:** Time both versions on a small set of representative individual-value tasks and choose the faster one that preserves accuracy.

## Remove the facet split <!-- role: fix -->

- Move the category field out of the row facet.
- Keep the points in one panel for the individual-value task.
- Re-check congestion only after the panel is collapsed back into a single view.
