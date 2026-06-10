---
id: reduce-distinct-categories-for-simultaneous-numerosity-estimates
title: Reduce the number of distinct categories for simultaneous numerosity estimates
bibliography: references.bib
description: For simultaneous numerosity comparison across categories, prefer fewer
  visually distinct groups in one display to improve fidelity and mitigate overload
  from multiple concurrent count estimates for overview readers.
labels:
- purpose:refine
- basis:empirical
- task:compare
- quality:fidelity
- lever:encoding
- group-cardinality:many
- reading-mode:overview
---

## Category count load <!-- role: advice -->

Reduce the number of visually distinct categories when viewers must estimate several counts at once. For example, merge minor classes before asking readers to compare many colored or oriented sets in the same view.

## Why fewer simultaneous count targets help <!-- role: reason -->

Simultaneous numerosity estimation does not scale cleanly to many distinct groups.

**Mechanism:** Each extra visually distinct category adds another quantity that must be estimated and held for comparison, which pushes against the limit on simultaneous numerosity estimates.

**Evidence:** The paper notes that the number of possible simultaneous numerosity estimates may be limited and draws the visualization implication that the number of visually distinct categories should be limited when simultaneous numerosity estimation is critical [@szafirFourTypesEnsemble2016].

## Use when several group counts must be read together <!-- role: context -->

- **User Goal:** Compare multiple group counts in one glance.
- **Task:** Estimate several numerosities simultaneously.
- **Chart Setting:** One display contains many visually distinct categories.
- **Audience:** Readers are making overview comparisons rather than exact counts.
- **Success Criterion:** Readers can compare the intended group quantities without losing track of categories.

## Do not use when categories are read one at a time <!-- role: exceptions -->

**Break it when:** The display only asks readers to estimate one category at a time. **Why:** The reported limit concerns simultaneous numerosity estimates across multiple groups.

## Tradeoffs of reducing category count <!-- role: costs -->

**Sacrifice:** Some simultaneous category detail is collapsed.\
**Risk:** Too many distinct groups overload the count-comparison task.\
**Mitigation:** Keep only the categories whose counts must be compared at the same time.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Leaving every category visually distinct in a view that asks for many simultaneous count comparisons. **Why it fails:** The number of concurrent numerosity estimates is limited.

## Check simultaneous count load <!-- role: check -->

**Failure Sign:** Reviewers can compare one or two group counts but lose track when all categories are shown together.\
**Quick Check:** Ask readers to compare all visible category counts at once; if they cannot do it reliably, reduce the number of distinct groups.\
**Stronger Test:** Compare count-comparison error before and after merging categories.

## Fix the encoding <!-- role: fix -->

- Combine minor categories into fewer visually distinct groups.
- Remove distinct styling from categories whose counts are not part of the main comparison.
- Keep only the categories needed for the simultaneous count judgment in the primary view.
