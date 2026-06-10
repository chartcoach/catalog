---
id: use-color-not-shape-for-scatterplot-mean-comparisons
title: Use color rather than shape to encode groups for scatterplot mean comparisons
bibliography: references.bib
description: For comparing group averages, prefer color encoding over shape encoding
  for group membership on scatterplots to improve fidelity and mitigate misreading
  of mean position for overview readers.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:scatter
- quality:fidelity
- lever:encoding
- channel:color-hue:use
- channel:shape:avoid
---

## Group encoding for mean comparison <!-- role: advice -->

Encode scatterplot groups with color when readers must compare their average position. For example, use two colors rather than circles versus triangles when the task is to judge which class sits higher on average.

## Why color helps class-average judgments <!-- role: reason -->

Readers first need to isolate the members of each class before they can estimate each class mean.

**Mechanism:** Color supports faster class selection in a scatterplot, which improves ensemble judgments about average position across the selected members.

**Evidence:** The paper reports a multiclass scatterplot study in which viewers compared mean position more accurately when groups were distinguished by color than when they were distinguished by shape; adding redundant color-plus-shape cues did not improve performance [@szafirFourTypesEnsemble2016].

**Notes:** The same study also found that adding more distractor classes did not impair these mean judgments in the way classic visual-search results might suggest.

## Use when marker appearance carries group identity <!-- role: context -->

- **User Goal:** Compare which group has the higher or lower average position.
- **Task:** Estimate or compare mean position between plotted classes.
- **Data:** Quantitative x/y values plus categorical group membership.
- **Chart Setting:** A scatterplot distinguishes classes by marker appearance.
- **Success Criterion:** Readers can accurately compare group means without tracing individual points one by one.

## Do not use outside this encoding choice <!-- role: exceptions -->

**Break it when:** Group identity is not being encoded by marker appearance in the scatterplot. **Why:** The reported advantage is specifically a choice between color and shape markers for mean-position judgments.

## Tradeoffs of color group encoding <!-- role: costs -->

**Sacrifice:** You should not expect extra accuracy from adding redundant shape coding just for this task.\
**Risk:** Relying on shape alone lowers accuracy for mean-position comparison.\
**Mitigation:** Keep color as the primary group code when average position is the intended readout.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Switching groups from color to shape in a scatterplot that is meant to support mean comparison. **Why it fails:** Shape coding performed worse than color for this specific judgment.

## Check the group encoding choice <!-- role: check -->

**Failure Sign:** Reviewers struggle to say which class is higher on average even though both classes are visible.\
**Quick Check:** Create color-coded and shape-coded versions of the same scatterplot and ask the same mean-position question on both; keep the color-coded version if answers are cleaner.\
**Stronger Test:** Compare accuracy on representative mean-position questions before and after the encoding change.

## Fix the encoding <!-- role: fix -->

- Replace shape-only group coding with color coding for the compared classes.
- Drop redundant shape coding if it was added only to improve this mean-comparison task.
- Keep shape from becoming the sole group identifier when the chart’s job is comparing class averages.
