---
id: add-icon-arrays-to-unequal-denominator-risk-comparisons
title: Add icon arrays to risk comparisons with unequal denominators
bibliography: references.bib
description: For compare tasks on grouped-result quantitative risk displays, use a
  multi-view layout with icon arrays alongside numeric group counts to improve fidelity
  and mitigate denominator neglect for audiences with low numeracy.
labels:
- purpose:refine
- basis:empirical
- task:compare
- scope:grouped-result
- structure:multi-view:use
- quality:fidelity
- lever:layout-structure
- knowledge:low
---

## Paired icon arrays <!-- role: advice -->

Add one icon array for each comparison group when the groups have different total sizes. For example, place paired arrays next to the numeric frequencies, size each array to its full denominator, and mark the affected cases within each array instead of relying on numbers alone.

## Why paired icon arrays work here <!-- role: reason -->

Paired icon arrays make the whole comparison visible at once. Readers can see both the event counts and the total number of people in each group, which reduces the tendency to compare only the numerators.

**Mechanism:** Showing the full denominator in each group makes unaffected people visible, so readers are less likely to overestimate benefit when the treated group is smaller or underestimate benefit when it is larger.

**Evidence:** In national probability samples from Germany and the United States, numeric-only displays with unequal denominators produced systematic misestimation of treatment risk reduction, especially among low-numeracy participants. Adding icon arrays reduced incorrect estimates and removed the dependence of judgments on whether denominators were equal or unequal [@garcia-retameroCommunicatingTreatmentRisk2009].

**Notes:** The improvement was especially strong for people with low numeracy.

## Where to use paired icon arrays <!-- role: context -->

- **User Goal:** Judge how much one option reduces risk relative to another.
- **Task:** Compare two group outcomes and estimate risk reduction.
- **Data:** Two groups with affected and unaffected counts, with different group totals.
- **Chart Setting:** Numeric risk information is already being shown and there is room to add one icon array per group.
- **Audience:** Mixed public audiences, especially readers with low numeracy.
- **Success Criterion:** Readers give similar risk-reduction judgments even when only the group denominators change.

## When not to rely on this as the main fix <!-- role: exceptions -->

**Break it when:** The numeric comparison already uses the same denominator in both groups. **Why:** The large denominator-neglect errors in the source were driven by unequal denominators.

## Costs of paired icon arrays <!-- role: costs -->

**Sacrifice:** You use more space and add a second representation of the same quantities.\
**Risk:** If the added arrays do not show each group's full denominator, they will not address the numerator-focused reading error.\
**Mitigation:** Size each array to the full group total and show affected cases within that full set.

## Common failure with paired icon arrays <!-- role: mistakes -->

**Mistake:** Keep unequal-denominator comparisons as numbers only, or add a visual that shows only the affected cases. **Why it fails:** Readers keep comparing raw event counts and misread the size of the treatment effect.

## How to test paired icon arrays <!-- role: check -->

**Failure Sign:** Readers think the benefit is larger when the treated group is smaller and smaller when the treated group is larger.\
**Quick Check:** Hold the true risk reduction constant, change only the denominators, and see whether audience judgments change across versions.\
**Stronger Test:** Ask readers to estimate how many out of 1000 would die in each group and compute the implied relative risk reduction; if the estimate shifts with denominator size, add paired icon arrays.

## How to fix the display <!-- role: fix -->

- Add one icon array for each comparison group next to the numeric frequencies.
- Size each icon array to the full denominator for that group.
- Mark the affected cases within each array so both affected and unaffected people remain visible.
- If the numeric statement must stay, keep it and add the paired icon arrays rather than leaving the comparison numbers-only.
