---
id: use-a-dual-axis-line-chart-when-correlation-is-the-main-message
title: Use a dual-axis line chart when correlation is the main message
bibliography: references.bib
description: For communicating the relationship in ordered-time paired series, prefer
  a dual-axis line chart over a connected scatterplot to improve insight and address
  missed positive or negative correlation cues for readers unfamiliar with connected
  scatterplots.
labels:
- purpose:select
- basis:empirical
- task:relate
- time:ordered-time
- chart:line:use
- chart:scatter:avoid
- quality:insight
- lever:chart-family
- operator:association
- literacy:novice
---

## Choose the chart family for correlation cues <!-- role: advice -->

Choose a dual-axis line chart when readers need to come away with a clear sense of positive or negative correlation. For example, use the line-chart form when parallel lines or an X-shape are the main takeaway, and avoid a connected scatterplot if the same data would make readers infer correlation from a single diagonal path.

## Why the dual-axis line chart works better for correlation <!-- role: reason -->

Readers already have learned visual associations between familiar line-chart patterns and correlation. Those learned cues do not transfer reliably to the diagonal segments of a connected scatterplot.

**Mechanism:** Parallel or crossing line patterns in a dual-axis line chart directly cue positive or negative relationships, while connected-scatterplot shapes draw attention to turns, loops, and path geometry instead.

**Evidence:** In the qualitative study, participants used correlational language far more often for dual-axis line charts than for connected scatterplots, and the paper concludes that a traditional dual-axis line chart may make positive or negative correlation much more salient when that is the intended takeaway [@harozConnectedScatterplotPresenting2016].

## Use when correlation is the takeaway <!-- role: context -->

- **User Goal:** Explain whether two measures move together or in opposite directions.
- **Task:** Help readers identify a positive or negative relationship.
- **Data:** Two simultaneous time series with matched sampling.
- **Chart Setting:** A static presentation graphic for paired time series.
- **Audience:** Readers who have much more experience with line charts than with connected scatterplots.
- **Success Criterion:** Readers explicitly describe a direct or inverse relationship.

## Do not use when another message matters more <!-- role: exceptions -->

**Break it when:** The main goal is to attract initial attention or to highlight distinctive loops, crossings, or L-shapes in the paired series. **Why:** The paper found that readers prioritized connected scatterplots for viewing and repeatedly noticed their unusual shapes.

## Costs of switching to a dual-axis line chart <!-- role: costs -->

**Sacrifice:** You give up the distinctive loop and L-shape patterns that connected scatterplots make visually salient.\
**Risk:** Intersections in a dual-axis line chart are only meaningful when the units and scales of the two vertical axes are the same.\
**Mitigation:** Do not rely on line intersections as evidence of a relationship unless the two vertical scales are directly comparable.

## Common chart-choice failure <!-- role: mistakes -->

**Mistake:** Use a connected scatterplot for a correlation takeaway without teaching readers how its diagonal segments encode association. **Why it fails:** Readers tend to describe the shape and motion of the path instead of stating a direct or inverse relationship.

## Check which chart makes correlation more explicit <!-- role: check -->

**Failure Sign:** Readers talk about loops, turns, or erratic motion but do not name a positive or negative relationship.\
**Quick Check:** Show naive readers both the connected scatterplot and the dual-axis line chart and ask for the main relationship message.\
**Stronger Test:** Keep the version that yields more explicit direct or inverse relationship language.

## Fix a missed-correlation presentation <!-- role: fix -->

- Replace the connected scatterplot with a dual-axis line chart when the main message is correlation.
- Keep the same paired series and time span so the chart-family change is the only difference.
- If you keep the connected scatterplot, annotate the positive or negative relationship directly.
