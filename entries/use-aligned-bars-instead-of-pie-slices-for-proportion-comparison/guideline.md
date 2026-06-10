---
id: use-aligned-bars-instead-of-pie-slices-for-proportion-comparison
title: Use an aligned bar chart instead of a pie chart for proportion comparison
bibliography: references.bib
description: For compare tasks, use bar charts on a common scale rather than pie charts
  to improve fidelity and address errors from judging slice angles for readers making
  exact value judgments.
labels:
- purpose:select
- basis:empirical
- task:compare
- chart:bar:use
- chart:pie-donut:avoid
- data:quantitative
- quality:fidelity:use
- lever:chart-family
- reading-mode:exact
---

## Bar chart over pie chart <!-- role: advice -->

Use an aligned bar chart when readers must judge how large one quantitative value is relative to another. For example, show the marked values as bars on a common linear scale instead of pie slices judged by angle.

## Why aligned bars beat pie slices here <!-- role: reason -->

An aligned bar chart puts both values on one scale, so the eye compares positions directly. A pie chart asks readers to judge angles, which is less precise for quick percentage estimation between marked values.

**Mechanism:** Common-scale bars reduce the comparison to a shared positional read. Pie slices require angle judgment, which adds more perceptual error in exact proportion tasks.

**Evidence:** In the collated ranking, the three aligned bar conditions all scored above the pie condition for accuracy, and each was significantly better than the pie condition under the reported 95% bootstrap test for proportional judgments [@zengReviewCollationGraphical2023; @heerCrowdsourcingGraphicalPerception2010].

## Use when choosing between bars and pie slices for exact reading <!-- role: context -->

- **User Goal:** Compare two marked quantitative values as a percentage or relative size.
- **Task:** Make a quick but accurate proportional judgment.
- **Data:** Quantitative values that could be shown either as bars or as slices.
- **Chart Setting:** A static single-view chart on a standard display, with an active choice between an aligned bar chart and a pie chart.
- **Audience:** Readers making quick visual judgments.
- **Success Criterion:** Higher accuracy in the proportion comparison.

## Do not treat this as a rule for every pie-chart use <!-- role: exceptions -->

**Break it when:** Exact proportional comparison between marked values is not the job of the chart. **Why:** This evidence only supports quick accuracy for that specific comparison task.

## Tradeoffs of replacing pie slices with bars <!-- role: costs -->

**Sacrifice:** You give up the angle-based pie form.\
**Risk:** Switching to bars without a common scale can erase the tested advantage.\
**Mitigation:** Keep the chosen bar chart aligned to one linear baseline.

## Common bar-versus-pie mistake <!-- role: mistakes -->

**Mistake:** Replacing the pie with a bar chart that still makes readers compare bars from unequal starting points. **Why it fails:** The supported advantage comes from aligned bar positions, not from any bar arrangement.

## Check the chart-family choice directly <!-- role: check -->

**Failure Sign:** The current design asks readers to compare slice angles for the main judgment.\
**Quick Check:** Make an aligned bar version of the same values and see whether the main comparison moves onto one shared axis.\
**Stronger Test:** Ask a reviewer to estimate the smaller value as a percent of the larger in both versions and keep the aligned bar chart if the answers are more consistent.

## Fix the chart-family choice <!-- role: fix -->

- Replace the pie slices with bars on a common linear scale.
- Mark the compared values directly on the bar chart.
- If the first bar version still uses unequal baselines, rework it into an aligned bar layout before finalizing the switch.
