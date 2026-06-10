---
id: provide-multiple-paths-to-the-same-chart-information
title: Provide multiple paths to the same chart information
bibliography: references.bib
description: For retrieve tasks in complex dashboard and multi-state chart interfaces,
  use multiple navigation paths on views, filtered states, and pages to improve accessibility
  and mitigate single-process information access for users with disabilities and assistive
  technologies.
labels:
- purpose:refine
- basis:accessibility
- task:retrieve
- quality:accessibility
- lever:interaction-access
- communication:workflow
---

## Add a second route to the same result <!-- role: advice -->

Provide more than one process to reach the same chart information or interactive state. For example, if a result is revealed through filter steps, view or state transitions, or page changes, add an alternative path such as search, direct navigation, or a parallel UI control that reaches that same result.

## Why redundant paths matter <!-- role: reason -->

A single navigation sequence can make information effectively unavailable when that sequence is hard to operate, remember, or discover. Redundant paths let users reach the same result even if one flow is inaccessible or impractical.

**Mechanism:** Multiple paths reduce dependence on one interaction sequence and make the information architecture more tolerant of different navigation preferences and assistive technology use.

**Evidence:** Chartability identifies single-process access as an accessibility failure in complex dashboards and applications and recommends alternative paths such as search and parallel controls to reach the same information or state. WCAG's Multiple Ways guidance likewise recommends at least two ways to locate content so users do not have to rely on one navigation method alone [@elavskyHowAccessibleMy2022; @w3c_understanding_multiple_2].

**Notes:** This is an information architecture problem as much as a chart problem.

## Use when the chart is inside a complex flow <!-- role: context -->

- **User Goal:** Find known information or return to a previously reached chart result.
- **Task:** Retrieve information after filters, state changes, view transitions, or page navigation.
- **Chart Setting:** The chart is embedded in a dashboard or application with deep or complex exploratory flows.
- **Audience:** Users with disabilities or assistive technologies who may prefer different ways to consume information.
- **Success Criterion:** The same information or chart state can be reached through at least two distinct processes.

## Do not rely on this rule outside complex flows <!-- role: exceptions -->

**Break it when:** The chart does not hide information behind view changes, state transitions, filter sequences, or page moves. **Why:** This rule targets information that would otherwise be locked behind one process.

## Tradeoffs of redundant navigation <!-- role: costs -->

**Sacrifice:** The interface needs extra navigation or control surfaces.
**Risk:** A second path that does not land on the same information only adds complexity.
**Mitigation:** Make each added path reach the same result or state, not a nearby substitute.

## Single-sequence access failure <!-- role: mistakes -->

**Mistake:** Requiring one fixed sequence of filters, page changes, or state transitions to reveal a result. **Why it fails:** Users who cannot operate, discover, or repeat that sequence have no other way to reach the same information.

## Check for a second route <!-- role: check -->

**Failure Sign:** A chart result or state can be reached only by one sequence of interactions.
**Quick Check:** Starting from the chart, try to reach the same information a second way, such as through search, direct navigation, or a parallel control.
**Stronger Test:** Recreate the same filtered or transitioned state without repeating the original sequence; if you cannot, fail.

## Add equivalent access paths <!-- role: fix -->

- Add direct navigation to the target view or page instead of requiring the original sequence.
- Add a parallel UI control that reaches the same filtered or transitioned state.
- Add search that finds the same information without repeating the original interaction path.
