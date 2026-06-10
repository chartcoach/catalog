---
id: animate-meaningful-chart-updates-and-announce-state-changes
title: Animate meaningful chart updates and announce state changes
bibliography: references.bib
description: For dynamic chart updates, use bounded transition timing and state announcements
  on changing chart elements to improve accessibility and mitigate hard-to-follow
  changes for readers following meaningful data updates, including screen-reader users.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:interaction-access
- temporal-pattern:dynamic
- access:screen-reader:use
---

## Animate and announce meaningful updates <!-- role: advice -->

Animate meaningful chart updates so readers can follow the change from one state to the next. For example, when a chart’s data or interactive state changes in a meaningful way, animate the update between 250 ms and 2 s and provide a screen-reader announcement for the new state.

## Why bounded update transitions help <!-- role: reason -->

Readers need a stable bridge between the old state and the new state when a chart changes. Screen-reader users also need an explicit nonvisual signal that the state changed.

**Mechanism:** Bounded transition timing supports object constancy, so readers can track what changed instead of seeing marks jump abruptly or linger too long. State announcements expose the same change to screen-reader users.

**Evidence:** Chartability states that meaningful chart data changes should use animation for object constancy and that changes to state must be announced to screen reader users [@elavskyHowAccessibleMy2022]. The linked source recommends keeping update animations between 250 ms and 2 s because shorter changes may be hard to follow and longer ones may frustrate users [@amr_structuring_and_2016].

**Notes:** This rule is presented as research-synthesized and explicitly described as needing more accessibility research.

## Use when chart updates carry meaning <!-- role: context -->

- **User Goal:** Follow what changed after a chart update.
- **Data:** The chart’s data or state changes in a meaningful way.
- **Chart Setting:** The chart updates dynamically or interactively.
- **Audience:** Readers include screen-reader users.
- **Success Criterion:** The visual change is trackable and the state change is also exposed nonvisually.

## Do not use when there is no meaningful change to follow <!-- role: exceptions -->

**Break it when:** the chart does not present a meaningful data or state change that users need to follow. **Why:** the source conditions this treatment on meaningful changes.

## Costs of animated update treatment <!-- role: costs -->

**Sacrifice:** The updated state is not shown instantaneously.
**Risk:** Transitions that are too short become hard to follow, and transitions that are too long frustrate users.
**Mitigation:** Keep transition duration within the 250 ms to 2 s range and pair the visual update with a screen-reader announcement.

## Common update failures <!-- role: mistakes -->

- **Mistake:** Letting meaningful chart changes appear as an instant jump with no transition. **Why it fails:** readers lose object constancy and the change becomes hard to follow.
- **Mistake:** Using transition durations faster than 250 ms or longer than 2 s. **Why it fails:** the change becomes either hard to follow or frustrating.
- **Mistake:** Changing chart state without a screen-reader announcement. **Why it fails:** screen-reader users are not informed that the state changed.

## Check meaningful update behavior <!-- role: check -->

**Failure Sign:** A meaningful chart change jumps abruptly, drags on too long, or is not announced to screen-reader users.
**Quick Check:** Trigger a meaningful update and verify that the visual transition lasts between 250 ms and 2 s and that a screen reader receives a state-change announcement.
**Stronger Test:** Trigger several meaningful updates and confirm each one is visually followable and nonvisually announced.

## Fix the update treatment <!-- role: fix -->

- Add an animated transition to each meaningful chart update.
- Adjust the transition duration so it is not faster than 250 ms and not longer than 2 s.
- Add a text announcement for each meaningful state change so screen-reader users are notified.
