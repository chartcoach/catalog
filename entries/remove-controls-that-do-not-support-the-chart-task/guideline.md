---
id: remove-controls-that-do-not-support-the-chart-task
title: Remove controls that do not support the chart's task
bibliography: references.bib
description: For interactive chart reading and task completion, avoid irrelevant controls
  and overly broad interaction on interactive charts to improve accessibility and
  mitigate unnecessary options and complexity for readers affected by cognitive load.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:interaction-access
- needs:cognitive
- polish:declutter
---

## Trim interaction controls <!-- role: advice -->

Remove controls and default interactions that do not directly support the chart's message, question, or task. For example, delete unused widgets and disable drag-select, click, or hover behavior when those interactions add no value for the reader.

## Why fewer controls help comprehension <!-- role: reason -->

Extra controls make readers inspect options before they can understand the chart. Narrowing the interaction scope keeps attention on the intended question and reduces unnecessary effort.

**Mechanism:** Removing irrelevant controls lowers cognitive load because readers do not have to evaluate useless options or navigate interaction paths that do not help them answer the chart's question.

**Evidence:** Chartability's Understandable heuristic says controls must not be irrelevant to the chart's message, question, or task, and that the chart's interactive scope must not be too broad; its notes report cognitive barriers when tools and applications expose more controls than necessary, including default drag-select, click, and hover behavior that provides virtually no value [@elavskyHowAccessibleMy2022]. The linked Inclusive Design "Add Value" principle advises including only controls and features that add value and avoiding unnecessary options and complexity [@inclusivedesignprinciples_add_value].

## Use when the chart has exposed interaction choices <!-- role: context -->

- **User Goal:** Understand the chart's message or answer a specific chart question.
- **Task:** Operate or inspect an interactive chart.
- **Chart Setting:** The chart, dashboard, tool, or application exposes widgets or default interactive behavior such as click, hover, or drag-select.
- **Audience:** Readers who may face cognitive barriers from excess options.
- **Success Criterion:** Every exposed control clearly supports the chart's message, question, or task.

## Do not remove controls that are necessary for the stated task <!-- role: exceptions -->

**Break it when:** A control directly supports the chart's message, question, or task, or is required to operate the chart. **Why:** Removing it would take away needed functionality rather than reduce cognitive load.

## Costs of narrowing interaction scope <!-- role: costs -->

**Sacrifice:** Readers get fewer ways to explore the chart.
**Risk:** A useful control can be removed by mistake if the task is not clearly defined.
**Mitigation:** Keep only the controls you can explicitly map to the chart's message, question, or task.

## Common over-interaction mistake <!-- role: mistakes -->

**Mistake:** Leaving default drag-select, click, or hover interactions enabled just because the tool provides them automatically. **Why it fails:** The chart exposes extra behavior that adds effort without adding value.

## Check whether every control earns its place <!-- role: check -->

**Failure Sign:** The chart contains controls or interactive behavior that do not change how the user answers the chart's question or understands its message.
**Quick Check:** For each visible control and default interaction, state the exact message, question, or task it supports; if you cannot name one, flag it.
**Stronger Test:** Temporarily disable a control or interaction; if the chart still works for its intended task, remove it.

## Remove or disable irrelevant interaction <!-- role: fix -->

- Remove visible controls that are not tied to the chart's message, question, or task.
- Disable default drag-select, click, or hover behavior when it does not add value.
- Narrow the interactive scope to the smallest set of functions needed for the intended task.
- Hide or turn off automatically exposed functionality when the tool adds it by default and it is not useful.
