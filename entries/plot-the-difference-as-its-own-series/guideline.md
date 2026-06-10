---
id: plot-the-difference-as-its-own-series
title: Plot the difference as its own series when differences are the message
bibliography: references.bib
description: For difference comparison over ordered time, use a direct difference
  series on line charts to improve judgment fidelity and mitigate gap-reading errors
  for readers tracking change between two series.
labels:
- purpose:refine
- basis:empirical
- task:compare
- time:ordered-time
- chart:line
- quality:fidelity
- lever:encoding
- operator:difference
---

## Direct difference series <!-- role: advice -->

Plot the difference itself when the message is how far apart two time series are. For example, add a separate line of pairwise differences on its own common scale instead of asking readers to infer the difference from the changing gap between two curves.

## Why a direct difference series works <!-- role: reason -->

Readers do not naturally recover a clean difference pattern from the space between two curves. They tend to see whichever curves get closest in different regions, while a direct difference plot shows the actual rise and fall of the difference over time.

**Mechanism:** A direct difference series converts the task into reading values from one common scale. A curve-difference display leaves the reader to judge distances between moving lines, which obscures the intended behavior.

**Evidence:** The paper shows that curve-difference charts fail to convey even the gross qualitative behavior of the differences, while a direct Cartesian graph of the differences reveals the rise and descent clearly. It recommends plotting the differences on their own graph when differences are to be conveyed [@clevelandGraphicalPerceptionTheory1984].

## Use when the gap between series is the message <!-- role: context -->

- **User Goal:** See when the difference between two series grows, shrinks, or changes sign.
- **Task:** Compare two quantitative series across ordered time.
- **Data:** Two time-ordered quantitative series with an interpretable point-by-point difference.
- **Chart Setting:** A two-line or curve-difference display is being considered or already exists.
- **Audience:** Readers tracking changes in the difference over time.
- **Success Criterion:** The behavior of the difference is directly visible.

## Do not use when only the original series matter <!-- role: exceptions -->

**Break it when:** The message is the individual levels of the two original series rather than their difference. **Why:** The source recommends direct difference plots specifically when differences are the quantity to be conveyed.

## Tradeoffs of plotting the difference directly <!-- role: costs -->

**Sacrifice:** The difference gets its own plot or extra series instead of living only as a gap between lines.
**Risk:** If you keep only the gap display, readers may judge whichever curves are nearest in each region instead of the intended difference.
**Mitigation:** Show the original series and the direct difference plot together when both messages matter.

## Common failure with two-line comparisons <!-- role: mistakes -->

**Mistake:** Expect readers to read the changing gap between two curves as if it were a direct series. **Why it fails:** The eye tends to judge minimum spacing in different regions rather than the intended vertical difference pattern.

## Check whether the difference is visible <!-- role: check -->

**Failure Sign:** Readers describe where the curves look close or far apart but cannot describe the actual difference trend.
**Quick Check:** Ask where the difference grows and shrinks in the current gap display and in a direct difference plot of the same data.
**Stronger Test:** If the gap display does not preserve even the gross behavior of the differences, add the direct difference plot.

## Fix the display <!-- role: fix -->

- Compute the point-by-point difference between the two series.
- Plot that difference as its own line on a common vertical scale.
- If readers also need the original series, show them in a companion line chart rather than relying on the gap alone.
