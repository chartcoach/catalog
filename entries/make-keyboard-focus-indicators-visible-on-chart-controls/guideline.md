---
id: make-keyboard-focus-indicators-visible-on-chart-controls
title: Make keyboard focus indicators visible on chart controls
bibliography: references.bib
description: For keyboard navigation in interactive charts, use a visible, high-contrast
  focus indicator on each focusable control to improve accessibility and mitigate
  missing, obscured, or too-thin focus states for keyboard-only users.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:interaction-access
- needs:keyboard-only
- access:keyboard:use
- access:contrast:use
- polish:focus
---

## Visible keyboard focus styling <!-- role: advice -->

Add a visible keyboard focus indicator to every focusable chart control and keep it unobscured. For example, give the focused mark or control a focus state with at least a 2 px border, ensure the focus indicator has 4.5:1 contrast against the background, and make sure surrounding chart elements do not fully cover it.

## Why visible focus styling matters <!-- role: reason -->

Keyboard users follow the focus state to find where interaction currently is in the chart. If the focus indicator is missing, faint, or hidden by chart content, users can lose their place and miss available controls.

**Mechanism:** A strong focus indicator makes the current interactive element visually discoverable during keyboard navigation, so users can track position and operate the chart without relying on a mouse.

**Evidence:** Chartability defines missing, obscured, or low-contrast keyboard focus indication as an operable accessibility problem and instructs auditors to verify that the focus indicator is easy to distinguish, including contrast checks with a dropper or contrast tool [@elavskyHowAccessibleMy2022]. The linked WCAG 2.2 focus appearance guidance requires a focus indicator that is visually distinct and large enough to perceive around the focused element [@w3c_understanding_focus].

**Notes:** Chartability notes that custom author-provided focus indication was rare in reviewed charting systems, with many implementations relying on default styles and assumptions [@elavskyHowAccessibleMy2022].

## Use when chart controls take keyboard focus <!-- role: context -->

- **User Goal:** Navigate and operate chart controls without a mouse.
- **Task:** Move focus across interactive elements and identify the current target.
- **Chart Setting:** The chart, dashboard, or data interface contains focusable interactive elements.
- **Audience:** Keyboard-only users and assistive technology users who depend on keyboard navigation.
- **Success Criterion:** The current focused element is easy to see at each step of keyboard navigation.

## Do not apply when no chart element can receive focus <!-- role: exceptions -->

**Break it when:** The chart exposes no keyboard-focusable elements or interactions. **Why:** No visual focus state is triggered, so this specific repair does not apply.

## Cost of custom focus styling <!-- role: costs -->

**Sacrifice:** You must design and test a chart-specific focus style instead of relying on default styles.
**Risk:** Default focus styles can be too small, too low contrast, or hidden by chart geometry.
**Mitigation:** Define an explicit focus treatment and verify its border size, contrast, and visibility during keyboard navigation.

## Common focus-indicator failures <!-- role: mistakes -->

- **Mistake:** Relying on the default focus style without checking its size, color, or visibility against the chart background. **Why it fails:** Default styles and assumptions can leave focus indication missing, obscured, or too hard to see.
- **Mistake:** Using a focus border that is thinner than 2 px or blends into the background. **Why it fails:** The focused element remains hard to locate during keyboard navigation.

## Test keyboard focus visibility <!-- role: check -->

**Failure Sign:** As you tab through the chart, the current focused element is hard to find, disappears behind chart content, or has a faint outline.
**Quick Check:** Navigate the chart with the keyboard and confirm that each focusable element shows a clear visible focus state.
**Stronger Test:** Use a dropper and contrast calculator or the WebAIM Contrast Tool to verify that the focus indicator reaches 4.5:1 contrast against the background, visually confirm that it is not fully obscured, and check that the border is at least 2 px.

## Repair a weak focus indicator <!-- role: fix -->

- Add an explicit visual focus state to each focusable chart control.
- Increase the focus border to at least 2 px.
- Increase focus indicator contrast against the background to at least 4.5:1.
- Restyle or reposition the focus treatment so surrounding chart elements do not fully obscure it.
