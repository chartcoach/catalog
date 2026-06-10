---
id: add-icon-arrays-alongside-risk-ratios-when-group-sizes-differ
title: Add icon arrays alongside numerical risk ratios when group sizes differ
bibliography: references.bib
description: For exact comparison of treatment risk reductions, use paired icon arrays
  on numerical risk summaries with unequal group sizes to improve fidelity and mitigate
  denominator neglect for audiences with low numeracy or limited nonnative language
  proficiency.
labels:
- purpose:refine
- basis:empirical
- task:compare
- structure:multi-view:use
- quality:fidelity
- lever:layout-structure
- operator:part-whole
---

## Paired icon arrays for both groups <!-- role: advice -->

Add one icon array for each compared group alongside the numerical ratios when the group sizes differ. For example, place a separate array next to each group's numbers, size each array to that group's full denominator, and mark the affected cases distinctly within the full set of icons.

## Why paired icon arrays work <!-- role: reason -->

Icon arrays make the total group size visible at the same time as the affected cases. That helps viewers see the numerator as part of a whole instead of treating the numerator as the whole story.

**Mechanism:** A paired icon-array display makes the denominator salient and visually separates the two groups. This reduces overestimation when the treated group is smaller and underestimation when the treated group is larger.

**Evidence:** Across national samples in the United States and Germany and among Polish immigrants in the United Kingdom, adding icon arrays to numerical risk information reduced denominator neglect and improved accuracy, with especially strong benefits for low-numeracy readers and for readers viewing the information in a nonnative language [@garcia-retameroUsingVisualAids2012].

## When to use paired icon arrays <!-- role: context -->

- **User Goal:** Help viewers compare the risk effect of one option against another.
- **Task:** Support accurate reading of relative risk reduction from two compared groups.
- **Data:** The compared groups have different denominators.
- **Chart Setting:** Numerical risk information is already present and can be paired with a second visual display.
- **Audience:** Readers have low numeracy, mixed numerical skill, or limited proficiency in the language used for the text.
- **Success Criterion:** Viewers use the full group sizes in their judgment and give fewer overestimates or underestimates of treatment effect.

## When paired icon arrays are not enough <!-- role: exceptions -->

- **Break it when:** The compared ratios already share the same denominator. **Why:** The main denominator-neglect problem is already reduced, so the added arrays solve a smaller problem.
- **Break it when:** The audience has low graph literacy and you cannot provide additional support. **Why:** Icon arrays help less when viewers struggle to interpret graphical displays.

## Tradeoffs of paired icon arrays <!-- role: costs -->

**Sacrifice:** You use more space than a numbers-only summary.
**Risk:** Viewers with low graph literacy may not benefit as much as other readers.
**Mitigation:** Keep the numerical ratios visible next to the icon arrays, and use common denominators when you can.

## Common icon-array failure mode <!-- role: mistakes -->

**Mistake:** Add icon arrays but make the two arrays ignore the true group sizes. **Why it fails:** If the arrays do not preserve each denominator, the display no longer exposes the part-to-whole comparison that reduces denominator neglect.

## How to check paired icon arrays <!-- role: check -->

**Failure Sign:** Reviewers still answer from the raw event counts, or the two arrays do not reflect the actual group totals.
**Quick Check:** Verify that each group has its own array and that the total number of icons in each array matches that group's denominator.
**Stronger Test:** Compare a numbers-only version against the numbers-plus-icon-arrays version with a reviewer; the paired version should produce fewer overestimates and underestimates of risk reduction.

## How to fix missing denominator cues <!-- role: fix -->

- Add a separate icon array for each compared group.
- Set the total icon count in each array to that group's denominator.
- Highlight the affected cases within each full array.
- Keep the numerical ratios next to the icon arrays instead of removing them.
