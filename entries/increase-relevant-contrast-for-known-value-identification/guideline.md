---
id: increase-relevant-contrast-for-known-value-identification
title: Increase target-defining contrast for known-value identification
bibliography: references.bib
description: For known-value target lookup, use strong task-relevant feature contrast
  on feature-coded displays to improve fidelity and mitigate distractor interference
  for readers doing lookup.
labels:
- purpose:refine
- basis:empirical
- task:retrieve
- quality:fidelity
- lever:encoding
- reading-mode:lookup
---

## Target-defining contrast <!-- role: advice -->

Increase perceptual distance on the feature that defines the target, and keep irrelevant encodings visually similar. For example, make the sought class clearly different in color or shape, and avoid unnecessary variation among distractors on features that do not matter to the search.

## Why strong relevant contrast works <!-- role: reason -->

Known-value identification depends on how easily the target set can be separated from surrounding non-targets.

**Mechanism:** Large differences on the task-relevant feature make the target easier to isolate, while irrelevant feature variation adds distractor diversity and makes the search noisier.

**Evidence:** The paper summarizes visual-search results showing that single-target search becomes harder when the target is more similar to distractors and when distractors are more diverse, and it turns this into a visualization guideline: maximize perceptual distance on task-relevant features and minimize differences on task-irrelevant ones [@szafirFourTypesEnsemble2016].

## Use when the target value is known in advance <!-- role: context -->

- **User Goal:** Find all points that match a specified value.
- **Task:** Identify marks by a known feature such as color, shape, size, or a spatial region.
- **Chart Setting:** A feature-coded display contains target and distractor marks at the same time.
- **Audience:** Readers are doing lookup rather than open-ended exploration.
- **Success Criterion:** The target set is isolated quickly and accurately.

## Do not use for location-only selection <!-- role: exceptions -->

**Break it when:** The reader must select points mainly by their locations rather than by a visual feature. **Why:** The relevant limit then becomes selection of multiple locations, not contrast between target and distractor features.

## Tradeoffs of stronger target contrast <!-- role: costs -->

**Sacrifice:** Irrelevant visual variety has to be reduced.\
**Risk:** Extra differences among distractors slow the search instead of helping it.\
**Mitigation:** Reserve the strongest visual differences for the feature that defines the target.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Adding more visual variation to distractors in the hope that the target will stand out anyway. **Why it fails:** Greater distractor diversity makes feature-based identification harder.

## Check searchability <!-- role: check -->

**Failure Sign:** Reviewers know the target feature but still search point by point.\
**Quick Check:** Increase the target–distractor difference and mute irrelevant variation on a test version; if the target set becomes easier to isolate immediately, keep the revision.\
**Stronger Test:** Time representative target-finding tasks before and after the change.

## Fix the encoding <!-- role: fix -->

- Make the target-defining feature more distinct from non-target features.
- Remove or mute variation on features that are irrelevant to the lookup task.
