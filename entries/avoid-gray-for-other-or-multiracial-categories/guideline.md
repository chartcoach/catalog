---
id: avoid-gray-for-other-or-multiracial-categories
title: Avoid gray for 'other' or multiracial categories
bibliography: references.bib
description: For non-temporal comparison of racial or ethnic groups, avoid gray category
  colors on 'other' or multiracial series in categorical charts to prevent diminished
  visual importance and mitigate signals that some groups matter less for readers
  represented in the data.
labels:
- purpose:refine
- basis:heuristic
- data:categorical
- quality:trust
- lever:encoding
- polish:palette
- aesthetic:color:avoid
---

## Equal-weight category colors <!-- role: advice -->

Assign a full category color to “other” and multiracial groups instead of graying them out. For example, give an “other,” “multiracial,” or “two or more races” series the same saturation and visual weight as the rest of the palette.

## Why gray can diminish people categories <!-- role: reason -->

Gray often reads as secondary or unimportant. When that treatment is applied to people categories, it can suggest that the people in that group matter less than the others in the chart.

**Mechanism:** A gray category weakens visual emphasis and can turn a label like “other” or “multiracial” into a diminished status rather than an equal part of the data.

**Evidence:** The source warns that using gray for “other” or “multiracial” categories can be inappropriate because gray can communicate that the people in that category are not as important as the others, and it shows examples where these categories receive equal visual importance instead [@muth_race_ethnicity_colors_2024].

## When to avoid gray categories <!-- role: context -->

- **User Goal:** Show all people categories respectfully.
- **Task:** Compare or explain racial or ethnic group values.
- **Data:** Categorical groups that include an “other” or multiracial category.
- **Chart Setting:** A chart with one palette color per category.
- **Audience:** Mixed readers, including people represented by the data.
- **Success Criterion:** “Other” and multiracial groups read as equally legitimate categories rather than as de-emphasized leftovers.

## When gray can still appear <!-- role: exceptions -->

**Break it when:** gray is not labeling “other” or multiracial people but only serving as a background category outside the chart’s focus. **Why:** the source allows white, gray, or black as a backdrop when a background category is least important and the focal groups carry the main color emphasis.

## Costs of removing gray <!-- role: costs -->

**Sacrifice:** You lose a common neutral de-emphasis device.
**Risk:** If every category is equally vivid, the main story focus can weaken.
**Mitigation:** Put emphasis on focal groups with stronger color on those groups rather than by graying out “other” or multiracial people.

## Common gray-category mistake <!-- role: mistakes -->

**Mistake:** Using gray as the automatic color for “other” or “multiracial.” **Why it fails:** The color treatment implies that those people are less important than the rest of the categories.

## How to check gray treatment <!-- role: check -->

**Failure Sign:** “Other” or multiracial appears in gray while peer categories use full colors.
**Quick Check:** Inspect the legend for gray assigned to “other,” “multiracial,” or similar labels.
**Stronger Test:** Verify that every people category, except a deliberate background group, has comparable visual importance.

## How to fix gray treatment <!-- role: fix -->

- Replace gray on “other” or multiracial categories with a full category color from the main palette.
- Match that category’s saturation and visual weight to the others.
- If you need a subdued background group, apply that treatment only to a clearly least-important backdrop category, not to “other” or multiracial people.
