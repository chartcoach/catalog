---
id: add-subgroup-views-beside-the-aggregate-scatterplot
title: Add subgroup views beside the aggregate scatterplot when trends may reverse
bibliography: references.bib
description: For grouped relationship analysis, use a multi-view subgroup breakdown
  on scatterplots to improve trust and mitigate the risk that the aggregate trend
  hides within-group reversals for readers interpreting associations.
labels:
- purpose:refine
- basis:empirical
- task:relate
- scope:grouped-result
- chart:scatter
- structure:multi-view:use
- quality:trust
- lever:layout-structure
---

## Subgroup breakdown next to the aggregate <!-- role: advice -->

Add subgroup views beside the aggregate scatterplot when the data are grouped and the within-group relationship may differ from the overall relationship. For example, keep the combined scatterplot, but also show each group separately so an overall positive correlation is not mistaken for positive within-group trends when each subgroup slopes downward.

## Why the subgroup breakdown works <!-- role: reason -->

Aggregate patterns can contradict subgroup patterns. Showing both levels lets readers see whether the overall direction is stable or whether combining groups has changed the apparent relationship.

**Mechanism:** Separate subgroup views expose within-group slopes that are hidden when all points are pooled into one correlation or one combined scatterplot.

**Evidence:** The paper's Simpson's paradox example preserves a positive overall Pearson correlation while arranging the grouped subsets so that each individual subgroup has a negative correlation, demonstrating that aggregate and within-group trends can disagree [@matejkaSameStatsDifferent2017].

## When this applies <!-- role: context -->

- **User Goal:** Interpret a relationship in grouped data.
- **Task:** Compare the overall association with the within-group association.
- **Data:** Paired quantitative observations divided into meaningful groups.
- **Chart Setting:** The current scatterplot pools all groups into one aggregate view.
- **Audience:** Readers may otherwise rely on one overall trend or one reported correlation.
- **Success Criterion:** Readers can see whether group-level trends match or reverse the aggregate trend.

## When not to add subgroup views <!-- role: exceptions -->

**Break it when:** The data do not contain meaningful groups to compare. **Why:** There are no within-group trends to contrast against the aggregate view.

## Tradeoffs of the subgroup breakdown <!-- role: costs -->

**Sacrifice:** You use more space than a single aggregate scatterplot.
**Risk:** Readers may focus on only one level and miss the other.
**Mitigation:** Keep the aggregate view and subgroup views together.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Plot only the combined point cloud when groups are a relevant unit of interpretation. **Why it fails:** The aggregate direction can hide or reverse the direction present inside the groups.

## How to test the refinement <!-- role: check -->

**Failure Sign:** The aggregate correlation is clear, but the within-group direction is unknown.
**Quick Check:** Compare the combined scatterplot with subgroup views; if subgroup slopes differ from the aggregate slope, keep both levels visible.
**Stronger Test:** Inspect the overall correlation and each subgroup correlation side by side before interpreting one pooled trend.

## What to change <!-- role: fix -->

- Split the grouped data into subgroup scatterplots alongside the aggregate scatterplot.
- Distinguish the groups before interpreting a single overall correlation.
- Report the aggregate relationship only after checking whether subgroup trends agree with it.
