---
id: use-bar-charts-to-emphasize-discrete-comparison
title: Use bar charts to emphasize discrete value comparison
bibliography: references.bib
description: For discrete comparison between separate quantitative observations, prefer
  a bar chart on simple comparison displays to improve readability and mitigate unintended
  trend interpretations for readers.
labels:
- purpose:select
- basis:empirical
- task:compare
- chart:bar:use
- chart:line:avoid
- quality:readability:use
- lever:chart-family
---

## Bar chart selection <!-- role: advice -->

Choose a bar chart when the main job is to compare separate values as distinct observations. For example, use bars instead of a connected line when you want readers to compare amounts directly rather than infer a continuous trend.

## Why bars emphasize comparison <!-- role: reason -->

Bars steer readers toward discrete judgments. Even when the underlying values are identical to a line chart, the bar form frames them as separate quantities to compare.

**Mechanism:** The separated bar marks cue item-by-item comparison, while a connecting line suggests continuity and trend.

**Evidence:** The paper summarizes evidence that the same values receive different verbal interpretations depending on whether they are shown as bars or lines: bars prompt discrete comparisons, while lines prompt trend descriptions [@bertiniWhyShouldntAll2020].

## Use when comparison is the intended interpretation <!-- role: context -->

- **User Goal:** Compare separate quantities directly.
- **Task:** Discrete comparison rather than trend reading.
- **Data:** Separate observations that should not be read as one continuous trajectory.
- **Chart Setting:** You are choosing between a bar chart and a line chart for the same values.
- **Audience:** Readers who need the chart to cue direct comparison.
- **Success Criterion:** Readers describe which values are larger or smaller rather than talking about trend shape.

## Do not use when continuity is the message <!-- role: exceptions -->

**Break it when:** The main job is to show a continuous trend across an ordered sequence. **Why:** Bars encourage separate comparisons and weaken the continuity cue.

## Costs of using bars for comparison <!-- role: costs -->

**Sacrifice:** You give up the strong visual cue for continuous trend and shape.
**Risk:** Blind use can hide the intended rise, fall, or trajectory of the series.
**Mitigation:** Switch to a line when the audience should read the sequence as one continuous pattern.

## Common bar-chart misuse <!-- role: mistakes -->

**Mistake:** Using bars when the chart should communicate a continuous trend. **Why it fails:** The bar form invites discrete comparison instead of a trend interpretation.

## Check whether bars are the right choice <!-- role: check -->

**Failure Sign:** Reviewers describe the chart as a trend when you need direct comparison, or they struggle to compare separate amounts quickly.
**Quick Check:** Render the same values as both bars and a line, then ask a reviewer what the chart is mainly showing.
**Stronger Test:** Keep the version that makes reviewers compare separate amounts without prompting.

## Fix the chart choice <!-- role: fix -->

- Replace the connected line with bars for the separate observations.
- Keep the bars visually separate so each value reads as an independent quantity.
- Switch back to a line if reviewers keep reading the display as a trend instead of a comparison.
