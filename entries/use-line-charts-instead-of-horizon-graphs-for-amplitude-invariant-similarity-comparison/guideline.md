---
id: use-line-charts-instead-of-horizon-graphs-for-amplitude-invariant-similarity-comparison
title: Use line charts instead of horizon graphs when similarity should ignore amplitude
  and vertical offset changes
bibliography: references.bib
description: For similarity comparison in ordered-time views, use line charts on time-series
  displays instead of horizon graphs to improve readability and mitigate slower pattern
  matching for viewers comparing amplitude- and offset-varying signals.
labels:
- purpose:select
- basis:empirical
- task:compare
- time:ordered-time
- chart:line:use
- chart:area:avoid
- quality:readability:use
- lever:chart-family
---

## Choose the time-series chart family for amplitude-invariant similarity search <!-- role: advice -->

Use a line chart instead of a horizon graph when viewers must quickly judge which candidate time series is most similar to a query and differences in amplitude or y-offset should not break the match. For example, show the query and candidates as stacked line traces rather than banded horizon graphs when similarity is defined with z-normalization or another amplitude- and offset-invariant comparison.

## Why the chart swap works <!-- role: reason -->

Horizon-graph band boundaries turn small vertical differences into visible band and color changes, which slows matching when viewers are supposed to treat those differences as unimportant.

**Mechanism:** A line chart preserves the continuous shape without adding band thresholds, so viewers can compare overall form more quickly when amplitude or vertical shift is not the deciding factor.

**Evidence:** In the normalization experiment, line charts were faster than horizon graphs for choosing the most similar time series to a query, with mean completion times of 21.1 seconds for line charts versus 28.8 seconds for horizon graphs, and the collated result ranks the line-chart condition ahead of the horizon-graph condition with a significant pairwise difference [@gogolouComparingSimilarityPerception2019; @zengReviewCollationGraphical2023].

**Notes:** The source also found horizon graphs slower than the other tested designs in this condition.

## Use when these conditions all hold <!-- role: context -->

- **User Goal:** Choose the most similar candidate time series to a shown query.
- **Task:** Visual similarity comparison where amplitude and vertical-offset changes should be discounted.
- **Data:** Multiple time series shown over the same time window and common scale.
- **Chart Setting:** Stacked small-multiple views with equal or comparable vertical space per series.
- **Audience:** Viewers making subjective similarity choices rather than exact numerical readouts.
- **Success Criterion:** Faster selection of the closest matching pattern.

## Do not use when these conditions hold <!-- role: exceptions -->

- **Break it when:** Local temporal stretching or shifting is the main deformation you need viewers to tolerate. **Why:** The source did not show a significant speed advantage of line charts over horizon graphs in that warping condition.
- **Break it when:** Vertical compactness is the dominant design constraint. **Why:** Horizon graphs were introduced as a more space-efficient encoding, so replacing them with lines gives up that compression.

## Know the tradeoffs before you swap <!-- role: costs -->

**Sacrifice:** You give up the vertical space savings of the horizon graph.
**Risk:** A line chart uses more display height for the same time series.
**Mitigation:** Use the line chart when faster similarity judgment matters more than dense vertical packing.

## Watch for this failure mode <!-- role: mistakes -->

**Mistake:** Keeping a horizon graph when viewers should ignore amplitude and y-offset differences. **Why it fails:** Band thresholds can exaggerate exactly those differences and slow the match.

## Review the choice with a direct A/B test <!-- role: check -->

**Failure Sign:** Viewers hesitate longer with horizon graphs when matching amplitude- or offset-varying candidates to a query.
**Quick Check:** Show the same query-and-candidates set once as line charts and once as horizon graphs, then compare which version yields a faster confident choice.
**Stronger Test:** Time a small set of representative similarity judgments under your amplitude-invariant criterion and compare median completion times across the two chart families.

## Make the revision concretely <!-- role: fix -->

- Replace each banded horizon graph with a line trace for the same query and candidate series.
- Keep the same time window and common scale when you compare the two designs.
- Re-test the revised view on representative similarity prompts where amplitude or y-offset should not decide the answer.
- If compactness matters more than speed in your layout, keep the horizon graph and accept the slower matching.
