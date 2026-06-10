---
id: separate-stacked-components-onto-a-common-baseline
title: Separate stacked components onto a common baseline
bibliography: references.bib
description: For component comparison across grouped parts, use aligned component
  baselines on bar charts to improve judgment fidelity and mitigate nonaligned-segment
  comparisons for readers making quick visual estimates.
labels:
- purpose:refine
- basis:empirical
- task:compare
- scope:grouped-result
- chart:bar
- quality:fidelity
- lever:layout-structure
- measure:multi
---

## Aligned component baselines <!-- role: advice -->

Separate stacked components onto a common baseline when readers must compare the same part across groups. For example, replace a divided bar with grouped bars so corresponding parts start from the same axis, and add a separate total mark for each group instead of forcing every value into one stack.

## Why aligned component baselines work <!-- role: reason -->

Grouped layouts let readers compare components by position on a common scale. Divided bars leave only a few components aligned; most of the rest must be judged by length or by positions on nonaligned scales.

**Mechanism:** When the same component starts from the same baseline in every group, readers can compare like with like directly. When components stay inside stacks, they have to compare segment lengths or mentally reconstruct distances between segment ends.

**Evidence:** In the paper's position-length experiment, judgment errors rose as compared values lost a common scale and had to be read by length. The redesign examples then replace divided bars with grouped displays so component values can be compared more accurately [@clevelandGraphicalPerceptionTheory1984].

## Use when comparing the same part across groups <!-- role: context -->

- **User Goal:** Compare the same component across several groups.
- **Task:** Judge which group's component is larger and estimate relative size.
- **Data:** Grouped totals split into multiple quantitative components.
- **Chart Setting:** A divided or stacked bar is already under consideration.
- **Audience:** Readers making quick visual judgments rather than exact measurements.
- **Success Criterion:** Lower comparison error for component-to-component judgments.

## Do not use when only totals matter <!-- role: exceptions -->

**Break it when:** The reader only needs the group totals and not the component-to-component comparisons. **Why:** Divided bars already let totals be judged by position along a common scale.

## Tradeoffs of separating the stack <!-- role: costs -->

**Sacrifice:** Totals and components no longer live in one stacked outline.
**Risk:** If you remove the stack and omit a total mark, the whole size for each group becomes harder to see.
**Mitigation:** Add a separate total bar or total dot for each group beside the separated components.

## Common failure with divided bars <!-- role: mistakes -->

**Mistake:** Leave the compared component values inside stacks. **Why it fails:** Most components then have no shared baseline, so readers must compare segment lengths or distances between segment ends.

## Check the component comparison <!-- role: check -->

**Failure Sign:** Reviewers compare segment lengths or gaps between segment tops instead of reading from one common axis.
**Quick Check:** Show the same data in the current divided bar and in a grouped version, then ask which group's matching component is larger.
**Stronger Test:** If the grouped version reduces hesitation or large percent-estimate errors, keep the grouped layout.

## Fix the display <!-- role: fix -->

- Unstack the components that readers must compare across groups.
- Align corresponding components to the same baseline.
- Add a separate total mark for each group rather than leaving the total visible only as stack height.
- If many component values must stay visible, move to a grouped dot display with one total mark and one mark per component.
