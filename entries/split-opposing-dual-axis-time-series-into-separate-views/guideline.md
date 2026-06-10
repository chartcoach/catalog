---
id: split-opposing-dual-axis-time-series-into-separate-views
title: Split opposing dual-axis time series into separate views
bibliography: references.bib
description: For exact value retrieval in multi-measure ordered-time charts, prefer
  a multi-view layout over a single-view dual-axis layout to improve fidelity and
  mitigate value-readout errors for general readers.
labels:
- purpose:select
- basis:empirical
- task:retrieve
- time:ordered-time
- structure:small-multiples:use
- structure:single-view:avoid
- quality:fidelity
- lever:layout-structure
- measure:multi
---

## Separate measures into aligned views <!-- role: advice -->

Split measures into separate aligned views when one chart would otherwise require opposing y-axes. For example, replace a single dual-axis time-series chart with two side-by-side panels that share time, and encode a negative quantity with bars connected to the zero baseline instead of reading it from a reversed second axis.

## Why separate views work for lookup <!-- role: reason -->

Separate views reduce scale conflict. Readers can decode each measure against its own axis instead of first deciding which of two incompatible y-axes applies.

**Mechanism:** One axis per measure simplifies exact lookup and makes the direction of each quantity easier to read.

**Evidence:** Across the study, redesigned charts improved knowledge-level value retrieval; in the markets case, the redesign replaced one chart with opposing positive and negative y-axes by two side-by-side charts and a zero-baseline bar for the negative series, while higher-level summaries and arguments for that chart stayed largely similar across versions [@burnsHowEvaluateData2020].

**Notes:** The supported gain in this case is mainly exact value retrieval, not a broad change in all higher-level interpretations.

## When separate views apply <!-- role: context -->

- **User Goal:** Locate and report exact values from two measures over time.
- **Task:** Exact retrieval from each series.
- **Data:** Two quantitative measures that would otherwise need separate scales, including cases where one measure is negative-valued.
- **Chart Setting:** A static time-series display with a shared time range.
- **Audience:** General readers.
- **Success Criterion:** Readers retrieve values correctly without decoding conflicting axes.

## When not to split into separate views <!-- role: exceptions -->

**Break it when:** The chart's main success criterion is the overall takeaway, trend summary, or argument rather than exact value lookup. **Why:** In the markets case, the split-view redesign did not materially change the kinds of summaries, trend descriptions, or policy arguments readers produced.

## Tradeoffs of separate views <!-- role: costs -->

**Sacrifice:** You give up some compactness from a single combined plot.\
**Risk:** Readers must compare across panels instead of within one plotting area.\
**Mitigation:** Keep the panels side by side and aligned on the same time range.

## Common dual-axis mistake <!-- role: mistakes -->

**Mistake:** Keep both measures in one plot with opposing y-axes when readers need exact values. **Why it fails:** Readers must first map each mark to a different scale, which increases readout difficulty.

## How to check the layout choice <!-- role: check -->

**Failure Sign:** Readers miss simple point-lookup questions on one or both measures.\
**Quick Check:** Compare a dual-axis draft and a split-view draft on one lookup question per measure; keep the version with fewer readout errors.\
**Stronger Test:** Run several value-retrieval questions on both versions and compare accuracy.

## How to fix a dual-axis time series <!-- role: fix -->

- Move each measure into its own panel.
- Align the panels on the same time span.
- Replace a reversed axis for a negative quantity with bars connected to the zero baseline.
- Keep the combined single view only if exact lookup is not the main success criterion.
