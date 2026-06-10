---
id: provide-visible-location-and-history-controls
title: Provide visible location and history controls
bibliography: references.bib
description: For navigation across complex interactive dashboard or app states, use
  visible location and history controls on visualization interfaces to improve accessibility
  and mitigate unclear current view and unrecoverable state changes for users with
  cognitive needs or assistive technologies.
labels:
- purpose:refine
- basis:accessibility
- structure:dashboard
- quality:accessibility
- lever:interaction-access
- communication:workflow
- needs:cognitive
---

## Location and history controls <!-- role: advice -->

Expose the current view and navigation state in complex visualization interfaces. For example, add breadcrumbs or step indicators for the active dashboard view, and provide save, reload, and back/forward history for the current visualization state.

## Why location and history controls help <!-- role: reason -->

Users can navigate more reliably when the interface tells them where they are and lets them recover a prior view instead of rebuilding it from memory. This reduces disorientation and makes the interaction more forgiving after errors or exploratory changes.

**Mechanism:** Visible location cues support orientation, and history or state recovery supports error tolerance and repeatable navigation.

**Evidence:** Chartability identifies unclear current location and state in complex dashboards or apps as an accessibility problem and recommends breadcrumbs together with save, reload, and history support so users can guide their path and recover prior states. [@elavskyHowAccessibleMy2022] Providing location information such as breadcrumbs or step indicators helps users understand their position within a set of pages, especially users with cognitive impairments or assistive technologies. [@w3c_understanding_location]

**Notes:** These features are most helpful when they are clearly communicated in the interface.

## When to add location and history controls <!-- role: context -->

- **User Goal:** Move through views or states without losing place.
- **Chart Setting:** A complex dashboard or app-based visualization with multiple views, steps, or state changes.
- **Audience:** Users with cognitive accessibility needs or assistive technologies.
- **Success Criterion:** Users can identify the current location and return to an earlier state without reconstructing it manually.

## When not to add location and history controls <!-- role: exceptions -->

**Break it when:** the visualization is a single static view with no multiple pages, steps, or revisitable states. **Why:** breadcrumbs, history, and save/load do not add meaningful location or recovery information in that situation.

## Tradeoffs of location and history controls <!-- role: costs -->

**Sacrifice:** The interface must devote visible space and interaction logic to location and history controls.\
**Risk:** Hidden or poorly communicated controls do not solve the accessibility problem.\
**Mitigation:** Keep breadcrumbs, history, and save/load controls visible enough that users can tell they exist.

## Common location and history failures <!-- role: mistakes -->

**Mistake:** Let the visualization change state without showing where the user is or how to get back. **Why it fails:** the interface remains disorienting and error recovery depends on memory.

## Check location and history support <!-- role: check -->

**Failure Sign:** After moving to another view or changing state, the interface gives no clear cue about the current location and no way to recover a prior state.\
**Quick Check:** Navigate through the dashboard or app and verify that the current view is shown with a breadcrumb or step indicator and that a prior state can be revisited.\
**Stronger Test:** Change the visualization through several states, then try to return to an earlier state without manually recreating it.

## Fix unclear location and history <!-- role: fix -->

- Add a breadcrumb trail or step indicator that identifies the current view within the dashboard or app.
- Add controls to save and reload the current visualization state.
- Add back/forward history so users can revisit earlier states without rebuilding them.
- Update the visible location cue when the active view changes.
