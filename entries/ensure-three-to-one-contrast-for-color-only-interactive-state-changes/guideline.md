---
id: ensure-three-to-one-contrast-for-color-only-interactive-state-changes
title: Ensure color-only interactive state changes reach 3:1 contrast
bibliography: references.bib
description: For interactive chart navigation and selection, use high-contrast color
  state changes on interactive elements in charts to improve accessibility and mitigate
  subtle hover, focus, and selection changes for low-vision users.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:interaction-access
- needs:low-vision
- access:contrast:use
---

## Contrast in state changes <!-- role: advice -->

Set hover, focus, and selection states so a color-only state change differs from the previous state by at least 3:1 contrast. For example, if a mark changes opacity, saturation, or hue when hovered, focused, or selected, strengthen that change until it clears 3:1 instead of relying on a subtle tint shift.

## Why stronger state contrast works <!-- role: reason -->

Interactive state changes tell readers what can be operated and what is currently active. When that change is only a slight color shift, the interactive state can blend into the default state and become hard to notice.

**Mechanism:** A stronger contrast jump makes the changed state visibly distinct from the prior state, so users can detect hover, focus, and selection more reliably.

**Evidence:** Chartability defines low contrast on interactive elements as an operability issue and requires a 3:1 difference between the previous and changed state when color alone signals hover, focus, or selection; it also names thicker strokes, dash patterns, and markers as acceptable additional indicators and recommends redundant use when possible [@elavskyHowAccessibleMy2022]. WCAG's non-text contrast guidance likewise requires a 3:1 contrast ratio for user-interface components and graphical objects against adjacent colors [@w3c_understanding_non_text_2].

**Notes:** If the state change is also conveyed with an added high-contrast non-color cue, the separate color-difference contrast threshold is not required.

## Use when state changes signal interactivity <!-- role: context -->

- **User Goal:** Find what is interactive and tell which element is hovered, focused, or selected.
- **Task:** Operate interactive marks or controls.
- **Chart Setting:** The chart includes interactive elements, and the state change is communicated visually.
- **Audience:** People with low vision or anyone likely to miss subtle state changes.
- **Success Criterion:** Each changed state is clearly distinguishable from its previous state.

## Skip the color-difference threshold when non-color cues already carry the state <!-- role: exceptions -->

**Break it when:** The changed state already adds a high-contrast non-color indicator such as at least a 2px stroke thickness change, a dash pattern, or a marker. **Why:** The source does not require a separate color-difference contrast threshold when those added indicators are present.

## Costs of stronger state contrast <!-- role: costs -->

**Sacrifice:** A subtle color-only hover, focus, or selection style may need to be replaced.\
**Risk:** If you keep only a slight opacity, saturation, or hue shift, the state change remains hard to detect.\
**Mitigation:** Add a high-contrast non-color cue so the state does not depend on color alone.

## Common failure mode in state styling <!-- role: mistakes -->

**Mistake:** Showing hover, focus, or selection with only a small change in opacity, saturation, or hue. **Why it fails:** The changed state can blend into the previous state and does not clearly communicate the interactive change.

## How to test state contrast <!-- role: check -->

**Failure Sign:** Hover, focus, or selection is visible only as a faint color shift.\
**Quick Check:** Compare the previous state and changed state with a contrast calculator or dropper tool and verify at least 3:1 contrast.\
**Stronger Test:** Check each hover, focus, and selection state separately; if a state relies on color alone and does not reach 3:1, treat it as a failure.

## What to change in the chart <!-- role: fix -->

- Darken, lighten, or otherwise adjust the hover, focus, or selection color until the changed state reaches at least 3:1 against the previous state.
- Replace a subtle opacity-only or saturation-only state change with a more distinct color change.
- Add a high-contrast non-color cue such as at least a 2px stroke thickness change, a dash pattern, or a marker.
- Use color and non-color state indicators together when possible.
