---
id: avoid-hue-only-encoding-for-ordered-values
title: Avoid hue-only encoding for ordered values
bibliography: references.bib
description: For ordinal or quantitative reading, avoid hue-only encoding on charts
  with ordered values to improve fidelity and mitigate unordered magnitude readings
  for readers.
labels:
- purpose:refine
- basis:empirical
- data:ordinal
- data:quantitative
- quality:fidelity:use
- lever:encoding
- channel:color-hue:avoid
---

## Hue-only encoding removal <!-- role: advice -->

Do not use hue as the only carrier of order or magnitude. For example, do not map ranked levels or numeric values only to hue steps when readers must tell which values are higher or lower.

## Why hue fails for ordered reading <!-- role: reason -->

Hue variation creates distinction, but not a reliable higher-lower sequence. When readers must infer order or magnitude, hue alone does not give them the perceptual structure they need.

**Mechanism:** Viewers do not perceive a natural ordering in changes of hue, so hue-only scales make ordered values look merely different instead of larger or smaller.

**Evidence:** The paper states that hue alone cannot express ordinal or quantitative information because viewers do not assign an inherent order to hue variation [@bertiniWhyShouldntAll2020].

## Use when readers must infer order <!-- role: context -->

- **User Goal:** Let readers judge order, rank, or magnitude.
- **Task:** Ordinal or quantitative reading.
- **Data:** Ordered categories or numeric values.
- **Chart Setting:** Color is being considered as the main encoding for the values.
- **Audience:** Readers who need to tell which values are higher or lower.
- **Success Criterion:** Readers can infer order directly from the display.

## Do not use this rule for purely categorical color <!-- role: exceptions -->

**Break it when:** Color is only distinguishing categories and no order must be inferred. **Why:** The problem is specific to hue as an ordered scale, not hue as a categorical separator.

## Costs of removing hue-only order <!-- role: costs -->

**Sacrifice:** You give up a purely hue-driven look for the ordered field.
**Risk:** If you ignore the rule, viewers may see differences in color without seeing a reliable value order.
**Mitigation:** Move the ordered field to a channel that visibly preserves order.

## Common hue-scale mistake <!-- role: mistakes -->

**Mistake:** Using hue steps as if they formed an obvious higher-lower sequence. **Why it fails:** The colors look different, but the order among them is not perceptually stable.

## Check whether hue is carrying too much <!-- role: check -->

**Failure Sign:** Reviewers cannot tell which hue-coded item is larger without relying on labels or legend reading.
**Quick Check:** Hide the legend and ask a reviewer to rank a few hue-coded marks.
**Stronger Test:** If the ordering disappears once the legend is removed, hue is doing a job it cannot do by itself.

## Fix the ordered encoding <!-- role: fix -->

- Remove hue as the sole encoding for the ordered field.
- Re-encode the ordered field with a channel that preserves perceptual order.
- Keep hue for distinction or semantic association rather than as the only magnitude cue.
