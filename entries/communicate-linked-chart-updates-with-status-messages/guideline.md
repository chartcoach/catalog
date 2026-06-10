---
id: communicate-linked-chart-updates-with-status-messages
title: Communicate chart interaction context with visible text and status messages
bibliography: references.bib
description: For interactive filtering and monitoring, use visible relationship text
  and programmatic status messages on charts that change other page content or receive
  external parameters to improve accessibility and mitigate ambiguous state changes
  for screen-reader users.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:interaction-access
- communication:context
- access:screen-reader:use
---

## Text relationship and status messages <!-- role: advice -->

Add visible text that states when a chart changes other content or when other controls change the chart. For example, name a filter relationship in text and emit a status message when a chart selection updates another panel or when an external control changes the chart's data or parameters.

## Why explicit interaction context works <!-- role: reason -->

Explicit relationship text and status messages turn hidden cross-view behavior into announced state changes. Users do not have to infer causal links from layout changes or hunt through the page to learn what changed.

**Mechanism:** Visible text explains the dependency between components, and programmatic status messages announce updates without moving focus, so users can track interaction effects as they happen.

**Evidence:** Chartability says that if a chart affects page logic or layout, or receives data or parameters from other controls, that relationship must be clearly communicated in text, and alerts or notifications must be programmatically available without requiring navigation. The paper also shows an interactive chart whose selection updates another view and notes that the update must be announced to screen readers [@elavskyHowAccessibleMy2022; @w3c_understanding_status].

## Use when interaction effects cross component boundaries <!-- role: context -->

- **User Goal:** Monitor what changed after interacting with a chart or related control.
- **Task:** Follow filtering, parameter changes, or other state changes across a page or view.
- **Chart Setting:** An interactive chart changes another area of the page or view, or another control changes the chart.
- **Audience:** Users who need explicit interaction context, including screen reader users.
- **Success Criterion:** Users can tell what changed and why without navigating away to discover it.

## Do not use when the chart is static and isolated <!-- role: exceptions -->

**Break it when:** The chart does not change other content and no other control changes the chart. **Why:** There is no cross-component interaction state to explain or announce.

## Costs of adding interaction context text <!-- role: costs -->

**Sacrifice:** You add visible text and update logic that must be maintained with the interaction.
**Risk:** Generic or repetitive messages can add noise without clarifying which change happened.
**Mitigation:** Tie each text explanation and status message to one specific interaction and one specific resulting change.

## Common failures in interaction context communication <!-- role: mistakes -->

- **Mistake:** Let the visual change in another panel be the only sign that an interaction had an effect. **Why it fails:** Users must infer the relationship instead of being told what changed.
- **Mistake:** Expose the update only after moving focus or navigating to another region. **Why it fails:** Screen reader users may miss the state change because it was not announced programmatically.

## Check linked interaction context <!-- role: check -->

**Failure Sign:** A chart interaction or linked control changes content elsewhere, but no visible text explains the relationship and no status message is announced.
**Quick Check:** Activate the chart interaction or linked control once. If another region updates and the dependency is not stated in text, fail it.
**Stronger Test:** Trigger the update with a screen reader active. If the change is not announced without moving focus or navigating, fail it.

## Fix hidden interaction effects <!-- role: fix -->

- Add visible text that states the dependency between the chart and the affected content.
- Emit a status or alert message when a chart interaction changes results, layout, or state elsewhere in the view.
- Emit a status or alert message when an external control changes the chart's data or parameters.
- Expose each status message programmatically so it can be monitored without navigation.
