---
id: avoid-color-saturation-as-the-uncertainty-scale-on-point-symbols
title: Avoid color saturation as the uncertainty scale on point symbols
bibliography: references.bib
description: For ordinal uncertainty reading on discrete point-symbol displays, avoid
  color saturation as the uncertainty encoding to prevent illogical symbol ordering
  and address misread certain-to-uncertain scales in simple non-interactive displays.
labels:
- purpose:refine
- basis:empirical
- data:ordinal
- operator:uncertainty
- lever:encoding
- channel:color-saturation:avoid
- quality:readability
---

## Replace saturation as the uncertainty channel <!-- role: advice -->

Do not rely on a saturation ramp as the main ordered uncertainty scale for point symbols. For example, replace a more saturated-to-less saturated certainty ramp with a fuzziness, value, or other tested ordered cue rather than expecting saturation alone to read as more or less certain.

## Why saturation is a weak uncertainty cue <!-- role: reason -->

Saturation did not read to participants as a clear ordinal uncertainty progression. Readers did not treat it as a logical certain-to-uncertain scale even though prior literature had suggested it might work.

**Mechanism:** When the visual channel does not imply a natural certainty order, readers must infer the mapping instead of seeing it directly.

**Evidence:** In the general uncertainty series, saturation fell into the unacceptable group for ordinal uncertainty signification, with mean, median, and modal intuitiveness ratings below the midpoint. The paper highlights this as notable because saturation had often been proposed as an intuitive uncertainty cue in earlier work [@maceachrenVisualSemioticsUncertainty2012].

**Notes:** Hue, orientation, and shape also scored poorly as general ordinal uncertainty variables in the same experiment.

## Use when a point symbol needs a general uncertainty scale <!-- role: context -->

- **User Goal:** Encode more-versus-less certainty for individual items.
- **Task:** Read an ordered uncertainty scale directly from the symbol.
- **Data:** Uncertainty is ordinal and attached to discrete records.
- **Chart Setting:** Point-symbol displays in simple, non-interactive information graphics or maps.
- **Audience:** Readers who must infer certainty from the symbol itself.
- **Success Criterion:** The symbol order feels logical without extra explanation.

## Do not use this warning outside the tested encoding setup <!-- role: exceptions -->

**Break it when:** Saturation is not the uncertainty channel or uncertainty is not being shown as an ordinal point-symbol scale. **Why:** The evidence only speaks to saturation as the ordering variable for discrete point-symbol uncertainty.

## Know the tradeoff of replacing saturation <!-- role: costs -->

**Sacrifice:** You give up a familiar color-only treatment.
**Risk:** Swapping to another channel can change the visual style of an existing symbol set.
**Mitigation:** Keep color constant unless color itself is the variable under test.

## Avoid the common saturation failure <!-- role: mistakes -->

**Mistake:** Using more or less saturated versions of the same point symbol as the sole ordered uncertainty scale. **Why it fails:** Participants did not judge saturation as a logical uncertainty progression.

## Check whether saturation is hurting interpretation <!-- role: check -->

**Failure Sign:** Readers cannot confidently tell which saturated symbol is less certain.
**Quick Check:** Compare the saturation version against a fuzziness or value version of the same three-step scale.
**Stronger Test:** Ask reviewers to rate which version is more logical for uncertainty and keep the higher-rated option.

## Fix a saturation-based uncertainty symbol set <!-- role: fix -->

- Replace the saturation ramp with a fuzziness-based uncertainty scale.
- If you must keep color constant, move the uncertainty ordering into value or another stronger tested cue.
- Keep the uncertain-to-certain order explicit while you transition away from saturation.
