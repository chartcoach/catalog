---
id: use-few-classes-for-value-range-reading
title: Use a classed color scale with few classes when readers need value ranges
bibliography: references.bib
description: For exact or near-exact lookup on quantitative choropleth maps, use a
  classed color scale with few classes to improve readability and mitigate uncertain
  value estimates for readers who cannot rely on interaction.
labels:
- purpose:refine
- basis:heuristic
- task:retrieve
- chart:choropleth
- data:quantitative
- quality:readability
- lever:encoding
- reading-mode:exact
---

## Limit the number of classes <!-- role: advice -->

Use a classed color scale with only a few classes when readers must read value ranges from the map. For example, on static maps in print or PDF, define a small set of labeled ranges instead of asking readers to infer values from a continuous gradient or from many narrowly spaced bins.

## Improve range estimation from color <!-- role: reason -->

Readers can place an area into a labeled range more reliably than they can estimate a precise value from a continuous color. That benefit shrinks as the number of classes grows.

**Mechanism:** A small set of clear bins turns color into readable ranges, while too many bins or an unclassed gradient forces readers into guesswork.

**Evidence:** The article says classed maps have an advantage over unclassed maps in value-estimation tasks and adds that the benefit falls as the number of classes increases, especially when the map is static and readers cannot hover for tooltips [@muth_classed_vs_unclassed_2021].

## Use when the map must support printed lookup <!-- role: context -->

- **User Goal:** Let readers read or estimate value ranges from the map itself.
- **Task:** Assign regions to labeled numeric ranges.
- **Data:** Continuous quantitative values.
- **Chart Setting:** A static choropleth map, especially in print or PDF, where tooltips are unavailable.
- **Success Criterion:** Readers can identify the correct range for a region from the legend and colors alone.

## Do not use when the priority is nuance <!-- role: exceptions -->

**Break it when:** The priority is to preserve subtle differences, local contrasts, or continuous pattern. **Why:** Few classes hide variation inside each bin.

## Accept the loss of fine detail <!-- role: costs -->

**Sacrifice:** You give up within-bin detail.
**Risk:** Adding many classes weakens the readability benefit.
**Mitigation:** Keep the class count low enough that the ranges are still easy to read.

## Avoid overclassing the map <!-- role: mistakes -->

**Mistake:** Using many classes when the map's job is value-range reading. **Why it fails:** Readers become less likely to identify the correct ranges.

## Test range reading without hover <!-- role: check -->

**Failure Sign:** Reviewers can only make vague guesses about a region's range from the printed legend.
**Quick Check:** Ask a reviewer to place several regions into legend ranges without interaction.
**Stronger Test:** Compare a few-class version against an unclassed or many-class version and keep the one that supports more confident range assignments.

## Simplify the bins <!-- role: fix -->

- Reduce the class count to a small set of labeled ranges.
- Rewrite the legend so each bin boundary is explicit.
- Replace an unclassed or overclassed scale when the map must work without hover.
