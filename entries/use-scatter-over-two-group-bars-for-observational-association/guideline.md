---
id: use-scatter-over-two-group-bars-for-observational-association
title: Use a scatter plot instead of a two-group bar chart to show observational association
bibliography: references.bib
description: For communicating observational relationships in a single static view,
  prefer a scatter plot over a two-group bar chart on paired quantitative data to
  improve fidelity and mitigate unwarranted causal interpretations for viewers judging
  whether variables are related.
labels:
- purpose:select
- basis:empirical
- task:relate
- chart:scatter:use
- chart:bar:avoid
- quality:fidelity:use
- lever:chart-family
- operator:association
---

## Use raw-point association displays <!-- role: advice -->

Replace a two-group summary chart with a scatter plot when you want viewers to read an observed association without inferring an intervention-like effect. For example, show the paired observations as points instead of two summary bars split by an arbitrary threshold, and do not swap the chart for plain text that states the same two-group averages.

## Why raw points weaken the causal reading <!-- role: reason -->

Scatter plots expose the underlying pairwise variation instead of collapsing the relationship into a simple high-versus-low comparison.

**Mechanism:** Showing individual points makes viewers more likely to describe correlation and less likely to describe one variable as causing the other. Two-group bar summaries and matching text encourage grouped comparisons that make a causal story feel more plausible.

**Evidence:** In Experiment 1, scatter plots produced lower causation agreement than bar graphs and plain text for the same contextualized data, and participants generated fewer causal conclusions from scatter plots than from bar graphs or text [@xiongIllusionCausalityVisualized2020].

**Notes:** The paper found that much of this difference is tied to aggregation, so this contrast is strongest against a bar chart that collapses the relationship into two groups.

## When this applies <!-- role: context -->

- **User Goal:** Show that two variables move together without implying that changing one would change the other.
- **Task:** Readers judge whether an observed relationship is correlational or causal.
- **Data:** Paired quantitative variables shown with concrete variable labels.
- **Chart Setting:** Single-view, static communication such as a media or education-style graphic; the rejected alternative is a two-group summary bar chart.
- **Audience:** Readers who may default to a causal interpretation from simple observed data.
- **Success Criterion:** Readers still see the association but express weaker agreement with a causal statement.

## When this fails <!-- role: exceptions -->

**Break it when:** The chart must communicate a grouped summary rather than the raw pairwise relationship. **Why:** The paper showed that aggregation itself drives much of the causal impression, so a chart-family swap does not solve a design whose message depends on heavy grouping.

## Tradeoffs of raw-point association displays <!-- role: costs -->

**Sacrifice:** You give up the single, simple summary offered by two bars.
**Risk:** Rewriting the same two-group comparison as text keeps the causal problem.
**Mitigation:** If raw points are not possible, use a less aggregated summary instead of a two-group split.

## Common failure around this choice <!-- role: mistakes -->

**Mistake:** Replace the two-group bar chart with plain text that states the same grouped averages. **Why it fails:** The text condition produced similarly high causal ratings, so the grouped summary still invites a causal interpretation.

## How to test this choice <!-- role: check -->

**Failure Sign:** Readers restate the chart as “if X increased, Y would increase” instead of “X and Y tend to vary together.”
**Quick Check:** Make an A/B version of the same data as a scatter plot and as a two-group bar chart, then ask which one sounds more like an intervention claim.
**Stronger Test:** Collect open-ended interpretations or causal-agreement ratings and choose the version with fewer causal conclusions.

## What to change <!-- role: fix -->

- Replace the two summary bars with a scatter plot of the same paired observations.
- Remove the arbitrary threshold that splits the x-variable into two groups.
- Do not substitute a plain-text two-group summary for the chart.
- If you must summarize, increase the number of groups instead of collapsing to two.
