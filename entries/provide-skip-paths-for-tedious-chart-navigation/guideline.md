---
id: provide-skip-paths-for-tedious-chart-navigation
title: Provide skip paths for repeated or exhaustive chart navigation
bibliography: references.bib
description: For interactive navigation tasks, use skip paths and summary access on
  repeated or dense chart structures to improve accessibility and mitigate repeated-content
  and point-by-point traversal for keyboard and screen-reader users.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:interaction-access
- needs:keyboard-only
- needs:screen-reader
- needs:cognitive
- access:keyboard:use
---

## Reduce navigation labor <!-- role: advice -->

Add a direct navigation path past repeated content and past exhaustive mark-by-mark traversal when those steps are not essential. For example, add a skip target that lands on the chart’s main content, and add an annotation or textual summary for statistically or visually important regions so users do not have to visit every point or bar in sequence.

## Why skip paths work <!-- role: reason -->

Sequentially traversing repeated interface blocks or every mark in a dense chart increases time cost and working-memory load. A direct jump to the main chart content or to a summary of important regions reduces labor and keeps essential tasks from depending on exhaustive navigation.

**Mechanism:** Skip paths and summaries shorten the interaction path for non-pointer modalities and reduce the memory needed to hold place during long navigation.

**Evidence:** Chartability marks tedious navigation as a critical accessibility failure and requires repeated content to be skippable and essential tasks not to depend on significant labor; it also recommends comparing interaction count or time across pointer, keyboard, search, and voice paths [@elavskyHowAccessibleMy2022]. The bypass-blocks guidance requires mechanisms such as skip links or headings so keyboard and screen-reader users can jump past repeated content efficiently [@w3c_understanding_bypass].

**Notes:** Detailed exploration can remain available, but it should not be the only way to reach essential content or function.

## Use when navigation is long or repetitive <!-- role: context -->

- **User Goal:** Reach the main chart content or complete one chart task efficiently.
- **Task:** Sequential navigation or inspection through keyboard or screen reader rather than only by pointer.
- **Data:** Repeated structures or dense displays that create long traversal paths.
- **Chart Setting:** An interactive data experience with repeated interface blocks or many navigable marks.
- **Audience:** People using keyboard-only, screen-reader, or other assistive-technology navigation, including users affected by higher cognitive load.
- **Success Criterion:** Essential content or function is reachable without exhaustive traversal, and task effort is comparable across input paths.

## Do not add it when there is nothing to bypass <!-- role: exceptions -->

**Break it when:** The chart has no repeated content and no long sequential interaction path for the task being tested. **Why:** There is no navigation-labor gap to remove, so an added skip path does not solve a real accessibility problem.

## Tradeoffs of shortcut paths <!-- role: costs -->

**Sacrifice:** You add extra navigation targets, summaries, or annotations.
**Risk:** If the shortcut becomes the only route, low-level detail can be harder to access.
**Mitigation:** Keep detailed exploration available, but make the shortcut sufficient for essential tasks.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Leaving the only access path as repeated tab stops or point-by-point reading through every mark. **Why it fails:** The chart may be technically operable, but the task still takes much more time and working memory for assistive-technology users.

## How to test navigation effort <!-- role: check -->

**Failure Sign:** A pointer user can complete the task quickly, but a keyboard or screen-reader user must move through repeated controls or many marks one by one.
**Quick Check:** Count the interactions or time needed to do one chart task with a pointer and with sequential keyboard navigation.
**Stronger Test:** Verify that the user can skip repeated blocks and reach the chart’s main content or key summary without visiting every intermediate element.

## What to change <!-- role: fix -->

- Add a skip target that lands after repeated headers, menus, or other repeated blocks and directly on the chart’s main content.
- Add an annotation or textual summary for statistically or visually important regions so key findings are reachable without visiting every mark.
- Keep detailed point-by-point interaction available, but do not make it the only route to essential content or function.
- Re-measure the interaction count or time for the same task across pointer and sequential keyboard paths, and shorten the longer path.
