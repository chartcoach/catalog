---
id: reuse-styling-and-controls-for-same-function-charts
title: Reuse the same styling and controls for charts with the same function
bibliography: references.bib
description: For repeated chart use across an application or environment, use consistent
  styling, user settings, and interaction defaults on charts that perform the same
  function to improve accessibility and mitigate confusion for users with cognitive
  or memory impairments.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:interaction-access
- polish:consistency
- needs:cognitive
---

## Reuse styling and interaction defaults <!-- role: advice -->

Keep default styling, user-set settings, and interaction defaults the same on charts that perform the same function in the same application or environment. For example, reuse the same default style and user-selected presentation settings across matching charts, and keep the same keybindings or interaction pattern when two charts support the same task.

## Consistency reduces relearning across charts <!-- role: reason -->

Consistent chart defaults let people transfer what they learned from one chart to the next instead of re-learning labels, styling, or controls each time.

**Mechanism:** Shared styling, settings, and interaction patterns make repeated chart use more predictable, so users can recognize and operate the same function without extra recall work.

**Evidence:** Chartability's Flexible principle requires charts in the same application or environment to share default styling, user-set settings, and interaction defaults when they perform the same task or function [@elavskyHowAccessibleMy2022]. Consistent identification guidance says components with the same function should be labelled consistently because consistent labels, icons, and positions help users recognize controls and reduce confusion, especially for people with cognitive or memory impairments [@w3c_understanding_consistent].

**Notes:** Consistency applies both to the defaults the system provides and to settings the user has already chosen.

## Use when charts repeat the same function <!-- role: context -->

- **User Goal:** Move between charts and reuse familiar controls and presentation choices.
- **Task:** Perform the same chart task or function more than once.
- **Chart Setting:** An application or environment contains multiple charts with shared controls, styling defaults, or keybindings.
- **Audience:** Users who benefit from familiar identification and repeated interaction patterns, especially users with cognitive or memory impairments.
- **Success Criterion:** The same function looks and behaves the same way on each matching chart, including user-selected settings.

## Do not force sameness across different functions <!-- role: exceptions -->

**Break it when:** The charts do not perform the same task or function. **Why:** The source requires carried-over styling and interaction defaults specifically for charts that perform the same function.

## Consistency limits per-chart variation <!-- role: costs -->

**Sacrifice:** You give up some freedom to style or bind controls differently on each chart.
**Risk:** Reusing the same pattern on charts with different functions can imply a sameness that is not real.
**Mitigation:** Standardize only the charts that share the same task or function.

## Common cross-chart inconsistency failures <!-- role: mistakes -->

- **Mistake:** Charts with the same function use different default styles or ignore the user's chosen settings. **Why it fails:** Users cannot rely on a stable presentation from chart to chart.
- **Mistake:** Charts with the same function use different keybindings or interaction patterns. **Why it fails:** The same task must be relearned on each chart.

## Check repeated functions for shared defaults <!-- role: check -->

**Failure Sign:** Two charts that do the same job look or behave differently, or one chart drops a setting the user already chose elsewhere.
**Quick Check:** Compare charts with the same function and verify that their default styling, settings, and keybindings match.
**Stronger Test:** Change a user setting, then repeat the same task on each matching chart and confirm that the presentation and interaction pattern carry over.

## Standardize the repeated chart behavior <!-- role: fix -->

- Align the default styling across charts that perform the same function.
- Apply the same user-selected settings to each chart with that function.
- Reuse the same keybindings for the same function across charts.
- Reuse the same interaction pattern for the same function across charts.
