---
id: provide-standard-ui-alternatives-for-complex-chart-actions
title: Provide standard UI alternatives for complex chart actions
bibliography: references.bib
description: For interactive exploration, use standard UI alternatives for complex
  actions on interactive charts with brushing, zooming, filtering, or gesture controls
  to improve accessibility and mitigate pointer-only interaction barriers for keyboard,
  screen-reader, and touch-device users.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:interaction-access
- access:keyboard:use
- access:screen-reader:use
- needs:keyboard-only
- needs:screen-reader
---

## Standard controls for special actions <!-- role: advice -->

Add a standard UI control for each complex chart action instead of requiring the custom action itself. For example, make a mouse hover or click interaction available through keyboard navigation, and add a search control that directly selects data in the chart space without requiring the user to perform the original gesture.

## Why standard alternatives improve operability <!-- role: reason -->

Complex chart interactions can depend on custom gestures that are hard to discover and hard to execute across input modes. A standard control gives the same action a predictable path and lets users reach chart content without reproducing the original gesture.

**Mechanism:** Standard alternatives make special actions discoverable and operable through common interaction paths, so the action does not depend on one gesture style or one input method.

**Evidence:** Chartability defines it as an operability failure when brushing, zooming, filtering, or gesturing use custom or complex chart controls without a standard UI alternative, and it gives keyboard equivalents and direct search across the data or chart space as concrete alternatives [@elavskyHowAccessibleMy2022]. The linked WCAG guidance for Multiple Ways supports providing more than one path to locate content, including search, to make content easier to find and reduce reliance on memory [@w3c_understanding_multiple].

**Notes:** The alternative does not need to be a literal one-to-one translation of the original gesture.

## Use when a chart action depends on a custom gesture <!-- role: context -->

- **User Goal:** Explore, zoom, filter, or select data through chart interaction.
- **Task:** Perform a special action such as brushing, zooming, filtering, gesturing, or direct element selection.
- **Chart Setting:** The chart uses a custom or complex interaction instead of a standard UI control.
- **Audience:** People operating with keyboard, screen reader, or touch input.
- **Success Criterion:** Every special action can be completed through a clear standard alternative.

## Do not apply when no special action exists <!-- role: exceptions -->

**Break it when:** The chart has no brushing, zooming, filtering, gesturing, or other special action beyond standard UI controls. **Why:** There is no complex interaction that needs an alternative path.

## Costs of parallel controls <!-- role: costs -->

**Sacrifice:** The interface needs an additional standard control for the same action.\
**Risk:** A literal one-to-one input translation can still leave the task hard to use.\
**Mitigation:** Use a different standard path when it is clearer, such as direct search across the data or chart space.

## Common failures in action alternatives <!-- role: mistakes -->

- **Mistake:** Leaving brushing, zooming, filtering, or gesturing available only through drag, hover, pinch, or another custom pointer behavior. **Why it fails:** Users who cannot use that gesture have no way to perform the action.
- **Mistake:** Adding an alternative control that is not clear or not operable with keyboard, screen reader, and touch. **Why it fails:** The alternative exists formally but not as a usable path.

## Check each special action <!-- role: check -->

**Failure Sign:** A chart state can be changed only by dragging, pinching, hovering, or another custom gesture inside the chart.\
**Quick Check:** List each special action, then try to complete it with only keyboard and with a screen reader; if any action lacks a clear standard control, fail.\
**Stronger Test:** On a touch device, confirm the same action is available through a standard control or search path instead of only through the custom gesture.

## Add alternative control paths <!-- role: fix -->

- Add a standard UI control for each brushing, zooming, filtering, or gesture-based action.
- Expose mouse hover or click interactions through keyboard navigation when the same element needs to be discoverable or selectable.
- Add a search control across the data or chart space so users can directly select elements without reproducing the gesture.
- Replace a gesture-only trigger with a clear control that works with keyboard, screen reader, and touch input.
