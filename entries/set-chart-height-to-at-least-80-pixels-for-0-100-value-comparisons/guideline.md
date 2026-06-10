---
id: set-chart-height-to-at-least-80-pixels-for-0-100-value-comparisons
title: Set chart height to at least 80 pixels for 0-100 value comparisons
bibliography: references.bib
description: For exact value comparison in static displays, use chart height of at
  least 80 pixels on bar and line charts with a 0-100 scale to improve fidelity and
  mitigate accuracy loss from undersized charts for web viewers.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:bar
- chart:line
- quality:fidelity
- lever:layout-structure
- reading-mode:exact
---

## Chart height <!-- role: advice -->

Increase chart height to at least 80 pixels when readers must compare values on a 0-100 scale. For example, in bar and line charts, revise a 40-pixel chart upward to 80 pixels, but do not expect extra accuracy gains from increasing the same chart to 160 or 320 pixels for this task alone.

## Why 80 pixels works <!-- role: reason -->

Very short charts compress the vertical distance that readers use to judge differences. Once the chart is tall enough that the pixel resolution roughly matches the data resolution, further height increases add little accuracy for this task.

**Mechanism:** A taller chart gives readers more vertical separation for tracing and comparing values, but the benefit plateaus once the display is no longer resolution-limited.

**Evidence:** In the chart-size experiment, 40-pixel charts produced significantly more error than 80-, 160-, and 320-pixel charts, while the larger heights did not differ significantly from each other. The paper concludes that increasing height beyond 80 pixels offers little accuracy benefit on a 0-100 scale. [@heerCrowdsourcingGraphicalPerception2010]

## Use when chart size is the bottleneck <!-- role: context -->

- **User Goal:** Compare marked values accurately.
- **Task:** Exact or near-exact difference reading.
- **Data:** Quantitative values shown on a 0-100 scale.
- **Chart Setting:** Static bar or line chart in a web display.
- **Audience:** Web viewers using standard displays.
- **Success Criterion:** Lower comparison error.

## Do not use this as a speed rule <!-- role: exceptions -->

**Break it when:** Your goal is to optimize response time, or your chart is outside the tested 0-100 bar/line setting. **Why:** The paper explicitly declined to make timing recommendations from the crowdsourced data, and the height finding was tested only on those chart types and scales.

## Costs of increasing chart height <!-- role: costs -->

**Sacrifice:** You use more vertical space.
**Risk:** Blindly making charts taller than 80 pixels can spend space without improving accuracy for this task.
**Mitigation:** Stop increasing height for accuracy once the chart reaches about 80 pixels on a 0-100 scale.

## Common height mistake <!-- role: mistakes -->

**Mistake:** Assuming that taller charts always improve value-comparison accuracy. **Why it fails:** The study found the accuracy benefit at 80 pixels, but not beyond it.

## How to check chart height <!-- role: check -->

**Failure Sign:** The chart is very short and readers make larger-than-expected value-comparison errors.
**Quick Check:** If a 0-100 bar or line chart is around 40 pixels tall, treat it as undersized for accurate comparison.
**Stronger Test:** Compare a 40-pixel version against an 80-pixel version on the same reading task and inspect error rates.

## How to fix chart height <!-- role: fix -->

- Increase a 0-100 bar or line chart from about 40 pixels to at least 80 pixels.
- If the chart is already 80 pixels or taller, do not enlarge it further for accuracy alone.
- Reserve larger heights for other needs, not because you expect better comparison accuracy from extra height by itself.
