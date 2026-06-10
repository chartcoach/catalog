---
id: use-histogram-instead-of-box-plot-for-novice-distribution-reading
title: Use a histogram instead of a box plot for novice distribution reading
bibliography: references.bib
description: For distribution reading, prefer a histogram over a box plot on quantitative
  data to improve readability and mitigate dependence on quartile-based statistical
  knowledge for novice readers.
labels:
- purpose:select
- basis:empirical
- task:distribute
- chart:histogram:use
- chart:box-violin:avoid
- lever:chart-family
- quality:readability
- literacy:novice
---

## Choose the chart family for distribution reading <!-- role: advice -->

Use a histogram instead of a box plot when non-expert readers need to read a quantitative distribution. For example, show the distribution with bins and counts in a histogram, and avoid a box plot when the reader would need percentile, quartile, or interquartile-range knowledge before they can interpret the chart.

## Why the chart choice works <!-- role: reason -->

A histogram lets the reader inspect the displayed distribution directly. A box plot shifts the task toward statistical terminology that non-expert readers may not already know.

**Mechanism:** The histogram keeps the reading task on visible distribution shape and binned frequency. The box plot adds a prerequisite layer of percentile and quartile knowledge before the reader can interpret the marks.

**Evidence:** The VLAT was designed for non-expert users and explicitly excluded box plots because understanding them requires specific statistical knowledge such as percentile, quartile, and interquartile range, while histograms were retained in the test blueprint [@leeVLATDevelopmentVisualization2017].

## Use when the audience is reading a distribution <!-- role: context -->

- **User Goal:** Understand the shape or spread of a quantitative distribution.
- **Task:** Distribution reading by a non-expert audience.
- **Data:** One quantitative variable.
- **Chart Setting:** A static chart where the reader should interpret the display without prior statistical instruction.
- **Audience:** Novice or non-expert readers.
- **Success Criterion:** Readers can interpret the distribution without learning quartile-based terms first.

## Do not use when quartile knowledge is already part of the task <!-- role: exceptions -->

**Break it when:** The audience already knows percentile, quartile, and interquartile-range concepts, and those summaries are part of the intended message. **Why:** Then the extra statistical abstraction of a box plot is not a barrier.

## Tradeoffs of the chart swap <!-- role: costs -->

**Sacrifice:** You give up the compact quartile summary of a box plot.\
**Risk:** A histogram depends on binning choices, so the displayed shape reflects those bins.\
**Mitigation:** Use the histogram when the main goal is readable distribution interpretation by novices, not compact statistical summarization.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Using a box plot for a novice audience and expecting immediate distribution reading. **Why it fails:** The reader must first understand percentile and quartile concepts before the display becomes interpretable.

## How to test the choice <!-- role: check -->

**Failure Sign:** Readers ask what the box, whiskers, or quartiles mean before they can answer the distribution question.\
**Quick Check:** Compare a histogram and a box plot for the same data with a novice reviewer; keep the histogram if the box plot needs concept explanation first.\
**Stronger Test:** If the reader can answer the distribution question from the histogram but not from the box plot without teaching quartiles or percentiles, choose the histogram.

## What to change <!-- role: fix -->

- Replace the box plot with a histogram for the novice-facing version.
- Phrase the task around the visible distribution rather than quartile-based summaries.
- Remove explanations that are only needed to decode percentile or quartile terminology.
