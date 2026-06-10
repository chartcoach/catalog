---
id: limit-mentally-rotated-feature-bindings-to-one-focal-part
title: Limit mentally rotated feature bindings to one focal part
bibliography: references.bib
description: For mental-rotation tasks on multi-part object diagrams, use a single
  focal feature binding on the rotated object to improve fidelity and mitigate loss
  of part identities for readers interpreting rotated structures.
labels:
- purpose:refine
- basis:empirical
- quality:fidelity
- lever:encoding
- reading-mode:exact
- polish:focus
---

## Single focal binding <!-- role: advice -->

Reduce the rotation step to one feature-part binding that readers must actively preserve. For example, keep one diagnostic part visually distinct during the imagined rotation and do not expect several colored parts to stay attached to several moving parts at once.

## Why one binding survives rotation <!-- role: reason -->

The rotation bottleneck in this study was not general memory load alone. It was the need to keep arbitrary features attached to moving parts while attention tracked the transformation, and that process supported only one binding.

**Mechanism:** During mental rotation, attention tracks a single part and preserves the feature attached to that part. Additional feature-part bindings are likely to detach because the visual system is not well suited to keeping several arbitrary features glued to several moving parts simultaneously.

**Evidence:** When the object stayed static, readers kept about two feature-part links, but during mental rotation capacity fell to about one; the same limit appeared when attention rotated a separate attached needle, and it did not appear for a scaling task [@xuCapacityVisualFeatures2015].

**Notes:** The paper argues that additional feature information may need to be filled in only after rotation is paused.

## Use when exact part identity matters during rotation <!-- role: context -->

- **User Goal:** Verify that the same part keeps the same identity after a rotation.
- **Data:** A multi-part object with several arbitrary features bound to different parts.
- **Chart Setting:** A diagram or instructional display that requires readers to imagine the rotation rather than inspect a completed rotated state.
- **Audience:** Readers doing exact spatial matching, not just gist-level shape recognition.
- **Success Criterion:** Readers preserve the identity of the critical part through the rotation step.

## Do not use for static or scaling tasks <!-- role: exceptions -->

**Break it when:** Readers do not have to imagine rotation, or the required change is expansion or contraction rather than rotation. **Why:** The paper found substantially better retention of feature-part bindings when the object was static or only scaled.

## Tradeoffs of one focal binding <!-- role: costs -->

**Sacrifice:** You stop showing several equally important bindings as simultaneously actionable during the rotation step.
**Risk:** Important non-focal identities may be deferred.
**Mitigation:** Reintroduce the remaining identities after the rotation step rather than during it.

## Too many simultaneous bindings <!-- role: mistakes -->

**Mistake:** Keeping every part equally distinct and asking readers to preserve all of those identities through a mental rotation. **Why it fails:** The measured capacity for this specific operation was about one binding, so non-focal parts are likely to be lost or swapped.

## Review the binding load <!-- role: check -->

**Failure Sign:** Readers reliably preserve one part identity but confuse the others after rotation.
**Quick Check:** Ask a reviewer which specific part identity they can track through the rotation without guessing.
**Stronger Test:** Compare accuracy for the focal part against accuracy for the non-focal parts.

## Edits that reduce binding load <!-- role: fix -->

- Keep one critical part visually distinct during the rotation step.
- De-emphasize noncritical parts while the reader is performing the rotation.
- Pause the rotation step before reintroducing additional part identities.
