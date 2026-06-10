---
id: use-classed-color-scales-for-ordinal-data
title: Use a classed color scale for ordinal data
bibliography: references.bib
description: For displays of ordinal values, use a classed color scale on charts or
  maps that encode value with color to improve fidelity and mitigate false intermediate
  states for readers interpreting ordered categories.
labels:
- purpose:refine
- basis:heuristic
- data:ordinal
- quality:fidelity
- lever:encoding
---

## Class the color steps <!-- role: advice -->

Use a classed color scale when the data has fixed ordered categories rather than continuous values. For example, give each Likert level, clothing size, or official rank its own color step instead of blending them across a continuous gradient.

## Prevent false in-between values <!-- role: reason -->

A continuous gradient implies that values can vary smoothly between adjacent colors. That implication is wrong when the data only contains named ordered levels.

**Mechanism:** Classed colors keep each valid level discrete, so readers do not infer nonexistent states between categories.

**Evidence:** The article explicitly says to use classed color scales when the data is classed and warns that an unclassed scale suggests options in between that do not exist [@muth_classed_vs_unclassed_2021].

## Use when the levels are fixed <!-- role: context -->

- **User Goal:** Show ordered categories with color without implying extra levels.
- **Data:** Ordinal values with fixed steps and no valid values between them.
- **Chart Setting:** A chart or map that uses a color scale to encode those ordered values.
- **Success Criterion:** Readers can identify the valid categories without inferring intermediate states.

## Do not use when the values vary continuously <!-- role: exceptions -->

**Break it when:** The values are continuous and the chart needs to show smooth variation between nearby values. **Why:** Classing removes nuance that an unclassed scale can preserve.

## Accept the loss of within-step detail <!-- role: costs -->

**Sacrifice:** You give up variation inside each category.
**Risk:** Adding extra steps beyond the real categories reintroduces artificial detail.
**Mitigation:** Match the number of color steps to the actual ordered levels in the data.

## Avoid continuous gradients on named levels <!-- role: mistakes -->

**Mistake:** Applying an unclassed gradient to fixed ordered categories. **Why it fails:** It makes readers think that values between adjacent categories are valid.

## Test whether the legend implies extra states <!-- role: check -->

**Failure Sign:** The legend fades smoothly even though the data only has fixed named levels.
**Quick Check:** Ask whether a color halfway between two legend labels would look like a valid data state.
**Stronger Test:** Verify that each unique data level maps to one distinct legend step.

## Replace the gradient with steps <!-- role: fix -->

- Replace the continuous gradient with a stepped color scale.
- Assign one color step to each valid ordered category.
- Remove interpolated legend stops between adjacent categories.
