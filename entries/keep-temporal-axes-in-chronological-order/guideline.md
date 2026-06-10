---
id: keep-temporal-axes-in-chronological-order
title: Keep temporal axes in chronological order
bibliography: references.bib
description: For overview trend reading in ordered-time bar charts, use chronological
  scale order on the temporal axis to improve fidelity and mitigate false time-sequence
  and trend readings for general readers.
labels:
- purpose:refine
- basis:empirical
- task:trend
- time:ordered-time
- chart:bar
- quality:fidelity
- lever:scale-order
- component:axis:use
---

## Chronological temporal ordering <!-- role: advice -->

Keep the temporal axis in calendar order when the chart is meant to show change over time. For example, reorder date labels left to right by time instead of sorting dates by value, and in grouped bars keep the subgroup sequence trackable across the date sequence rather than re-sorting bars within each date by severity.

## Why chronological order works <!-- role: reason -->

Chronological order preserves the chart's time-reading grammar. Readers can follow the sequence as a timeline instead of mistaking a ranking for a temporal trend.

**Mechanism:** Chronological ordering lets readers identify the earliest and latest points correctly and supports valid trend reading across the full series and within subgroups.

**Evidence:** In the study's temporal bar-chart case, the value-sorted version led all seven viewers to name the wrong earliest date, made viewers more likely to describe the trend as decreasing, and rarely surfaced the bi-modal pattern, while the chronological redesign supported correct date identification and more frequent recognition of the bi-modal shape [@burnsHowEvaluateData2020].

## When chronological order applies <!-- role: context -->

- **User Goal:** Explain how values changed over time.
- **Task:** Describe the overall trend or the trend within each subgroup.
- **Data:** Dated observations, especially with repeated subgroup series.
- **Chart Setting:** A static bar chart whose x-axis labels claim to show time.
- **Audience:** General readers who may not inspect axis order closely.
- **Success Criterion:** Readers identify the correct time sequence and describe the trend without inventing a false decline.

## When not to use chronological order as the main arrangement <!-- role: exceptions -->

**Break it when:** The chart's goal is to rank dates or within-date categories by largest or smallest values rather than to show change over time. **Why:** The paper notes that the value-sorted version was appropriate for questions about which days had the largest or smallest counts and which subgroups were highest or lowest within those days.

## Tradeoffs of chronological order <!-- role: costs -->

**Sacrifice:** The highest and lowest dates are less immediately surfaced than in a value-sorted display.\
**Risk:** Readers may need more effort to spot extrema from a chronological axis alone.\
**Mitigation:** If ranking is the real task, keep the sorted order only after removing time-series framing such as claims that the chart shows values "over time."

## Common temporal-ordering mistake <!-- role: mistakes -->

**Mistake:** Sort temporal labels by magnitude but keep a title or annotation that says the chart shows change over time. **Why it fails:** Readers interpret the display as a timeline and infer the wrong sequence and trend.

## How to check temporal ordering <!-- role: check -->

**Failure Sign:** Readers describe a steady decrease or name the wrong earliest date.\
**Quick Check:** Read the x-axis labels left to right; if calendar order is broken, the chart is not supporting time-series reading.\
**Stronger Test:** Ask a reader to identify the earliest date and describe the trend over time; if either answer is wrong, the ordering is failing.

## How to fix temporal ordering <!-- role: fix -->

- Reorder the temporal axis into calendar order.
- Stop sorting dates by magnitude when the chart's job is trend reading.
- If ranking dates is the actual goal, rewrite the title and annotation so the chart no longer claims to show change over time.
- If subgroup trends are still hard to follow, arrange repeated categories consistently across the chronological sequence.
