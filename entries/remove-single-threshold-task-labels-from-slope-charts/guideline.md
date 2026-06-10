---
id: remove-single-threshold-task-labels-from-slope-charts
title: Remove single-threshold task labels from slope charts
bibliography: references.bib
description: For grouped-result comparison of search-task slopes, avoid threshold
  annotations on slope charts to prevent false task classification and mitigate slope-only
  misinterpretation for domain experts.
labels:
- purpose:refine
- basis:empirical
- task:compare
- scope:grouped-result
- quality:fidelity
- lever:text-annotation
- communication:framing
- component:annotation:avoid
---

## Delete the cutoff label <!-- role: advice -->

Remove any single cutoff that classifies slope magnitude into search types. For example, do not mark about 10 ms/item as a decisive divide between “parallel” and “serial” on slope histograms or RT × set size summaries.

## Why slope cutoffs mislead <!-- role: reason -->

A cutoff annotation suggests that the data naturally split into distinct task classes and that slope alone is enough to identify them. The paper shows that neither assumption holds.

**Mechanism:** Removing the cutoff prevents readers from making an unsupported reverse inference from one slope value to a search type.

**Evidence:** The paper reports a unimodal overall slope distribution with no evidence for a bimodal serial-parallel split, and it shows that feature, conjunction, and spatial-configuration slope distributions overlap substantially [@wolfeWhatCan11998].

**Notes:** The paper specifically calls the common 10 ms/item divide a myth and advises skepticism toward claims that classify a task from slope magnitude alone.

## Use when a slope chart could imply a category <!-- role: context -->

- **User Goal:** Compare or label different search-task types.
- **Task:** Present slope results without implying an unsupported serial-parallel split.
- **Data:** Slopes from multiple tasks, groups, or conditions that could be compared on one scale.
- **Chart Setting:** A histogram, grouped slope summary, or any slope chart where a reference cutoff could be drawn.
- **Audience:** Researchers or analysts reading visual-search figures.
- **Success Criterion:** Readers do not infer task class from a single threshold on slope magnitude.

## Do not use when no category claim is being made <!-- role: exceptions -->

**Break it when:** The figure only reports relative search efficiency and does not claim that slope alone determines task type. **Why:** The paper says slope differences still matter for explaining why some searches are easier than others.

## Tradeoffs of removing the cutoff <!-- role: costs -->

**Sacrifice:** You lose a simple one-line classifier.
**Risk:** Readers may still look for a shorthand category boundary.
**Mitigation:** Replace the cutoff with direct class comparisons using distributions or slope ratios.

## Common threshold failure <!-- role: mistakes -->

**Mistake:** Add a reference line or caption that treats one slope value as the boundary between task types. **Why it fails:** The underlying slope distributions overlap, so values on either side of the line can come from different task classes.

## How to test the cutoff claim <!-- role: check -->

**Failure Sign:** The figure includes one slope cutoff and a categorical interpretation built on it.
**Quick Check:** Remove the cutoff mentally and ask whether the classification claim still follows from the remaining plot.
**Stronger Test:** Compare the task-class distributions directly; if they overlap, the cutoff annotation is unsupported.

## Edits that replace the cutoff <!-- role: fix -->

- Delete the slope cutoff line and any label that names values below or above it as distinct task types.
- Rewrite the title or caption to describe slope as a continuous measure of efficiency rather than a categorical classifier.
- Add an overlapping distribution view or a slope-ratio view if the figure still needs to support task comparison.
