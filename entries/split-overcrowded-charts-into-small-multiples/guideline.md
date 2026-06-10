---
id: split-overcrowded-charts-into-small-multiples
title: Split an overcrowded chart into small multiples
bibliography: references.bib
description: For pattern reading in dense displays, prefer a small-multiples layout
  on charts where too many elements compete for the same space to improve accessibility
  and mitigate overcrowded single-view displays for people with cognitive needs.
labels:
- purpose:select
- basis:accessibility
- structure:small-multiples:use
- structure:single-view:avoid
- quality:accessibility:use
- lever:layout-structure
- density:dense
- needs:cognitive
---

## Switch to small multiples <!-- role: advice -->

Use a small-multiples layout instead of one crowded view when too many elements compete for the same space. For example, divide a dense chart into smaller charts with less data in each panel so the remaining density preserves the signal instead of forcing all marks into one panel.

## Why smaller panels reduce labor <!-- role: reason -->

A crowded single view makes readers separate signal from competition in the same space. Smaller panels lower the number of elements that must be processed at once while still allowing dense data to be shown when that density is meaningful.

**Mechanism:** Dividing one overloaded display into multiple smaller displays reduces cognitive and functional labor by limiting direct mark competition within each view.

**Evidence:** Chartability marks inappropriate data density as a critical Assistive issue and recommends dividing a chart into smaller charts with less data when too many elements compete for one space. The linked references also support preserving signal without forcing all detail into one overloaded display, using grouped views or summary structures to reduce visual noise [@elavskyHowAccessibleMy2022; @stackoverflow_stop_aggregating; @had_bin-summarize-smooth_framework].

**Notes:** Dense views are not automatically wrong; density can be kept when it serves the data's signal.

## Use when a single view is overcrowded <!-- role: context -->

- **User Goal:** Find or explain a cluster, pattern, or lack of pattern.
- **Data:** Many elements compete for the same space.
- **Chart Setting:** One chart has become visually dense or crowded.
- **Audience:** Readers whose cognitive labor should be reduced, including people with cognitive needs.
- **Success Criterion:** The pattern remains visible with less effort in each view.

## Do not split when density is the signal <!-- role: exceptions -->

**Break it when:** The dense single view is needed to retain the data's signal and the clustering, pattern, or lack of pattern is explicitly explained. **Why:** In that case the density serves a purpose rather than creating unnecessary labor.

## Tradeoffs of splitting the view <!-- role: costs -->

**Sacrifice:** You give up one shared panel containing all elements at once.\
**Risk:** Splitting the view can weaken the signal if the important pattern depends on the full dense view.\
**Mitigation:** Keep the dense view only when that density is purposeful and explain the pattern directly.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keep every element in one panel after the marks start competing for the same space. **Why it fails:** Readers must do extra work to separate the pattern from the crowding.

## Check whether the layout should be split <!-- role: check -->

**Failure Sign:** Too many elements compete for the same space in the single-view version.\
**Quick Check:** Compare the crowded single view with a version split into smaller charts with less data per panel; if the split version shows the pattern with less competition, use small multiples.\
**Stronger Test:** If you keep the single view, verify that its density serves a stated purpose and that the clustering, pattern, or lack of pattern is explained.

## Fix the overcrowded view <!-- role: fix -->

- Divide the crowded chart into smaller charts with less data in each chart.
- Reduce the amount of data shown in each panel until the remaining density serves a clear purpose.
- If you keep a dense single view to preserve signal, add an explicit explanation of the clustering, pattern, or lack of pattern.
