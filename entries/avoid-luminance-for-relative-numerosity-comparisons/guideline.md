---
id: avoid-luminance-for-relative-numerosity-comparisons
title: Avoid luminance encoding for group comparisons of numerosity
bibliography: references.bib
description: For relative numerosity comparison, avoid luminance encoding for group
  identity on point-based displays to prevent count bias and mitigate darker-looks-more
  errors for overview readers.
labels:
- purpose:refine
- basis:empirical
- task:compare
- quality:fidelity
- lever:encoding
- channel:color-lightness:avoid
- reading-mode:overview
---

## Group coding for count comparison <!-- role: advice -->

Do not separate compared groups mainly by dark-versus-light coding when readers must judge which group is more numerous. For example, use hue or orientation rather than a darker and lighter set of marks when the display asks readers to compare counts.

## Why luminance biases count judgments <!-- role: reason -->

Readers do not see numerosity independently of all other mark properties.

**Mechanism:** Darker groups can appear more numerous than lighter groups, which biases relative count judgments even when the true counts are the same.

**Evidence:** The paper states that darker collections can appear more numerous and warns designers to be careful using luminance when relative numerosity matters; it also notes that relative numerosity is robust across color and orientation in visualization studies [@szafirFourTypesEnsemble2016].

## Use when relative counts matter <!-- role: context -->

- **User Goal:** Compare how many items belong to each group.
- **Task:** Make a relative numerosity judgment.
- **Chart Setting:** Multiple groups of marks are distinguished visually within one display.
- **Audience:** Readers are making quick overview estimates rather than exact counts.
- **Success Criterion:** Equal-count groups do not look different in quantity because of the encoding.

## Do not use when count is not being read from the view <!-- role: exceptions -->

**Break it when:** Relative numerosity is not a relevant reading of the display. **Why:** The reported bias matters specifically for count judgments.

## Tradeoffs of avoiding luminance <!-- role: costs -->

**Sacrifice:** Lightness is no longer available as the main grouping cue for the categories being counted.\
**Risk:** If kept, darker groups can look larger than equal lighter groups.\
**Mitigation:** Move the compared groups to hue or orientation instead.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Using a dark group and a light group to carry categories whose counts will be compared. **Why it fails:** The dark group can inherit a false numerosity advantage.

## Check for luminance-driven count bias <!-- role: check -->

**Failure Sign:** An equal-count darker group looks more numerous than a lighter one.\
**Quick Check:** Make a test display with equal counts in dark and light groups and ask which group seems larger.\
**Stronger Test:** Repeat the same comparison after switching the groups to hue or orientation and compare the error pattern.

## Fix the encoding <!-- role: fix -->

- Replace lightness-based group coding with hue for the categories being counted.
- Replace lightness-based group coding with orientation when that channel is available for the same comparison.
- Remove dark-versus-light grouping from the primary view if numerosity comparison is part of the task.
