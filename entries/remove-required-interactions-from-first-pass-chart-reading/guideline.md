---
id: remove-required-interactions-from-first-pass-chart-reading
title: Remove required interactions from the first reading of a chart
bibliography: references.bib
description: For initial reading and interpretation, avoid required interaction access
  on chosen charts to improve fidelity and mitigate extra task demands for novice
  readers.
labels:
- purpose:refine
- basis:empirical
- lever:interaction-access
- quality:fidelity
- literacy:novice
---

## Remove required interactions from the first pass <!-- role: advice -->

Remove interaction techniques when the chart's job is initial reading and interpretation. For example, show the first view statically instead of making readers discover sorting, brushing, or axes reordering before they can answer basic questions.

## Why fewer interactions help first-pass reading <!-- role: reason -->

First-pass reading should test or support interpretation of the visual encoding itself. Requiring interaction adds a second task: discovering and operating the controls.

**Mechanism:** Static presentation keeps the reader focused on reading the chart. Required interaction can hide the answer behind control discovery and introduce extra complexity before the reader has even understood the display.

**Evidence:** The VLAT intentionally excluded interaction techniques because people have limited ability to detect embedded interaction initially, interaction can invite additional complex tasks, and elaborate interaction can make the task more like reading text than reading visually represented data [@leeVLATDevelopmentVisualization2017].

## Use when the goal is first-pass interpretation <!-- role: context -->

- **User Goal:** Read and interpret the chart on first exposure.
- **Chart Setting:** The view is being used for initial comprehension or literacy assessment.
- **Audience:** Novice or non-expert readers.
- **Success Criterion:** Performance reflects reading the chart, not discovering controls.

## Do not use when interaction itself is the target skill <!-- role: exceptions -->

**Break it when:** The goal is to teach or assess the interaction technique itself. **Why:** Then sorting, brushing, or reordering is part of the intended skill rather than a confound.

## Tradeoffs of removing interaction <!-- role: costs -->

**Sacrifice:** You give up exploratory flexibility in the initial view.\
**Risk:** A static first view may not expose all of the chart's analytic capabilities.\
**Mitigation:** Separate first-pass reading from later interaction training instead of mixing them into the same step.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Hiding the first answer behind an interaction that the reader must discover. **Why it fails:** The chart now measures control discovery as much as chart interpretation.

## How to test the chart <!-- role: check -->

**Failure Sign:** Readers must ask how to use the chart before they can answer the first question.\
**Quick Check:** Ask whether the first task can be completed without any interaction.\
**Stronger Test:** If you must explain sorting, brushing, or reordering before basic reading can begin, the interactions are confounding first-pass interpretation.

## What to change <!-- role: fix -->

- Freeze the initial state so the first reading task is answerable without interaction.
- Remove required interactions from the first set of questions or explanations.
- Move interaction instruction into a separate tutorial or later workflow step.
