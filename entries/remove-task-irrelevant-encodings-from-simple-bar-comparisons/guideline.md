---
id: remove-task-irrelevant-encodings-from-simple-bar-comparisons
title: Remove task-irrelevant encodings from simple bar comparisons
bibliography: references.bib
description: For simple between-value comparison tasks, avoid task-irrelevant secondary
  encodings on bar charts to prevent competing relational interpretations and mitigate
  interference when viewers must compare one dimension at a time.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:bar
- quality:fidelity
- lever:encoding
- measure:multi
- group-cardinality:binary
---

## Remove competing encodings from the comparison <!-- role: advice -->

Keep only the task-relevant visual dimension varying when a bar chart asks readers for one simple comparison. For example, keep both bars the same lightness when readers must compare height, and keep both bars the same height when readers must compare lightness.

## Why a single varying dimension helps <!-- role: reason -->

Viewers do not read all possible relations from a graph at once. They use a task-dependent visual routine that locks onto one feature first, so an independently varying second feature can create a competing interpretation even when readers are told to ignore it.

**Mechanism:** Holding the non-target encoding constant removes an extra anchor point, so attention can follow the intended comparison without competing with another possible relation.

**Evidence:** In two-bar graphs, first saccades in the mixed-dimension task followed the anchor point from the task-relevant dimension, but responses were faster when the relevant and irrelevant preferred features fell on the same bar than when they fell on different bars, showing interference from the irrelevant dimension [@michalVisualRoutinesAre2017].

**Notes:** The strongest direct support is for simple two-bar comparisons using bar height and bar lightness.

## Use when one relation should dominate <!-- role: context -->

- **User Goal:** Judge one relation between two bars.
- **Task:** Compare one dimension while another visible dimension could imply a different comparison.
- **Data:** Two compared values, with more than one visual feature available to vary.
- **Chart Setting:** A bar chart where height and lightness could both vary within the same pair of bars.
- **Audience:** Viewers or students making a simple graph comparison one dimension at a time.
- **Success Criterion:** Readers extract the intended relation without slowing down or drifting to another plausible relation.

## Do not use when both dimensions must be read together <!-- role: exceptions -->

**Break it when:** Readers are supposed to compare both encoded dimensions in the same judgment. **Why:** The evidence supports suppressing an irrelevant dimension during a single intended comparison, not removing information that is itself part of the task.

## Costs of removing the extra encoding <!-- role: costs -->

**Sacrifice:** You give up a second simultaneously visible distinction inside the same two-bar comparison.
**Risk:** Applied blindly, this can hide a dimension that readers also need to inspect.
**Mitigation:** Keep the second dimension constant during the focal comparison, and only vary it when that second relation becomes part of the task.

## Common encoding failure <!-- role: mistakes -->

**Mistake:** Let both bar height and bar lightness vary when the chart asks for only one of those comparisons. **Why it fails:** The second varying feature creates a competing anchor point, which can slow the intended judgment when the two preferred features land on different bars.

## Check for competing relations <!-- role: check -->

**Failure Sign:** The same pair of bars supports two different simple readouts, such as one bar being taller while the other is darker.
**Quick Check:** Ask what single relation the viewer is meant to judge, then check whether another varying feature inside the same bar pair answers a different comparison.
**Stronger Test:** Compare the current chart with a version where the non-target feature is held constant; if the constant version yields faster and less conflicted judgments of the intended relation, keep the constant version.

## Fix the encoding conflict <!-- role: fix -->

- Hold the non-target visual dimension constant across the bars being compared.
- If height is the intended comparison, give the bars the same lightness.
- If lightness is the intended comparison, give the bars the same height.
- Do not ask readers to ignore a varying within-pair feature unless that feature is also meant to be compared.
