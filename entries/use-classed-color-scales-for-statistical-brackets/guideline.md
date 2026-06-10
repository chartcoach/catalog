---
id: use-classed-color-scales-for-statistical-brackets
title: Use a classed color scale to show predefined statistical brackets
bibliography: references.bib
description: For lookup tasks on quantitative choropleth maps, use a classed color
  scale to improve insight and mitigate missed threshold membership for readers checking
  whether areas fall into predefined ranges.
labels:
- purpose:refine
- basis:heuristic
- task:retrieve
- chart:choropleth
- data:quantitative
- quality:insight
- lever:encoding
- reading-mode:lookup
---

## Bin the threshold ranges <!-- role: advice -->

Use a classed color scale when the message is whether regions fall into predefined statistical brackets. For example, put all areas above or below a benchmark, in the top tenth, or beyond a standard-deviation cutoff into shared color bins instead of leaving every value on a continuous gradient.

## Make threshold membership visible <!-- role: reason -->

Threshold-based messages depend on group membership, not on every tiny numeric difference. Classes turn those thresholds into visible bins that readers can scan quickly.

**Mechanism:** Shared colors make the relevant brackets explicit, so readers can see which areas belong to each range instead of inferring that from subtle color shifts.

**Evidence:** The article says classed color scales are the right choice when the objective is to show whether regions fall into specific statistical brackets, such as above or below an average or inside a defined extreme group [@muth_classed_vs_unclassed_2021].

**Notes:** In this situation, the focus is on bracket membership rather than on the map's full continuous pattern.

## Use when the map answers an in-or-out question <!-- role: context -->

- **User Goal:** Show whether each region falls inside a predefined statistical range.
- **Task:** Identify threshold membership quickly.
- **Data:** Continuous quantitative values plus explicit cut points such as a benchmark, percentile, or deviation threshold.
- **Chart Setting:** A choropleth map with a legend that defines the brackets.
- **Success Criterion:** Readers can tell which regions belong to each bracket at a glance.

## Do not use when the goal is the overall pattern <!-- role: exceptions -->

**Break it when:** The goal is to show the general spatial pattern rather than bracket membership. **Why:** An unclassed scale shows broad gradients and subtle variation more directly.

## Accept the simplification <!-- role: costs -->

**Sacrifice:** You lose some numeric nuance inside each bracket.
**Risk:** The chosen cut points can dominate the interpretation.
**Mitigation:** Place class boundaries at the exact statistical thresholds you want to communicate.

## Avoid continuous colors for threshold messages <!-- role: mistakes -->

**Mistake:** Using an unclassed color scale when the message is above or below a benchmark. **Why it fails:** Readers have to infer threshold membership from small color differences instead of seeing it directly.

## Compare threshold reading across versions <!-- role: check -->

**Failure Sign:** Reviewers cannot quickly tell which regions are inside the target bracket.
**Quick Check:** Compare a classed and unclassed version and ask which one makes above/below-threshold membership easier to spot.
**Stronger Test:** Ask a reviewer to identify several regions against the threshold from the map alone, without relying on interaction.

## Encode the cut points directly <!-- role: fix -->

- Set class boundaries at the benchmark or other statistical cut points.
- Assign the same color to all regions in the same bracket.
- Rewrite the legend so the bracket boundaries are explicit.
