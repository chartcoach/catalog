---
id: add-settle-to-group-before-comparing-scattered-risk-arrays
title: Add a settle-to-group transition before comparing scattered risk arrays
bibliography: references.bib
description: For compare tasks on scattered icon-array risk graphics, use a settle-to-group
  transition on multi-view risk displays to improve magnitude judgments and mitigate
  the poor accuracy of scattered-only layouts for mixed-numeracy audiences.
labels:
- purpose:refine
- basis:empirical
- task:compare
- structure:multi-view
- quality:fidelity
- lever:interaction-access
- temporal-pattern:dynamic
- knowledge:mixed
---

## Add a settle-to-group step <!-- role: advice -->

If you begin with a scattered risk array, animate the event icons into a grouped block before the reader makes the comparison. For example, let colored event units settle to the bottom of each array after the scattered view, whether or not the events were also revealed one at a time.

## Why settling improves a scattered display <!-- role: reason -->

A grouped end state restores an easier magnitude readout after the display has shown randomness. This lets readers see the random distribution cue first without leaving them to compare two scattered patterns at decision time.

**Mechanism:** The settle transition keeps the initial randomness cue but replaces the hard-to-read scattered arrangement with a final grouped arrangement that supports direct magnitude comparison.

**Evidence:** Scattered displays performed particularly poorly unless they included the settle animation that let users view grouped event icons, but these settle variants still did not outperform displays that started grouped [@zikmund-fisherAnimatedGraphicsComparing2012].

## Use when you must show randomness first <!-- role: context -->

- **User Goal:** Compare two options accurately after first seeing that events are randomly distributed.
- **Task:** Make a side-by-side risk comparison from icon arrays that begin in scattered form.
- **Data:** Quantitative event rates shown in two parallel risk arrays.
- **Chart Setting:** Animated risk pictographs where the design intentionally starts with scattered event positions.
- **Audience:** Adults with mixed numeracy.
- **Success Criterion:** Better treatment choice and gist knowledge than a scattered-only version.

## Do not add this transition when the random start is unnecessary <!-- role: exceptions -->

**Break it when:** The display does not need an initial scattered view to communicate randomness. **Why:** Starting grouped performed as well or better, so the extra motion adds complexity without a demonstrated gain.

## Costs of the settle transition <!-- role: costs -->

**Sacrifice:** You add one more motion step and more viewing time.
**Risk:** The transition can still be less effective than simply starting with a grouped display.
**Mitigation:** Use the settle step only when the scattered opening has a specific communication role.

## Common scattered-only failure <!-- role: mistakes -->

**Mistake:** Showing a scattered event layout and leaving it scattered at the moment of comparison. **Why it fails:** Scattered-only versions were among the poorest performers.

## Verify that the grouped end state is what users compare <!-- role: check -->

**Failure Sign:** The comparison question appears while the icons are still scattered.
**Quick Check:** Confirm that every scattered version ends with the affected icons visibly grouped before the user answers.
**Stronger Test:** Compare the scattered-only and scatter-plus-settle versions on the same values and keep the one with better choice and knowledge accuracy.

## Resolve the scattered view into a readable comparison view <!-- role: fix -->

- Add a settle animation that moves all event icons into one grouped block.
- Keep the grouped end state visible while the reader makes the decision.
- Remove any design that returns the icons to a scattered state before response.
- If the scattered introduction is not needed, delete it and start with the grouped display.
