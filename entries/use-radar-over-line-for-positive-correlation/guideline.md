---
id: use-radar-over-line-for-positive-correlation
title: Use a radar chart instead of a plain line chart for positive correlation judgments
bibliography: references.bib
description: For relate tasks, use a radar chart on positive-correlation displays
  instead of a plain line chart to improve fidelity and mitigate imprecise discrimination
  of nearby association strengths for readers judging correlation.
labels:
- purpose:select
- basis:empirical
- task:relate
- chart:radar:use
- chart:line:avoid
- quality:fidelity:use
- lever:chart-family
- operator:association
---

## Choose radar over plain line for positive correlation <!-- role: advice -->

Use a radar chart rather than a plain line chart when the display shows a positive correlation and readers must judge correlation strength. For example, if the same positive relationship can be shown as a plain Cartesian line chart or as its radar-form transform, keep the radar version and avoid the plain line version.

## Why the radar transform helps here <!-- role: reason -->

This is a bounded contrast within one task. The coordinate transform changed correlation precision enough to matter.

**Mechanism:** The radar chart yielded smaller JNDs than the plain positive line chart, so nearby positive association levels were easier to distinguish.

**Evidence:** For positive correlations, radar charts significantly outperformed plain line charts in the correlation experiment, and the 2023 review incorporated this result into its collated empirical knowledge for relate tasks [@harrisonRankingVisualizationsCorrelation2014; @zengReviewCollationGraphical2023].

## Use when positive correlation is the message and both forms are feasible <!-- role: context -->

- **User Goal:** Judge which display shows the stronger positive correlation.
- **Task:** Compare nearby association strengths.
- **Data:** Two quantitative variables shown as a positive-correlation pattern.
- **Chart Setting:** A single static display where radar and plain line versions are both feasible.
- **Success Criterion:** More reliable discrimination of nearby positive correlation values.

## Do not generalize this contrast to unsupported directions <!-- role: exceptions -->

**Break it when:** The same decision is being made for negative-correlation versions of radar and line charts. **Why:** The negative radar and negative line conditions were excluded as unreliable, so this contrast is only supported for the positive case.

## What you give up by replacing the line chart <!-- role: costs -->

**Sacrifice:** You give up the plain line-chart layout for this judgment task.
**Risk:** Extending this recommendation beyond positive-correlation reading goes beyond the supported evidence.
**Mitigation:** Keep this chart swap limited to positive-correlation judgment and test other cases separately.

## Common chart-choice mistake <!-- role: mistakes -->

**Mistake:** Treating the plain line chart and its radar transform as equivalent for positive correlation judgments. **Why it fails:** The experiment found a significant precision advantage for the radar version.

## How to test the choice <!-- role: check -->

**Failure Sign:** Readers struggle to distinguish nearby positive correlations in the plain line version.
**Quick Check:** Render matched radar and plain-line versions of the same positive-correlation data and compare them on close correlation values.
**Stronger Test:** Ask reviewers to make side-by-side stronger-correlation judgments in both versions and keep the one that yields more consistent answers.

## What to change <!-- role: fix -->

- Replace the plain positive line chart with the radar version for the correlation-reading step.
- Keep data, size, and correlation level matched when comparing the two versions.
- Re-test using close correlation pairs after the chart swap.
