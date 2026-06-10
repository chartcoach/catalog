---
id: provide-keyboard-equivalent-access-for-interactive-chart-controls
title: Provide keyboard-equivalent access for interactive chart controls
bibliography: references.bib
description: For operating interactive charts, use matched keyboard interaction access
  on interactive chart controls to improve accessibility and mitigate mouse-only interaction
  for keyboard-only and screen-reader users.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:interaction-access
- needs:keyboard-only
- needs:screen-reader
- access:keyboard:use
---

## Mirror pointer interactions through the keyboard interface <!-- role: advice -->

Give every interactive chart control a keyboard path that provides the same outcome as the pointer interaction. For example, let Tab and arrow keys reach chart controls, make focus mirror hover, make Enter or Space mirror click or selection, and test the same chart with a screen reader and on touch devices.

## Why equivalent keyboard interaction matters <!-- role: reason -->

Mouse-only interaction hides chart functionality from people who use the keyboard interface and can also break access through screen readers and other assistive technologies. Equivalent keyboard interaction makes the same controls discoverable and operable without requiring a pointer.

**Mechanism:** When focus follows the same interaction path as hover and keyboard activation follows the same path as click, users can reach, inspect, and trigger chart behavior through the keyboard interface instead of depending on a mouse.

**Evidence:** Chartability marks single-input interaction as a critical failure and specifies that interactive charts reachable by mouse must also be operable by keyboard, with focus mirroring hover, Enter or Space mirroring clicks, and screen reader and touch experiences tested alongside keyboard-only testing [@elavskyHowAccessibleMy2022]. WCAG's keyboard criterion requires all functionality to be operable through a keyboard interface, and the cited Progressive Access example demonstrates interactive diagrams that support keyboard and menu-driven exploration across devices [@w3c_understanding_keyboard; @progressiveaccess_accessible_chemistry].

**Notes:** The source treats the keyboard interface as the primary access path to build first for interactive content.

## Use when the chart has pointer-driven interaction <!-- role: context -->

- **User Goal:** Operate or inspect chart interactions without using a mouse.
- **Chart Setting:** The chart includes hover, click, selection, or another pointer-driven interaction.
- **Audience:** Keyboard-only users and screen reader users, with touch users needing a verified experience as well.
- **Success Criterion:** Every interactive state can be reached and triggered without a mouse, and keyboard focus produces the same interaction feedback as pointer hover.

## Do not apply this as an added interaction requirement to static charts <!-- role: exceptions -->

**Break it when:** The chart has no interactive controls or pointer-driven behavior to replicate. **Why:** The source frames this requirement as a repair for interactive content that already works with a mouse or another input device.

## Costs of matching keyboard interaction <!-- role: costs -->

**Sacrifice:** You add implementation and testing work across keyboard, screen reader, and touch interaction paths.\
**Risk:** Treating touch and mouse as one generic pointer path can still leave mobile interaction inaccessible because touch uses a larger hit area.\
**Mitigation:** Test keyboard, screen reader, and touch separately instead of assuming one input mode covers the others.

## Common failure modes in keyboard access <!-- role: mistakes -->

- **Mistake:** Leave hover or click behavior available only to the mouse. **Why it fails:** The chart remains operable through only one input type.
- **Mistake:** Make chart elements focusable but do not make focus mirror hover or Enter and Space mirror click. **Why it fails:** Keyboard users can reach the control without getting the same interaction outcome.

## How to test interaction equivalence <!-- role: check -->

**Failure Sign:** A mouse can reveal, select, or trigger chart behavior that Tab, arrow keys, Enter, or Space cannot reproduce.\
**Quick Check:** Put the mouse away and navigate the chart with Tab and arrow keys; confirm that focus reaches the interactive controls and produces the same state as hover.\
**Stronger Test:** Activate the same controls with Enter or Space, then repeat the interaction with a screen reader and on a touch device to check for different behavior.

## What to change in the chart <!-- role: fix -->

- Add a keyboard path to each interactive chart control using Tab and arrow keys.
- Bind keyboard focus to the same reveal or inspection state used for hover.
- Bind Enter or Space to the same action used for click or selection.
- Re-test the chart with a screen reader and on a touch device, then adjust any interaction that still works only through the pointer path.
