---
id: use-bar-charts-for-discrete-group-comparisons
title: Use a bar chart for comparisons across discrete groups
bibliography: references.bib
description: For comparing values across discrete groups, use a bar chart instead
  of a line chart on categorical data to improve fidelity and mitigate false trend
  interpretations for readers relying on common graph conventions.
labels:
- purpose:select
- basis:empirical
- task:compare
- chart:bar:use
- chart:line:avoid
- data:categorical
- quality:fidelity:use
- lever:chart-family
---

## Choose bars for separate groups <!-- role: advice -->

Choose a bar chart when the x positions are separate groups rather than a continuous progression. For example, show male versus female or age groups as separate bars instead of connecting the group summaries with a line.

## Why bars fit discrete comparisons <!-- role: reason -->

Readers bring learned expectations to graph formats. Bars cue comparison between separate values, while lines cue a trend across a sequence, so the wrong chart family can steer readers toward the wrong interpretation.

**Mechanism:** A bar chart directs attention to differences between categories instead of implying continuity or a trend between them.

**Evidence:** The paper reports that readers described bar versions of the same data in comparison terms, while line versions encouraged trend-like interpretations, including inappropriate continuous inferences for categorical data [@zacksDesigningGraphsDecisionMakers2020].

## Use when the message is one group versus another <!-- role: context -->

- **User Goal:** Compare one group to another.
- **Task:** Group comparison.
- **Data:** Summarized values for discrete categories.
- **Chart Setting:** One quantitative axis and one categorical axis.
- **Audience:** Readers using common graph conventions.
- **Success Criterion:** Readers describe the group comparison rather than an overall trend.

## Do not use when the main message is a trend across ordered points <!-- role: exceptions -->

**Break it when:** The main message is how values change across an ordered sequence. **Why:** Readers use line graphs to interpret trends across multiple data points.

## Accept less continuity to gain a cleaner comparison <!-- role: costs -->

**Sacrifice:** Bars downplay continuity across adjacent points.
**Risk:** Using bars on truly ordered trend data can push readers toward isolated comparisons instead of overall change.
**Mitigation:** Switch to a line chart only when trend is the intended message.

## Avoid implying continuity between categories <!-- role: mistakes -->

**Mistake:** Connecting discrete group summaries with a line. **Why it fails:** Readers may infer an ordered continuum or monotonic relation that the categories do not support.

## Compare the chart families directly <!-- role: check -->

**Failure Sign:** Readers describe the pattern as a trend instead of a group comparison.
**Quick Check:** Show a bar and line version to a few viewers and ask for the first sentence they would say about the data.
**Stronger Test:** Keep the version that elicits direct comparison statements rather than continuous-trend statements.

## Replace the misleading trend cue <!-- role: fix -->

- Replace the connecting line with separate bars.
- Keep the group names on the categorical axis.
- Remove the visual cue of continuity between categories.
