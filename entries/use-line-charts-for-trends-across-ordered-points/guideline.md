---
id: use-line-charts-for-trends-across-ordered-points
title: Use a line chart to emphasize a trend across ordered points
bibliography: references.bib
description: For reading change across ordered data points, use a line chart instead
  of a bar chart on ordered values to improve readability and mitigate isolated point-by-point
  reading for viewers relying on common graph conventions.
labels:
- purpose:select
- basis:empirical
- task:trend
- chart:line:use
- chart:bar:avoid
- quality:readability:use
- lever:chart-family
- reading-mode:overview
---

## Choose lines for trends <!-- role: advice -->

Choose a line chart when the main message is how values change across an ordered sequence. For example, connect successive measurements with a line when you want viewers to read the overall rise or fall rather than treat each point as a separate category.

## Why lines fit trends <!-- role: reason -->

Readers expect a line to express a connected progression. That expectation helps them extract the overall direction of change instead of focusing only on isolated point-by-point differences.

**Mechanism:** A line chart organizes the points into one continuous structure, which guides attention toward trend across the sequence.

**Evidence:** The paper explains that readers implicitly treat line graphs as highlighting trends across multiple data points and contrasts this with the comparison-focused reading encouraged by bar graphs [@zacksDesigningGraphsDecisionMakers2020].

## Use when the message is overall change <!-- role: context -->

- **User Goal:** Understand rise, fall, or other overall pattern across an ordered sequence.
- **Task:** Trend reading.
- **Data:** Multiple values arranged in meaningful order.
- **Chart Setting:** A single series or comparable ordered points on one common scale.
- **Audience:** Readers using common graph conventions.
- **Success Criterion:** Readers describe the direction or pattern of change.

## Do not use when the task is comparing discrete groups <!-- role: exceptions -->

**Break it when:** The main task is comparing named categories or separate groups. **Why:** Readers use bar charts to interpret comparisons between individual data points.

## Gain trend structure but lose category emphasis <!-- role: costs -->

**Sacrifice:** Individual point-by-point category comparisons become less prominent.
**Risk:** If the x positions are not meaningfully ordered, the line suggests continuity that is not really there.
**Mitigation:** Use bars when the x axis is categorical rather than ordered.

## Avoid flattening a trend into separate categories <!-- role: mistakes -->

**Mistake:** Using bars when the message is the trend across the series. **Why it fails:** Readers focus on isolated values instead of the overall change.

## Compare the trend cue directly <!-- role: check -->

**Failure Sign:** Readers report only point-by-point differences and miss the overall direction.
**Quick Check:** Show a bar and line version to a few viewers and ask what pattern they see first.
**Stronger Test:** Keep the version that elicits trend descriptions rather than isolated comparison statements.

## Replace category marks with a connected sequence <!-- role: fix -->

- Replace separate bars with a connected line.
- Keep the order explicit on the x axis.
- Remove bar-specific emphasis when the trend is the message.
