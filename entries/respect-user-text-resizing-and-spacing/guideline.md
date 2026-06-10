---
id: respect-user-text-resizing-and-spacing
title: Respect user text resizing and spacing settings
bibliography: references.bib
description: For chart reading when users change text size or spacing, use chart text
  styling that respects user-agent font-size and text-spacing changes on chart text
  elements to prevent loss of content or functionality and address charts that block
  browser zoom or imported styles for people with low vision.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:interaction-access
- channel:text:use
- needs:low-vision
- access:zoom:use
---

## Respect user text settings <!-- role: advice -->

Let chart text inherit user-controlled font-size and text-spacing changes. For example, keep labels, titles, and other chart text resizable through browser zoom or an imported custom stylesheet, and remove style rules that block those changes.

## Why respecting text overrides works <!-- role: reason -->

When chart text follows user settings, readers who enlarge text or increase spacing can keep reading the chart without losing content or controls.

**Mechanism:** User-agent text adjustments reach the chart, so enlarged or respaced text remains readable and available without breaking the experience.

**Evidence:** Chartability states that user-changed font size and text spacing must be respected and that charts must not interfere with programmatic changes such as custom stylesheets or browser zoom. WCAG guidance further requires text to be resizable up to 200% without assistive technology and without loss of content or functionality [@elavskyHowAccessibleMy2022; @w3c_understanding_resize].

**Notes:** This guideline covers both font-size changes and text-spacing changes.

## Use when text settings come from the user environment <!-- role: context -->

- **User Goal:** Read chart text after enlarging text or increasing spacing.
- **Chart Setting:** A digital chart in a browser or application where user-agent settings can change text presentation.
- **Audience:** People who change text size or spacing, including people with low vision.
- **Success Criterion:** Chart text adjusts accordingly without loss of content or functionality.

## Do not apply this as written outside digital user-agent contexts <!-- role: exceptions -->

**Break it when:** The artifact is not a digital chart that can receive user-agent text changes such as browser zoom or imported styles. **Why:** This rule targets programmatic text adjustments in digital environments.

## Costs of giving users control over chart text <!-- role: costs -->

**Sacrifice:** Exact fixed control over text size and spacing.
**Risk:** Rigid text layouts may need rework once users enlarge or respace text.
**Mitigation:** Remove rules that block user overrides and revise the text layout until content and functionality remain available.

## Common failure mode: fixed chart text <!-- role: mistakes -->

**Mistake:** Hard-code chart text so browser zoom or imported text styles do not change font size or spacing. **Why it fails:** Users cannot apply their own reading settings, and content or functionality may be lost.

## Check whether chart text still works after user changes <!-- role: check -->

**Failure Sign:** Chart text stays fixed, ignores increased spacing, or loses content or functionality after user changes.
**Quick Check:** Use the browser's built-in zoom and confirm that chart text adjusts accordingly.
**Stronger Test:** Increase text to 200% and apply a custom stylesheet that changes text spacing, then verify that chart text remains available and the chart still functions.

## Fix blocked text resizing and spacing <!-- role: fix -->

- Replace fixed text rules with styles that allow user-controlled font-size changes.
- Remove style rules that prevent imported text-spacing changes from taking effect.
- Rework the text layout so enlarged or respaced chart text remains available without losing functionality.
