---
id: reduce-aggregation-when-showing-observed-relationships
title: Reduce data aggregation when showing an observed relationship
bibliography: references.bib
description: For communicating observational relationships in grouped or binned quantitative
  displays, avoid high data aggregation on relational charts to improve fidelity and
  mitigate unwarranted causal interpretations for viewers reading summarized data.
labels:
- purpose:refine
- basis:empirical
- task:relate
- scope:grouped-result
- quality:fidelity:use
- lever:encoding
- operator:association
- group-cardinality:binary
---

## Lower the aggregation level <!-- role: advice -->

Keep more of the original paired values visible instead of collapsing the relationship into a few summary groups. For example, increase binning from 2 groups to 8 or 16 groups, or show non-aggregated values rather than a two-group summary.

## Why aggregation strengthens the causal reading <!-- role: reason -->

Strong aggregation turns a relationship into a few high-versus-low comparisons that are easy to read as cause and effect.

**Mechanism:** When many observations are compressed into only a few summary marks, viewers can interpret the display as evidence that moving from one group to another changes the outcome. Showing more bins or raw values weakens that simplified causal story.

**Evidence:** In Experiment 2, causation ratings were highest for the most aggregated displays and dropped as the same data were binned into more groups across bar, line, and dot encodings. A post-hoc comparison also found aggregated displays were judged more causal than comparable non-aggregated displays [@xiongIllusionCausalityVisualized2020].

**Notes:** The paper found this aggregation effect across multiple mark types, not only bar charts.

## When this applies <!-- role: context -->

- **User Goal:** Show association without making the relationship look causal.
- **Task:** Readers infer whether paired variables are merely correlated or could be causally linked.
- **Data:** Paired quantitative variables that can be binned or summarized.
- **Chart Setting:** Single-view bar, line, dot, or text-like summary that currently compresses many observations into a small number of groups.
- **Audience:** Readers interpreting observational or survey-style data.
- **Success Criterion:** Lower agreement with causal statements while retaining the ability to see the relationship.

## When this fails <!-- role: exceptions -->

**Break it when:** The display already shows non-aggregated values or already uses many bins. **Why:** The paper identified the risk as coming from stronger aggregation, so there is no further aggregation reduction left to apply.

## Tradeoffs of lower aggregation <!-- role: costs -->

**Sacrifice:** You lose some of the simplicity of a very compact summary.
**Risk:** Changing only the mark type while keeping a coarse grouped summary can leave the causal problem in place.
**Mitigation:** Revise the grouping first, then compare encodings if you still need to refine the display.

## Common failure around aggregation <!-- role: mistakes -->

**Mistake:** Split one variable into only two groups and report one average outcome for each group. **Why it fails:** The highest causal ratings appeared in the most aggregated conditions.

## How to test aggregation <!-- role: check -->

**Failure Sign:** A small number of marks stand in for many observations, especially a two-group split.
**Quick Check:** Count the groups or bins; a two-bin summary is the highest-risk condition tested in the paper.
**Stronger Test:** Recreate the same data with more bins or raw values and compare causal-agreement ratings across versions.

## What to change <!-- role: fix -->

- Increase the number of bins instead of collapsing the relationship into only two groups.
- Replace a grouped summary with non-aggregated paired values when possible.
- Remove text or chart treatments that frame the relationship only as a low-versus-high group comparison.
- Compare the final chart against a less aggregated version before publishing.
