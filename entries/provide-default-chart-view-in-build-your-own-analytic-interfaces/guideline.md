---
id: provide-default-chart-view-in-build-your-own-analytic-interfaces
title: Provide a default chart view in build-your-own analytic interfaces
bibliography: references.bib
description: For build-your-own analytic tasks, use a default, opinionated starting
  view on chart-building interfaces to improve accessibility and mitigate from-scratch
  chart assembly for users with cognitive and intersecting access needs.
labels:
- purpose:refine
- basis:accessibility
- task:compose
- quality:accessibility
- lever:interaction-access
- communication:workflow
- needs:cognitive
---

## Default starting view <!-- role: advice -->

Provide a default, opinionated chart view whenever users must assemble a chart by combining variables themselves. For example, open the analytic interface with a prebuilt chart already populated from the data instead of an empty builder that requires users to choose all variables before seeing any view.

## Why the default starting view works <!-- role: reason -->

A default chart view removes the blank-start step from analytic exploration. Users can begin by reading and adjusting an existing view instead of first having to construct the entire view themselves.

**Mechanism:** A populated starting view reduces the cognitive and functional labor of first use because the user does not need to perform the initial variable-combination work before any chart appears.

**Evidence:** Chartability defines this as an Assistive heuristic and states that when users must craft their own chart by combining variables in an analytic environment, a default, opinionated view should be provided as a starting point because build-your-own analytical experiences are difficult from a cognitive perspective, especially when other access needs intersect [@elavskyHowAccessibleMy2022].

**Notes:** The source treats this as community practice rather than a critical failure.

## Use when a chart builder starts blank <!-- role: context -->

- **User Goal:** Begin exploring or analyzing data in an interface that lets the user assemble a chart.
- **Task:** Choose or combine variables to define the chart view.
- **Chart Setting:** The first screen is a build-your-own analytic environment rather than a single prepared visualization.
- **Audience:** Users with disabilities, especially users facing cognitive load and intersecting access needs.
- **Success Criterion:** Users can start from a ready-made view and then modify it.

## Do not use this as a blanket rule outside build-your-own starts <!-- role: exceptions -->

**Break it when:** The interface does not require users to assemble a chart themselves as the starting state. **Why:** This guideline only addresses the blank-start burden of build-your-own analytic experiences.

## Tradeoffs of an opinionated starting view <!-- role: costs -->

**Sacrifice:** The interface no longer starts as a fully blank, user-defined workspace.
**Risk:** A nominal default that still leaves the core chart fields empty does not reduce the initial setup work.
**Mitigation:** Make the default a populated chart view that users can modify after it appears.

## Common blank-start failure <!-- role: mistakes -->

**Mistake:** Showing only an empty chart builder or variable picker as the initial state. **Why it fails:** Users still have to do the initial composition work before they can see any chart.

## How to review the starting state <!-- role: check -->

**Failure Sign:** A fresh load shows controls for choosing variables but no actual chart view.
**Quick Check:** Open the interface without prior selections; if users must combine variables before any chart appears, it fails.
**Stronger Test:** Verify that the first visible state is a populated chart that can be edited, not just configured.

## How to fix a blank chart builder <!-- role: fix -->

- Set the initial screen to a populated, opinionated chart view.
- Preselect the variables needed for that first view instead of leaving the chart fields empty.
- Let users revise the default view after it appears rather than making them construct the first view from scratch.
