---
id: add-visible-instructions-for-chart-interactions
title: Add visible instructions for every chart interaction
bibliography: references.bib
description: For interactive chart use, use visible interaction instructions on charts
  with any interactive controls to improve accessibility and mitigate undiscoverable
  keyboard and pointer actions for users with keyboard-only or cognitive access needs.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:interaction-access
- component:annotation:use
- needs:keyboard-only
- needs:cognitive
- access:keyboard:use
---

## Add visible interaction instructions <!-- role: advice -->

Add visible instructions anywhere a chart supports interaction. For example, state how to hover or select with a mouse, and list the keyboard actions used to move between visuals, enter a chart or filter, and make a selection.

## Why visible interaction instructions work <!-- role: reason -->

Visible interaction instructions make hidden controls discoverable across input modes. They reduce guesswork about how to enter an interactive chart, move among controls, and complete selections.

**Mechanism:** When interaction instructions are shown in the interface, users do not have to infer whether a chart is interactive or guess which keys or pointer actions are supported.

**Evidence:** Chartability marks missing interaction cues or instructions as a critical operability failure and requires any interactive chart to explain its controls, including keyboard controls [@elavskyHowAccessibleMy2022]. WCAG guidance requires labels or instructions for interactive controls, and the cited accessible dashboard example provides explicit key instructions for navigation, entry, and selection [@w3c_understanding_labels; @sf_covid19_data].

**Notes:** Do not rely on the assumption that good visual design makes interaction self-evident.

## When visible interaction instructions apply <!-- role: context -->

- **User Goal:** Operate an interactive chart or dashboard control.
- **Task:** Enter a chart, navigate between visuals, or select or filter options.
- **Chart Setting:** The chart has interactive behavior such as hover, selection, filtering, or keyboard navigation.
- **Audience:** People using keyboard input, including screen reader users, and people who benefit from explicit instructions.
- **Success Criterion:** A user can discover that interaction exists and identify the required keys or pointer actions before trial and error.

## When not to apply this rule <!-- role: exceptions -->

**Break it when:** The chart is fully static and exposes no interactive behavior. **Why:** The requirement is scoped to charts that have interactive capabilities.

## Costs of visible interaction instructions <!-- role: costs -->

**Sacrifice:** The chart must carry extra explanatory text.
**Risk:** Partial instructions can still leave keyboard interaction undiscoverable.
**Mitigation:** Document every supported interaction mode, including keyboard controls.

## Common failure around visible interaction instructions <!-- role: mistakes -->

**Mistake:** Assuming users will infer interactive behavior from the design and omitting visible instructions. **Why it fails:** Hover, keyboard, or selection behavior remains hidden to users who do not explore the chart the same way.

## How to test visible interaction instructions <!-- role: check -->

**Failure Sign:** The chart responds to hover, focus, tab, arrow keys, Enter, or Space, but no visible text explains those actions.
**Quick Check:** Look for instructions before interacting. If you cannot tell how to enter, move, or select with the keyboard, the chart fails.
**Stronger Test:** Use only the keyboard to navigate the visualization and verify that every working key action is named in the instructions.

## How to fix missing interaction instructions <!-- role: fix -->

- Add a visible instruction block that states the chart is interactive and where interaction applies.
- List each supported keyboard action, including how to move, enter, and select.
- Name the matching pointer action when the chart supports hover or mouse selection.
- If interaction spans several visuals or filters, explain how users move between them before they operate the chart.
