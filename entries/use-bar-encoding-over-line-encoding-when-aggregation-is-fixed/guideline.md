---
id: use-bar-encoding-over-line-encoding-when-aggregation-is-fixed
title: Use bar encoding instead of line encoding when aggregation is fixed
bibliography: references.bib
description: For communicating non-temporal associations with the same aggregation
  level, prefer bar encoding over line encoding on grouped or paired-value displays
  to improve fidelity and mitigate stronger causal readings for viewers interpreting
  observational data.
labels:
- purpose:select
- basis:empirical
- task:relate
- time:non-temporal
- chart:bar:use
- chart:line:avoid
- quality:fidelity:use
- lever:chart-family
---

## Change the mark type while keeping the summary fixed <!-- role: advice -->

When the same grouped summaries or paired-value rows must stay intact, switch from a line encoding to a bar encoding to weaken causal interpretation. For example, keep the same 2-, 8-, or 16-bin summaries but draw bars instead of connected lines, or use bars rather than paired line traces on nominal index displays.

## Why bars read as less causal than lines here <!-- role: reason -->

Connected lines make a non-temporal relationship look more like a continuous trend, which can strengthen causal interpretation.

**Mechanism:** With the same data manipulation held constant, line segments emphasize continuity across values, while bars weaken that continuous causal-seeming trace. The change works only when the aggregation level does not also change.

**Evidence:** In Experiment 2, bar encodings received lower causation ratings than line encodings when both used the same binning levels. In Experiment 3, non-aggregated paired-value displays also showed lower causation ratings for bars than for lines [@xiongIllusionCausalityVisualized2020].

**Notes:** The paper also notes that two-bar bar charts appear to be a special case that can still invite strong causal interpretations.

## When this applies <!-- role: context -->

- **User Goal:** Reduce causal interpretation without changing which values are summarized.
- **Task:** Compare two encodings of the same observed relationship.
- **Data:** Non-temporal paired quantitative values, either binned into groups or aligned by a nominal index.
- **Chart Setting:** A line encoding is being considered for the same values that could also be shown as bars.
- **Audience:** Readers judging whether one variable could be causing the other.
- **Success Criterion:** Lower causal agreement while preserving the same aggregation level.

## When this fails <!-- role: exceptions -->

**Break it when:** The bar version and line version do not keep the same aggregation level. **Why:** The paper found aggregation level had a larger effect and can overwhelm the mark-type difference.

## Tradeoffs of switching from lines to bars <!-- role: costs -->

**Sacrifice:** You give up the continuous visual trace of the line.
**Risk:** A two-bar bar chart can still invite a strong causal reading.
**Mitigation:** If you choose bars, avoid collapsing the data into only two groups.

## Common failure around this choice <!-- role: mistakes -->

**Mistake:** Replace a bar encoding with a connected line while leaving the same grouped summaries in place. **Why it fails:** With aggregation held constant, line encodings were judged more causal than bar encodings.

## How to test this choice <!-- role: check -->

**Failure Sign:** The display connects non-temporal summarized values with line segments.
**Quick Check:** Redraw the same values as bars and compare the two versions side by side.
**Stronger Test:** Ask viewers to rate a causal statement for both versions and keep the lower-causality version.

## What to change <!-- role: fix -->

- Redraw the connected summaries as bars while keeping the same values and grouping.
- Keep aggregation constant when comparing the line and bar versions.
- If the current bar chart has only two groups, increase the number of groups before finalizing.
- Re-test the revised chart with the same causal-interpretation prompt.
