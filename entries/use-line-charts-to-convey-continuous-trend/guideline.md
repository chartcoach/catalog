---
id: use-line-charts-to-convey-continuous-trend
title: Use line charts to convey continuous trend
bibliography: references.bib
description: For trend reading on ordered quantitative data, prefer a line chart on
  displays of sequential observations to improve readability and mitigate discrete-comparison
  interpretations for readers.
labels:
- purpose:select
- basis:empirical
- task:trend
- chart:line:use
- chart:bar:avoid
- quality:readability:use
- lever:chart-family
---

## Line chart selection <!-- role: advice -->

Choose a line chart when the main job is to show continuous change across an ordered sequence. For example, connect the observations with a line for trend displays and avoid bars when you want readers to read rise, fall, and shape rather than separate amounts.

## Why a line changes the reading task <!-- role: reason -->

A connected line changes what readers think the data is about. The same vertical positions can be read as separate quantities in bars or as a continuous trajectory in a line, so the chart family itself guides interpretation.

**Mechanism:** Connecting points creates an affordance for continuity and trend, while bars emphasize individual comparisons between discrete values.

**Evidence:** The paper summarizes evidence that people describe the same values differently in bars and lines: bars elicit discrete comparisons, while lines elicit trend descriptions. It uses this result to argue that chart choice should follow the intended interpretation, not only position precision [@bertiniWhyShouldntAll2020].

## Use when trend is the intended interpretation <!-- role: context -->

- **User Goal:** Explain change, direction, or overall shape across a sequence.
- **Task:** Trend reading rather than point-by-point comparison.
- **Data:** Sequential observations with a meaningful order and an implied continuity.
- **Chart Setting:** You are choosing between a bar chart and a line chart for the same values.
- **Audience:** Readers who need the chart to cue a trend interpretation.
- **Success Criterion:** Readers describe the series in terms of rise, fall, slope, or overall shape.

## Do not use when the values should stay discrete <!-- role: exceptions -->

**Break it when:** The main job is to compare separate values as independent observations. **Why:** The line introduces a continuity cue that can shift attention away from discrete comparisons.

## Costs of using a line for trend <!-- role: costs -->

**Sacrifice:** You give up some emphasis on separate item-by-item comparison.
**Risk:** Readers may infer continuity where the data should be treated as distinct observations.
**Mitigation:** Switch to bars when the message is comparison between separate values rather than trend.

## Common line-chart misuse <!-- role: mistakes -->

**Mistake:** Adding a connecting line when the values should be read as separate comparisons. **Why it fails:** The connection itself suggests continuity and trend.

## Check whether the line is the right choice <!-- role: check -->

**Failure Sign:** Reviewers talk about individual amounts instead of the overall trajectory.
**Quick Check:** Render the same data as both bars and a line, then ask a reviewer for a one-sentence description.
**Stronger Test:** Keep the version that makes reviewers describe the intended trend without prompting.

## Fix the chart choice <!-- role: fix -->

- Replace bars with a connected line across the ordered observations.
- Keep the ordered sequence visible so the line reads as one trajectory.
- Remove the line and switch to bars if reviewers keep treating the sequence as separate comparisons.
