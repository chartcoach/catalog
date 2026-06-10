---
id: provide-undo-redo-for-interactive-visualization-actions
title: Provide undo and redo for interactive visualization actions
bibliography: references.bib
description: For interactive tasks, use reversible interaction controls on interactive
  visualizations to improve accessibility and mitigate interaction mistakes for users
  with disabilities and users of assistive technologies.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:interaction-access
---

## Reversible interaction controls <!-- role: advice -->

Make every interactive visualization action reversible. For example, when a chart interaction changes state or performs a task, add both an undo action and a redo action for that operation.

## Why reversible actions matter <!-- role: reason -->

Reversible controls turn interaction errors into recoverable steps. They let a user explore, make a mistake, and return to the previous state instead of getting trapped by a changed chart state or failed operation.

**Mechanism:** Undo and redo add tolerance to interactive chart workflows by giving users a direct recovery path after an accidental or unwanted action.

**Evidence:** Chartability defines unforgivable interactions as an accessibility problem in interactive visualizations and states that users must be able to both undo and redo their actions. Error-tolerant design research recommends undo, redo, and recovery paths because users will make mistakes and interfaces should tolerate them [@elavskyHowAccessibleMy2022; @baber_task_analysis_1994].

**Notes:** This rule applies beyond data-entry fields. The source notes that interaction errors in data experiences can be more complex than the narrow cases covered by form-focused error-prevention criteria.

## Use when interaction errors can happen <!-- role: context -->

- **User Goal:** Complete a task in an interactive visualization and recover from a mistaken action if needed.
- **Task:** Operate a visualization that changes state or performs an action.
- **Chart Setting:** The visualization is interactive or has the ability to perform a task.
- **Audience:** Users with disabilities and users of assistive technologies.
- **Success Criterion:** After an action, the user can reverse it and reapply it.

## Do not require it on static views <!-- role: exceptions -->

**Break it when:** The visualization is static and performs no interactive task or operation. **Why:** There is no user action to undo or redo.

## Costs of reversible controls <!-- role: costs -->

**Sacrifice:** The interface must support additional recovery actions.
**Risk:** If only some interactive actions are reversible, users can still get stuck on the remaining ones.
**Mitigation:** Apply the same undo-and-redo pattern to each action that changes the visualization state or performs a task.

## Irreversible interaction changes <!-- role: mistakes -->

**Mistake:** Let a chart interaction change the visualization state without any undo or redo path. **Why it fails:** A normal user mistake becomes an accessibility barrier instead of a recoverable step.

## How to test reversal <!-- role: check -->

**Failure Sign:** After performing an interactive action, there is no way to return to the previous state and no way to reapply the reversed action.
**Quick Check:** Perform one chart action, then try to undo it and redo it.
**Stronger Test:** Repeat that check for each distinct task or state-changing interaction the visualization supports.

## What to change <!-- role: fix -->

- Add an undo action for each interaction that changes the visualization state or performs a task.
- Add a matching redo action that restores the undone state.
- Review every interactive operation in the visualization and add the same recovery path wherever a user can make a mistake.
