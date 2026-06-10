---
id: make-chart-layouts-reflow-under-zoom
title: Make chart layouts reflow under zoom
bibliography: references.bib
description: For zoomed reading and interaction, use reflow-capable layout behavior
  on chart space and chart elements to improve accessibility and mitigate content
  cutoff and two-direction scrolling for people who zoom content or use assistive
  technology.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:layout-structure
- access:zoom:use
- access:reflow:use
---

## Reflow the chart layout under zoom <!-- role: advice -->

Make the chart space reflow when users zoom so text, geometries, and controls resize and stay available. For example, let the chart be zoomed through assistive technology or an equivalent mechanism, and wrap, stack, or otherwise rearrange the display so no meaningful information or functionality is cut off or requires two-direction scrolling.

## Why reflow under zoom preserves access <!-- role: reason -->

Zoom enlarges content to make a chart readable and operable. A fixed chart frame can clip labels, marks, or controls and force users to navigate in two directions, which hides information and interrupts interaction. Reflow keeps the zoomed chart in view while preserving the same information and functions.

**Mechanism:** Reflow lets enlarged text, geometries, and controls stay visible together instead of breaking the chart into clipped regions or separate horizontal and vertical navigation paths.

**Evidence:** Chartability requires chart space to be zoomable, requires text, geometries, and all elements to resize appropriately for the zoom type, and requires content to reflow without being cut off in two directions [@elavskyHowAccessibleMy2022]. The linked WCAG reflow guidance requires preserving information and functionality when zoomed or viewed at 320 CSS pixels, and recommends layouts that wrap or stack content to avoid horizontal scrolling [@w3c_understanding_reflow].

## Use when zoom must preserve the chart <!-- role: context -->

- **User Goal:** Enlarge the chart to read or operate it.
- **Chart Setting:** The chart is viewed with browser, operating-system, application, or assistive-technology zoom, or in a narrow responsive layout.
- **Audience:** People who zoom content or use assistive technology.
- **Success Criterion:** Text, geometries, and controls all resize appropriately, and no meaningful information or functionality is lost or cut off in two directions.

## Do not add extra reflow changes when the layout already passes <!-- role: exceptions -->

**Break it when:** The current chart layout already preserves all meaningful information and functionality when zoomed or viewed at narrow width without two-direction scrolling. **Why:** Extra rearrangement is unnecessary once the reflow condition is already satisfied.

## Costs of reflowing the layout <!-- role: costs -->

**Sacrifice:** The original composition of the chart may change at higher zoom levels or narrower widths.\
**Risk:** A careless reflow can drop meaningful information or functionality while rearranging the display.\
**Mitigation:** Resize text, geometries, and controls together and verify that every meaningful view and function remains available after reflow.

## Common zoom and reflow failures <!-- role: mistakes -->

- **Mistake:** Let text enlarge but keep marks, geometries, or controls fixed. **Why it fails:** The criterion requires all elements to change size appropriately for the zoom type.
- **Mistake:** Allow zoom to push part of the chart off-screen so users must navigate in two directions. **Why it fails:** Content should reflow without losing information or functionality and should not be cut off from view in two directions.

## Check zoom and reflow support <!-- role: check -->

**Failure Sign:** Zoomed charts show clipped labels, hidden marks, missing controls, or require both horizontal and vertical navigation to access meaningful content.\
**Quick Check:** Zoom the chart with the available browser, application, or assistive-technology method and confirm that text, geometries, and controls resize and remain visible.\
**Stronger Test:** View the chart at a narrow width equivalent to reflow testing, such as 320 CSS pixels, and confirm that no meaningful information or functionality is lost and the view does not break into two-direction cutoff.

## Fix zoom and reflow failures <!-- role: fix -->

- Allow the chart container to resize under zoom instead of keeping a fixed chart space.
- Resize chart text, geometries, and interactive elements according to the zoom type being used.
- Rearrange the display during reflow by wrapping or stacking content so the zoomed view keeps all meaningful information and functionality.
- Redesign the responsive layout if the current arrangement cannot avoid content cutoff in two directions.
