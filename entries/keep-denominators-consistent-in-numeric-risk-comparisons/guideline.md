---
id: keep-denominators-consistent-in-numeric-risk-comparisons
title: Keep denominators consistent in numerical risk comparisons
bibliography: references.bib
description: For compare tasks on grouped-result numerical risk displays, use consistent
  denominators across groups to improve fidelity and mitigate denominator neglect
  for audiences with low numeracy.
labels:
- purpose:refine
- basis:empirical
- task:compare
- scope:grouped-result
- quality:fidelity
- lever:text-annotation
- chart:text:use
- knowledge:low
---

## Consistent denominators <!-- role: advice -->

Use the same denominator for each group when presenting a numerical risk comparison. For example, rewrite treated-versus-untreated outcomes so both groups are shown as x out of 100 or x out of 800, rather than mixing one numerator over 100 with another over 800.

## Why consistent denominators work here <!-- role: reason -->

Matched denominators make the two groups directly comparable in a numbers-only display. Readers do not have to normalize mentally before comparing the event counts, so they are less likely to rely on raw numerators.

**Mechanism:** Keeping the same denominator across groups reduces the chance that readers will compare absolute event counts as if they were proportions.

**Evidence:** When the study presented equally effective treatments with different denominators in the treated and untreated groups, many participants misestimated risk reduction; errors were much lower when the denominators were equal. This pattern was strongest among low-numeracy participants, showing that consistent denominators improve numerical comparisons [@garcia-retameroCommunicatingTreatmentRisk2009].

## Where to use consistent denominators <!-- role: context -->

- **User Goal:** Understand how much one option changes risk relative to another.
- **Task:** Compare two group risks from numbers alone.
- **Data:** Two-group outcome counts that can be expressed on a common base.
- **Chart Setting:** Text-heavy or numbers-only risk communication without paired icon arrays.
- **Audience:** Mixed public audiences, especially readers with low numeracy.
- **Success Criterion:** Readers estimate the same treatment effect regardless of which raw group size was larger.

## When to use a different fix <!-- role: exceptions -->

**Break it when:** You can add icon arrays that show the full denominator for each group. **Why:** The source found that icon arrays eliminated the denominator-size effect even when the group totals remained unequal.

## Costs of consistent denominators <!-- role: costs -->

**Sacrifice:** You may need to restate the comparison on a common base instead of presenting only the original raw counts.\
**Risk:** Leaving mixed raw denominators prominent beside the common-base rewrite can keep attention on the raw numerators.\
**Mitigation:** If the original unequal totals must remain visible, pair the standardized numbers with icon arrays.

## Common failure with consistent denominators <!-- role: mistakes -->

**Mistake:** Mix denominators across groups in a numbers-only comparison. **Why it fails:** Readers compare raw event counts instead of proportions and overestimate or underestimate the treatment effect.

## How to test denominator consistency <!-- role: check -->

**Failure Sign:** Reader judgments change when only the group denominators change, even though the true relative risk reduction stays the same.\
**Quick Check:** Rewrite the same comparison once with matched denominators and once with unmatched denominators; if answers differ, standardize the denominators.\
**Stronger Test:** Ask readers to estimate deaths per 1000 after reading the comparison; if the implied relative risk reduction is too high when the treated group is smaller or too low when it is larger, change the denominators.

## How to fix the display <!-- role: fix -->

- Convert each group's outcome to the same denominator before presenting the comparison.
- Replace mixed forms such as x out of N versus y out of M with matched forms such as x out of 100 versus y out of 100.
- Keep the comparison on that common base wherever readers are expected to judge treatment effect from the numbers.
- If unequal raw totals must remain visible, add paired icon arrays that show each full denominator.
