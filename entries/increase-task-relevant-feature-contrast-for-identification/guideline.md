---
id: increase-task-relevant-feature-contrast-for-identification
title: Increase perceptual contrast on task-relevant features for identification tasks
bibliography: references.bib
description: For lookup tasks, use stronger perceptual separation on the features
  that define the target subset in feature-coded views to improve fidelity and mitigate
  missed or slow target detection for viewers scanning a display.
labels:
- purpose:refine
- basis:empirical
- quality:fidelity:use
- lever:encoding
- reading-mode:lookup
---

## Increase relevant feature contrast <!-- role: advice -->

Increase the perceptual distance between the features that define the target subset, and keep differences on task-irrelevant features small. For example, make the sought subset stand farther apart in color, shape, or size, and avoid adding extra variation on other channels when that variation does not help the identification task.

## Why stronger relevant contrast helps identification <!-- role: reason -->

Identification by feature works best when the display makes the target-defining feature easy to separate from distractors across the whole view. Extra variation on irrelevant features competes with that separation and makes the subset harder to isolate quickly.

**Mechanism:** Stronger task-relevant separation supports broad feature-based selection, while smaller task-irrelevant differences reduce distraction from nonessential variation.

**Evidence:** The review collates this paper as covering retrieval, extrema, anomalies, aggregation, clustering, and correlation tasks. Within its identification discussion, the paper states that designers should maximize perceptual distance among features that delineate task-relevant properties and minimize differences on irrelevant features to support identification in visualizations [@zengReviewCollationGraphical2023; @szafirFourTypesEnsemble2016].

## Use when feature-based selection is the real job <!-- role: context -->

- **User Goal:** Find all marks matching a known value or detect a visually distinct subset.
- **Task:** Identify a subset by feature rather than by reading every item.
- **Chart Setting:** Displays where data classes are encoded with visual features such as color, shape, or size.
- **Success Criterion:** Faster and more accurate isolation of the intended subset.

## Do not rely on this when the subset is location-defined <!-- role: exceptions -->

**Break it when:** The subset must be selected by location instead of by visual feature. **Why:** The paper explicitly distinguishes cases where points cannot be selected easily by feature and must instead be selected by their locations.

## Tradeoffs of stronger relevant contrast <!-- role: costs -->

**Sacrifice:** You give up freedom to vary irrelevant features independently.
**Risk:** Extra variation on irrelevant features can compete with the target-defining feature and weaken selection.
**Mitigation:** Keep nonessential channels visually quieter than the channel that carries the identification task.

## Common failure with feature contrast <!-- role: mistakes -->

**Mistake:** Highlighting the target feature while also introducing large differences on unrelated features. **Why it fails:** The display no longer isolates the feature that should drive selection.

## Check whether the target subset pops out <!-- role: check -->

**Failure Sign:** Reviewers hesitate, disagree, or miss items when asked to find the target subset.
**Quick Check:** Compare the current view with a version that increases separation on the target-defining feature and reduces irrelevant variation.
**Stronger Test:** Ask reviewers to find all target items in both versions and note which version yields faster agreement.

## Fix the feature contrast <!-- role: fix -->

- Increase separation on the single feature that defines the target subset.
- Reduce variation on features that are not needed for the identification task.
