---
id: avoid-locking-chart-access-to-one-technology-path
title: Avoid locking chart access to one technology path
bibliography: references.bib
description: For digital chart access and interaction, avoid interaction-access that
  depends on a single browser, device, software environment, operating system, or
  input mechanism on charts to prevent fragile technology support and mitigate isolation
  of chart information or functionality for users of compliant assistive technologies.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:interaction-access
---

## Support multiple access paths <!-- role: advice -->

Do not make chart information or chart controls depend on one browser, device, software environment, operating system, or input mode. For example, let the same chart be used with keyboard, mouse, or touch, and verify that its information and functionality still work in more than one browser or operating system.

## Why multiple access paths matter <!-- role: reason -->

A chart becomes fragile when access depends on one technology path. Users who switch platforms or input methods can lose access to the same information or controls.

**Mechanism:** Supporting more than one platform and more than one input path keeps chart information and functionality available when users rely on different compliant assistive technologies or switch between input devices.

**Evidence:** Chartability defines fragile technology support as a robustness issue and states that chart access must not be isolated to one browser, device, software environment, or operating system; it requires diverse technological means to access chart information and functionality [@elavskyHowAccessibleMy2022]. WCAG’s concurrent input mechanisms guidance says users should be able to switch between keyboard, mouse, touch screen, and other input devices interchangeably, and that restricting specific inputs can exclude some users [@w3c_understanding_concurrent].

## When to apply cross-technology support <!-- role: context -->

- **User Goal:** Read the chart and use any provided chart interaction.
- **Chart Setting:** The chart is delivered digitally and may be opened in different browsers, devices, software environments, or operating systems, or used with different input mechanisms.
- **Audience:** People may rely on compliant assistive technologies or switch among keyboard, mouse, touch, or other input devices.
- **Success Criterion:** The same chart information and chart functionality remain available without forcing one specific platform or input mode.

## When input switching is not the review target <!-- role: exceptions -->

**Break it when:** The chart exposes information but has no interactive chart functionality to operate. **Why:** The input-switching part of the rule no longer changes the experience; focus on whether the chart information still remains available across browsers, devices, software environments, and operating systems.

## Tradeoffs of broader technology support <!-- role: costs -->

**Sacrifice:** You give up the convenience of relying on one preferred platform or one preferred input mode.\
**Risk:** A chart can appear available in another environment while still losing key information or controls.\
**Mitigation:** Compare the same chart information and the same chart functionality after switching platforms or input modes.

## Common isolation failures <!-- role: mistakes -->

- **Mistake:** Testing only one browser, device, software environment, or operating system. **Why it fails:** Access is still isolated if users must move to that one environment to reach the chart.
- **Mistake:** Supporting only one input mechanism, such as one gesture or one device class. **Why it fails:** Users cannot switch to the input mode or assistive technology they need.

## How to test technology support <!-- role: check -->

**Failure Sign:** The chart works only in one browser, device, software environment, or operating system, or only with one input mechanism.\
**Quick Check:** Open the chart in a second environment and repeat the same reading or interaction path with a second input mechanism such as keyboard instead of mouse.\
**Stronger Test:** Verify that the same chart information and the same chart functionality remain available after switching among keyboard, mouse, and touch and after moving to another supported platform.

## How to repair isolated support <!-- role: fix -->

- Remove chart behaviors that require one specific browser, device, software environment, or operating system.
- Expose the same chart controls through more than one input mechanism, such as keyboard plus mouse or touch.
- Rework any platform-specific behavior until the same chart information and functionality are available in each tested environment.
- If one environment cannot support the chart interaction, add another technological means to access the same chart information and functionality.
