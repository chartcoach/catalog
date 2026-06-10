---
id: add-one-suggested-variable-at-a-time-beyond-the-current-selection
title: Add one suggested variable at a time beyond the current selection
bibliography: references.bib
description: For early exploration of previously unseen tabular data, use one-variable-ahead
  suggested views in a multi-view recommendation gallery to improve coverage of overlooked
  relationships and address exact-match-only browsing for analysts.
labels:
- purpose:refine
- basis:empirical
- structure:multi-view
- data:tabular
- quality:insight:use
- lever:interaction-access
- audience:analyst
---

## Suggested-variable views <!-- role: advice -->

Add suggested views that append exactly one non-selected variable to the current selection. For example, keep exact-match views for the selected variables and a separate suggestion section that shows charts with one added field beyond the current selection.

## Why one-variable-ahead suggestions help <!-- role: reason -->

Small recommendation steps widen the search space without fully disconnecting the results from the analyst's current intent. They surface relevant relationships the analyst did not explicitly ask for while keeping the gallery understandable.

**Mechanism:** Adding one extra variable preserves the current context, so analysts can broaden exploration without losing track of what they selected.

**Evidence:** In the study, 124 of 179 bookmarked views in the recommendation browser included a variable that had been automatically added by the system. Most participants also rated the inclusion of additional non-selected variables as helpful or very helpful [@wongsuphasawatVoyagerExploratoryAnalysis2016].

## Use when selected variables should lead to nearby discoveries <!-- role: context -->

- **User Goal:** Broaden exploration from a current variable choice without jumping to unrelated views.
- **Task:** Explore relationships around one or more selected variables.
- **Data:** Multivariate tabular data with more variables than can be inspected one by one.
- **Chart Setting:** Multi-view recommendation gallery that can show both exact matches and suggestions.
- **Audience:** Analysts who are still forming questions.
- **Success Criterion:** Analysts save or pursue views that include useful non-selected variables.

## Do not use when the view must stay limited to the chosen fields <!-- role: exceptions -->

**Break it when:** The task is a focused follow-up question that should stay restricted to only the analyst's chosen variables. **Why:** Extra suggested variables are less aligned with targeted question answering, where users preferred direct manual specification.

## Tradeoffs of added-variable suggestions <!-- role: costs -->

**Sacrifice:** You give up tighter relevance to only the currently selected fields.
**Risk:** Added-variable views can pull attention away from the exact-match views.
**Mitigation:** Separate exact-match views from suggestion views so the analyst can distinguish them at a glance.

## Common failure mode: exact-match-only recommendations <!-- role: mistakes -->

**Mistake:** Show only views that exactly match the current variable selection. **Why it fails:** Analysts are more likely to miss useful relationships in variables they did not think to select.

## Check whether suggestions are doing useful work <!-- role: check -->

**Failure Sign:** Nearly all saved or expanded views use only the originally selected variables.
**Quick Check:** Review a sample of bookmarks or expansions and check whether analysts actually keep views with added variables.
**Stronger Test:** Compare sessions with and without added-variable suggestions and count how many saved views include a suggested field.

## Fix the suggestion logic <!-- role: fix -->

- Append one extra variable to each suggested view instead of changing many variables at once.
- Separate exact-match views from suggestion views in the gallery.
- Let analysts exclude variables they do not want the suggestion system to add.
