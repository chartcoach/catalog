---
id: use-dot-plots-for-average-comparisons-with-unequal-group-sizes
title: Use dot plots instead of bar graphs for average comparisons with unequal group
  sizes
bibliography: references.bib
description: For compare tasks on grouped quantitative displays where readers judge
  averages across groups of different sizes, use dot plots on raw-value charts to
  improve fidelity and mitigate summed-area judgments for readers interpreting group
  means.
labels:
- purpose:select
- basis:empirical
- task:compare
- scope:grouped-result
- chart:dotplot:use
- chart:bar:avoid
- quality:fidelity
- lever:chart-family
- operator:difference
---

## Switch from bars to dots for unequal-size group means <!-- role: advice -->

Use a dot plot instead of a filled bar graph when readers must decide which group has the higher average and the groups contain different numbers of observations. For example, show each value as a dot on a shared y-scale rather than as a set of filled bars, because bar area can stand in for the sum instead of the average.

## Why dots work better than bars here <!-- role: reason -->

Filled bars carry both value and area, so a group with more bars can look larger in total even when that does not match the average. Dots remove the filled-area cue and make the comparison depend more on overall position.

**Mechanism:** Unequal group sizes break the correlation between total filled area and average value. In bars, that mismatch harms mean judgments; dots reduce the area cue and support comparing average position more directly.

**Evidence:** In unequal set-size comparisons, dot graphs produced better discrimination than normal bar graphs, while normal bar graphs performed like misaligned length-only bars; performance also dropped sharply when unequal counts made summed area a poor proxy for average [@yuanPerceptualProxiesExtracting2019].

**Notes:** The experiments did not show a reliable dot-plot advantage when the compared groups had equal numbers of items.

## Use when group size differs across compared averages <!-- role: context -->

- **User Goal:** Decide which of two groups has the higher average.
- **Task:** Compare group means.
- **Data:** Quantitative observations shown as multiple raw values per group, with unequal numbers of observations across groups.
- **Chart Setting:** Static displays where each group's raw values are visible.
- **Success Criterion:** More accurate average comparisons when group sizes differ.

## Do not use this as a blanket replacement <!-- role: exceptions -->

- **Break it when:** The task is a single-value comparison rather than a group-mean comparison. **Why:** In 1vs1 comparisons, aligned bars were as precise as dots.
- **Break it when:** The compared groups have the same number of observations and unequal-count bias is not present. **Why:** The experiments did not show a reliable dot-plot advantage in that condition.

## Tradeoffs of switching to dots <!-- role: costs -->

**Sacrifice:** You replace aggregate-looking rectangles with individual points.
**Risk:** Unequal group size can still bias judgments in dot plots, because the more numerous group can influence the decision.
**Mitigation:** If the mean itself is the key message, represent the mean explicitly in addition to the dots.

## Common average-comparison mistake <!-- role: mistakes -->

**Mistake:** Using filled bars for unequal-size raw groups and expecting readers to extract the mean from bar tops alone. **Why it fails:** Readers can use total bar area as a proxy, and that breaks down when group sizes differ.

## How to check for summed-area bias <!-- role: check -->

**Failure Sign:** The group with more marks also looks like the larger total, even when its average is close to or below the other group.
**Quick Check:** Build a test case where the higher-average group has fewer observations and see whether the bar version becomes much harder to judge than a dot version.
**Stronger Test:** A/B test the same unequal-size comparison as a bar graph and as a dot plot, and compare accuracy on which group average is higher.

## How to fix unequal-size mean comparisons <!-- role: fix -->

- Replace each bar with a dot placed on the same value scale.
- Keep the two groups separate, but remove filled bar area as the dominant cue.
- Add an explicit mean representation if the chart's question is about the average.
- If the graphic must stay bar-based, avoid using it as the sole display for judging unequal-size group averages.
