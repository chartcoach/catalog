---
id: use-common-denominators-for-compared-risk-ratios
title: Use a common denominator for compared risk ratios
bibliography: references.bib
description: For exact comparison of treatment risk reductions, use a common denominator
  on numerical risk summaries to improve fidelity and mitigate denominator neglect
  for audiences with low numeracy.
labels:
- purpose:refine
- basis:empirical
- task:compare
- quality:fidelity
- lever:text-annotation
- operator:part-whole
- knowledge:low
---

## Common denominators for compared ratios <!-- role: advice -->

Rewrite compared risk ratios to the same denominator before asking viewers to judge treatment effect. For example, restate both groups as rates per 100 or per 1,000 instead of comparing one ratio like 5/100 against another like 80/800.

## Why common denominators work <!-- role: reason -->

Unequal denominators let viewers compare the raw event counts and miss the part-to-whole relation. A shared denominator removes that shortcut and makes the comparison depend on the actual rates rather than on the numerators alone.

**Mechanism:** A common denominator turns the task into a direct rate comparison. That prevents viewers from overestimating or underestimating risk reduction just because one group started with more people.

**Evidence:** In the reviewed studies, unequal denominators produced strong denominator neglect, especially among low-numeracy participants, while equal denominators substantially improved accuracy; the review concludes that reporting risks with the same denominator supports informed medical decisions [@garcia-retameroUsingVisualAids2012].

## When to use common denominators <!-- role: context -->

- **User Goal:** Help viewers judge how much one option changes risk relative to another.
- **Task:** Make an accurate comparison between two risk ratios.
- **Data:** Two groups are being compared and their original sample sizes differ.
- **Chart Setting:** The result is shown as numerical risk information without a visual aid.
- **Audience:** Readers have mixed numerical skill, especially low numeracy.
- **Success Criterion:** Viewers estimate the relative risk reduction accurately instead of reacting to the larger numerator.

## When not to rely on this alone <!-- role: exceptions -->

**Break it when:** The original unequal group sizes must remain visible and cannot be replaced by a common-base restatement. **Why:** The shared-denominator rewrite removes the display of the original group totals, so it cannot carry both messages by itself.

## Tradeoffs of common denominators <!-- role: costs -->

**Sacrifice:** You give up a direct display of the original study group sizes.
**Risk:** Readers may no longer see that one group was much larger than the other.
**Mitigation:** If the original group sizes matter, add a visual display that keeps the full denominators visible rather than leaving the unequal ratios alone.

## Common denominator failure mode <!-- role: mistakes -->

**Mistake:** Leave compared ratios on different denominators and expect readers to normalize them mentally. **Why it fails:** Many viewers compare the event counts in the numerators and misjudge the treatment effect.

## How to check denominator consistency <!-- role: check -->

**Failure Sign:** A smaller numerator is being read as a larger benefit even though the compared groups have different totals.
**Quick Check:** Scan the two ratios and confirm that both use the same base such as per 100 or per 1,000.
**Stronger Test:** Rewrite the current ratios to a common denominator and compare the two versions with a reviewer; if the rewritten version yields a more stable estimate of risk reduction, the original display invited denominator neglect.

## How to fix unequal denominators <!-- role: fix -->

- Recalculate each compared risk to the same denominator.
- Present the two rates with the same base in the final numerical summary.
- If you must keep the original unequal group sizes visible, add a visual display that shows each full denominator.
