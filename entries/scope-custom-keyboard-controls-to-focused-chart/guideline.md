---
id: scope-custom-keyboard-controls-to-focused-chart
title: Scope custom keyboard controls to the focused chart
bibliography: references.bib
description: For interactive navigation in charts and dashboards, use focus-scoped
  custom keyboard controls on interactive chart elements to prevent assistive-technology
  command conflicts and mitigate keyboard traps for screen reader and keyboard-only
  users.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:interaction-access
- needs:screen-reader
- needs:keyboard-only
- access:keyboard:use
---

## Focused keyboard control scope <!-- role: advice -->

Limit custom keyboard handlers to the focused chart or focused chart elements. For example, keep Tab for normal focus movement, activate chart navigation or selection keys only after the user enters the chart, and do not let chart shortcuts run as page-wide or app-wide overrides.

## Why focus-scoped controls help <!-- role: reason -->

Focus-scoped controls let people move through a page with native keyboard and assistive-technology commands until they intentionally enter a chart. This prevents the chart from stealing keys that users rely on for navigation and operation.

**Mechanism:** Restricting custom handlers to the focused component preserves normal page navigation outside the chart and keeps chart-specific controls active only inside the chart interaction mode.

**Evidence:** Chartability marks assistive-technology control overrides as a critical operability failure and warns that overriding native keys such as Tab creates severe problems for keyboard and screen reader users [@elavskyHowAccessibleMy2022]. WCAG 2.1 requires character shortcuts to be off, remapped with non-printable keys, or active only on focus, and accessible dashboard guidance shows explicit focused entry into charts instead of page-wide overrides [@w3c_character_key; @sf_covid19_data_2].

**Notes:** Visible keyboard instructions help users discover when chart-specific controls become active.

## Use when chart controls are custom <!-- role: context -->

- **User Goal:** Move through the page and operate an interactive chart without losing native commands.
- **Task:** Enter a chart, navigate within it, and select values or filters by keyboard.
- **Chart Setting:** An interactive chart or dashboard uses custom keyboard handlers or a chart-specific navigation model.
- **Audience:** Screen reader users and keyboard-only users.
- **Success Criterion:** Chart controls respond only when the chart or its elements have focus, and normal page navigation still works outside the chart.

## Do not rely on page-wide key overrides <!-- role: exceptions -->

**Break it when:** The interaction design depends on page-wide or app-wide key overrides to work. **Why:** The custom control model must be redesigned, because the source requires custom keys to stay inactive until the chart or element has focus.

## Tradeoffs of focus-scoped controls <!-- role: costs -->

**Sacrifice:** Page-wide shortcuts are no longer always available.
**Risk:** Users may not realize that chart-specific keys exist after you limit them to focused use.
**Mitigation:** Add visible instructions for entering the chart and using the focused controls.

## Common control-scope failures <!-- role: mistakes -->

- **Mistake:** Override the native Tab key for chart navigation. **Why it fails:** This creates keyboard traps and interferes with expected keyboard and screen reader movement.
- **Mistake:** Leave chart shortcuts active when focus is elsewhere on the page. **Why it fails:** Page-level handlers can steal commands from assistive technology.

## Test control scope with focus <!-- role: check -->

**Failure Sign:** A chart responds to its custom keys when focus is outside the chart, or Tab no longer moves focus normally.
**Quick Check:** With focus outside the chart, press the chart's custom keys and confirm that nothing in the chart responds; then focus the chart and confirm that the keys work there.
**Stronger Test:** Navigate the page and chart with a keyboard and screen reader to verify that entering, moving within, and selecting in the chart does not override native commands.

## Repair global key overrides <!-- role: fix -->

- Move custom key handlers from page or app scope to the chart container or focused chart elements.
- Restore native Tab behavior for focus movement and remove chart logic attached to it.
- Require an explicit chart entry state before enabling chart navigation or selection keys.
- Add visible keyboard instructions that tell users how to enter the chart and which focused controls are available.
