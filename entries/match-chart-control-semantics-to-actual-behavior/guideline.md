---
id: match-chart-control-semantics-to-actual-behavior
title: Match chart control semantics to actual behavior
bibliography: references.bib
description: For accessibility review of web charts, use semantically valid document
  elements and roles on interactive chart elements to improve accessibility and mitigate
  mislabeled controls for screen-reader users.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:interaction-access
- needs:screen-reader
- access:screen-reader:use
---

## Match semantics to behavior <!-- role: advice -->

Use document elements and roles that match what each chart control actually does. For example, if a chart mark, filter, or toggle acts like a button, expose it as a button and make sure its name, role, and current state are available to assistive technologies.

## Why semantic matching works <!-- role: reason -->

Semantic matching gives assistive technologies the same control model the visual interface implies. When the announced role and state match the actual interaction, screen reader users can identify what a chart control is, what it does, and whether its state changed.

**Mechanism:** Correct semantics make control type and state programmatically available, which lets assistive technologies interpret and announce interactive chart behavior reliably.

**Evidence:** Chartability identifies semantically invalid document elements as a Robust accessibility failure and specifies that web checks may start with automated validators but only pass after screen reader verification [@elavskyHowAccessibleMy2022; @deque_axe_devtools]. The Name, Role, Value criterion requires user interface components to expose programmatically determinable names, roles, and states so assistive technologies can identify the control and its current state [@w3c_understanding_name].

## Use when semantic validity must be verified <!-- role: context -->

- **User Goal:** Audit or remediate chart accessibility.
- **Task:** Verify that interactive chart elements work with assistive technologies.
- **Chart Setting:** A web chart or dashboard contains interactive elements, custom controls, or state changes.
- **Audience:** Screen reader users and other assistive technology users.
- **Success Criterion:** Document elements are semantically valid, and a screen reader announces the correct control type and state.

## Do not stop at automation alone <!-- role: exceptions -->

**Break it when:** the review treats an automated scan as sufficient evidence that chart semantics are valid. **Why:** this guideline only passes once a screen reader test also verifies the experience.

## Costs of semantic verification <!-- role: costs -->

**Sacrifice:** You must add manual screen reader testing instead of relying on automated validation alone.\
**Risk:** Passing a checker can still leave the announced control type or state wrong in practice.\
**Mitigation:** After automated validation, run a focused screen reader pass on each meaningful interactive chart element.

## Common semantic failures <!-- role: mistakes -->

- **Mistake:** Styling a generic element to behave like a button without giving it button semantics. **Why it fails:** assistive technologies may not identify what the control is or what action it performs.
- **Mistake:** Declaring the chart semantically valid after only an automated scan. **Why it fails:** Chartability requires screen reader verification before this failure is cleared.

## How to test semantic validity <!-- role: check -->

**Failure Sign:** An interactive chart element is announced as a generic element or with the wrong control type, or its state is not announced.\
**Quick Check:** Run an automated web accessibility validator such as Axe-core, Wave, HTML Codesniffer, Accessibility Insights, or W3C Markup Validation.\
**Stronger Test:** Use a screen reader to move through each interactive chart element and confirm that its name, role, and current state match the visible behavior.

## What to change <!-- role: fix -->

- Replace a generic document element with the semantic element that matches the interaction it performs.
- Give each custom chart control a programmatically determinable name, role, and current state.
- Re-run an automated validator on the web chart after the semantic change.
- Repeat the screen reader pass until the announced role and state match the chart’s actual behavior.
