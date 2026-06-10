---
id: report-compared-risks-on-a-shared-denominator
title: Report compared risks on a shared denominator
bibliography: references.bib
description: For exact comparison of risk reduction in grouped-result quantitative
  summaries, prefer matched denominators on numeric two-group comparisons to improve
  fidelity and mitigate denominator neglect for readers interpreting treatment effectiveness.
labels:
- purpose:refine
- basis:empirical
- task:compare
- scope:grouped-result
- quality:fidelity
- lever:encoding
- operator:part-whole
- reading-mode:exact
---

## Shared denominators <!-- role: advice -->

Report both groups on the same denominator when presenting numeric risk reduction. For example, restate treated and untreated outcomes as rates out of a shared base such as 100 or 1000 instead of comparing values like 2/100 against 50/500 or 30/500 against 10/100.

## Equal denominators prevent numerator-driven misreading <!-- role: reason -->

Using the same denominator removes the need to mentally reconcile different group sizes. Readers can compare like with like instead of judging the effect from raw event counts alone.

**Mechanism:** A shared denominator makes the part-to-whole relation directly comparable across groups, so the numerator is read in relation to the same total in both groups.

**Evidence:** In both studies, numeric-only judgments of treatment risk reduction were fairly accurate when treated and untreated groups used equal denominators, but accuracy dropped when denominators differed and participants relied too much on numerators [@garcia-retameroIconArraysHelp2010].

## Use when group risks are presented numerically <!-- role: context -->

- **User Goal:** Judge how much a treatment changes risk.
- **Task:** Compare two group risks and infer relative risk reduction.
- **Data:** Two event counts out of two group totals, where the original group sizes may differ.
- **Chart Setting:** Numeric-only risk communication in which the comparison is carried by the reported ratios.
- **Audience:** Younger or older adults interpreting health-risk information.
- **Success Criterion:** Readers can estimate the treatment effect accurately without over- or under-weighting raw event counts.

## Do not use when a shared base cannot be the main comparison <!-- role: exceptions -->

**Break it when:** The main display must preserve the original unequal group sizes and cannot restate both risks on a common base. **Why:** The paper treats matched denominators as the preferred convention, but recommends visual displays when that convention is not feasible.

## Tradeoffs of matched denominators <!-- role: costs -->

**Sacrifice:** The main ratio statement no longer shows the original sample-size imbalance directly.
**Risk:** Readers may miss that one group was actually much larger or smaller in the underlying study or recall set.
**Mitigation:** If the unequal group sizes must remain visible, keep them visible with a visual display such as icon arrays instead of relying on numeric ratios alone.

## Common failure with denominator formatting <!-- role: mistakes -->

**Mistake:** Keep unequal denominators in a numeric-only comparison and assume readers will mentally normalize them. **Why it fails:** Many readers judge the comparison from the absolute event counts and misread how large the effect really is.

## How to review denominator formatting <!-- role: check -->

**Failure Sign:** The two compared risks are written with different totals.
**Quick Check:** Rewrite both ratios to the same base and see whether the perceived strength of the effect changes.
**Stronger Test:** If the comparison becomes directly readable only after normalization, the original formatting is inviting denominator neglect.

## How to repair denominator formatting <!-- role: fix -->

- Rewrite each compared risk to the same denominator.
- Use the normalized values as the main comparison when you report risk reduction.
- If you cannot normalize the main comparison, add icon arrays rather than leaving the comparison numeric-only.
