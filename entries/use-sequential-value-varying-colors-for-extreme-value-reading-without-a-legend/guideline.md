---
id: use-sequential-value-varying-colors-for-extreme-value-reading-without-a-legend
title: Use sequential value-varying colors for extreme-value reading without a legend
bibliography: references.bib
description: For extreme-value lookup without a legend, prefer sequential value-varying
  color encoding on quantitative maps to improve accuracy and speed and mitigate misordered
  high-versus-low judgments for readers who must infer magnitude from color alone.
labels:
- purpose:refine
- basis:empirical
- task:extreme
- chart:map
- data:geospatial
- quality:fidelity:use
- lever:encoding
- channel:color-saturation:use
- channel:color-hue:avoid
---

## Sequential color order <!-- role: advice -->

Use a sequential value-varying color scheme when viewers must identify the highest or lowest values from color alone on a quantitative map. For example, on choropleth and isarithmic maps, replace a rainbow hue scheme with a sequential light-to-dark scheme when the task is to pick the maximum or minimum region without consulting a legend.

## Why sequential color order helps <!-- role: reason -->

A sequential scheme gives viewers a consistent perceptual order for low-to-high magnitude, which makes it easier to judge which mapped area is highest or lowest without first decoding hue categories.

**Mechanism:** Value-varying color supports direct high-versus-low judgments, while rainbow hue requires viewers to infer an order that is not consistently perceived.

**Evidence:** Participants were more accurate and faster with sequential schemes than with rainbow schemes for extreme-value tasks on both choropleth and isarithmic maps, and the collated ranking places both sequential conditions above both rainbow conditions [@zengReviewCollationGraphical2023; @golbiowskaRainbowDashIntuitiveness2022].

## Use when the map must reveal highs and lows directly <!-- role: context -->

- **User Goal:** Find which region has the highest or lowest value.
- **Task:** Identify extremes from color alone rather than from a legend.
- **Data:** Quantitative values encoded as filled geographic areas.
- **Chart Setting:** A choropleth or isarithmic map where the viewer must read the color order directly.
- **Success Criterion:** Higher accuracy and faster response when identifying maxima or minima.

## Do not use when the task is legend-assisted lookup <!-- role: exceptions -->

**Break it when:** The main task is legend-assisted value lookup rather than finding maxima or minima from color alone. **Why:** The study did not show the same sequential advantage across the other map-reading tasks, so this rule is task-specific.

## Tradeoffs of sequential color order <!-- role: costs -->

**Sacrifice:** You may give up performance advantages that rainbow color can have on some non-extreme tasks.
**Risk:** Reusing this palette rule for every map task can weaken performance when the job is not to judge high versus low directly.
**Mitigation:** Apply this rule specifically to no-legend extreme reading, then re-evaluate the palette for other tasks.

## Common palette mistake <!-- role: mistakes -->

**Mistake:** Keeping a rainbow hue scale for high-versus-low reading because viewers might learn the order over time. **Why it fails:** Partial learning does not remove the basic ordering problem, so viewers still make more errors and take longer than with a sequential scheme.

## How to test color order <!-- role: check -->

**Failure Sign:** Reviewers disagree about which color means the highest or lowest value when the legend is hidden.
**Quick Check:** Hide the legend and ask a few readers to point to the max and min regions.
**Stronger Test:** Compare the current rainbow version against a sequential version of the same map and see which one yields faster and more accurate max/min answers.

## How to revise the palette <!-- role: fix -->

- Replace the rainbow hue palette with a sequential value-varying palette on the area fill.
- Keep one consistent low-to-high order across the mapped areas and any supporting legend.
- Re-test the revised map on the exact max/min question with the legend removed.
- If the map’s main task changes to legend-assisted value lookup, reassess the palette instead of carrying this rule over unchanged.
