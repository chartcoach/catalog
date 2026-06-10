---
id: use-independent-scales-in-small-multiple-time-series-when-ranges-differ-and-local-trends-matter
title: Use independent scales in small-multiple time series when ranges differ and
  local trends matter
bibliography: references.bib
description: For trend tasks on ordered-time small multiples, use independent scales
  on each panel to improve readability and mitigate visually flattened change when
  series ranges differ widely for analysts inspecting within-series trends.
labels:
- purpose:refine
- basis:empirical
- task:trend
- time:ordered-time
- chart:area
- structure:small-multiples
- quality:readability:use
- lever:scale-order
---

## Set panel scales to local ranges <!-- role: advice -->

Use an independent y-scale for each small-multiple time series when the ranges differ sharply and the task is to read each series' trend. For example, in a set of regional area charts, give each panel its own scale so a moderate rise in a low-range region does not appear visually constant because a high-range region sets the global maximum.

## Preserve visible change within each panel <!-- role: reason -->

A common scale across very unequal series compresses smaller-range panels. That makes meaningful local change hard to see, even when the numbers do change.

**Mechanism:** Independent scales preserve perceptible variation within each panel, which helps viewers read the shape of change for that series.

**Evidence:** The paper explains that separate scales were used for each regional area chart to emphasize trends for specific regions, and it notes that using the same scale for all panels would make a smaller-range series appear constant because the relevant difference would be hard to perceive on the global scale [@olaSimpleChartsDesign2016].

## Use when within-series trend is the main task <!-- role: context -->

- **User Goal:** See how each series changes over time.
- **Task:** Compare local trend shape within each panel rather than exact magnitude across panels.
- **Data:** Multiple time series with strongly different value ranges.
- **Chart Setting:** Small-multiple area charts or similar repeated time-series panels.
- **Success Criterion:** Meaningful change remains visible in lower-range panels.

## Do not use when exact cross-panel magnitude comparison is the main task <!-- role: exceptions -->

**Break it when:** The primary task is to compare absolute levels directly across panels. **Why:** Independent scales emphasize local trend and weaken direct absolute comparison between panels.

## Trade off cross-panel magnitude comparison against local trend visibility <!-- role: costs -->

**Sacrifice:** You give up a single shared scale for exact cross-panel magnitude reading.
**Risk:** Viewers may over-compare panel heights that were scaled independently.
**Mitigation:** Use independent scales only when within-panel trend detection is the main goal.

## Avoid forcing all panels onto one dominant scale <!-- role: mistakes -->

**Mistake:** Using one common y-scale across small multiples with highly unequal ranges when the task is trend reading. **Why it fails:** Smaller-range series become visually flattened and can look unchanged.

## Test whether smaller-range panels look falsely constant <!-- role: check -->

**Failure Sign:** A panel with real numeric change looks nearly flat because another panel has a much larger range.
**Quick Check:** Render the same panels once with a common scale and once with independent scales and check whether local change becomes visible.
**Stronger Test:** Ask a reviewer to identify trend direction in a low-range panel; if they miss it on the shared-scale version, the scaling choice is hiding the pattern.

## Re-scale the small multiples for local trend reading <!-- role: fix -->

- Assign each small-multiple panel its own y-scale.
- Re-check whether lower-range panels now show visible increases or decreases.
- If exact cross-panel magnitude comparison becomes the main task, switch back to a shared scale or a different comparison view.
