---
id: avoid-lightness-differences-for-numerosity-comparisons
title: Avoid lightness differences when viewers compare numerosity
bibliography: references.bib
description: For overview quantity comparisons, avoid lightness encoding on grouped
  marks to prevent biased numerosity judgments and mitigate false differences when
  viewers compare how many items belong to each group.
labels:
- purpose:refine
- basis:empirical
- task:compare
- quality:fidelity:use
- lever:encoding
- channel:color-lightness:avoid
- reading-mode:overview
---

## Remove lightness as the group cue for counts <!-- role: advice -->

Do not use lightness differences to distinguish groups when readers must judge how many items each group contains. For example, avoid making one class darker than another in a dot display when the quantity comparison itself is important.

## Why lightness biases quantity reading <!-- role: reason -->

Darker collections can look more numerous even when the count is unchanged. That means the lightness cue can distort the very quantity comparison the display is supposed to support.

**Mechanism:** Lightness changes perceived numerosity, so viewers may infer a larger count from a darker group rather than from the actual number of marks.

**Evidence:** The review collates this paper as covering summary tasks such as aggregation and quantity-related judgments. In its numerosity discussion, the paper states that darker collections can appear more numerous and warns designers to be careful when luminance differentiates collections whose relative numerosity matters [@zengReviewCollationGraphical2023; @szafirFourTypesEnsemble2016].

## Use when group size is the message <!-- role: context -->

- **User Goal:** Compare how many items belong to each group.
- **Task:** Relative numerosity judgment across groups.
- **Chart Setting:** Mark-based displays where groups could be distinguished by lightness.
- **Success Criterion:** Quantity comparisons that reflect actual counts rather than apparent darkness.

## Do not apply this when quantity is not being compared <!-- role: exceptions -->

**Break it when:** Relative numerosity is not a relevant judgment in the display. **Why:** The warning is tied specifically to cases where viewers compare how many items belong to each collection.

## Tradeoffs of removing lightness as a class cue <!-- role: costs -->

**Sacrifice:** You give up using lightness as the primary distinction between count-comparison groups.
**Risk:** If you keep lightness differences, the darker group can seem larger than it is.
**Mitigation:** Equalize lightness across the groups whose counts are being compared.

## Common failure with count comparisons <!-- role: mistakes -->

**Mistake:** Making one group darker and expecting unbiased quantity comparison. **Why it fails:** The lightness difference itself shifts perceived numerosity.

## Check whether darkness is changing the apparent count <!-- role: check -->

**Failure Sign:** An equal-count darker group looks more numerous at a glance.
**Quick Check:** Swap or equalize group lightness while keeping counts fixed and see whether the apparent winner changes.
**Stronger Test:** Build an equal-count mockup and ask reviewers which group seems more numerous before and after removing the lightness difference.

## Fix the lightness bias <!-- role: fix -->

- Equalize lightness across the groups whose quantities are being compared.
- Reserve lightness for attributes that are not part of the numerosity judgment.
