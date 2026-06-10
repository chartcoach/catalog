---
id: use-color-not-size-for-secondary-quantity-in-value-tasks
title: Use color instead of size for a secondary quantitative field when position
  carries the primary value
bibliography: references.bib
description: For exact individual-value tasks, use color encoding for the secondary
  quantitative field on multivariate point plots to improve fidelity and mitigate
  size-based interference with a primary positional value for readers reading or comparing
  single points.
labels:
- purpose:refine
- basis:empirical
- lever:encoding
- channel:color-hue:use
- channel:area:avoid
- operator:lookup
- reading-mode:exact
- quality:fidelity
---

## Reassign the secondary quantity from size to color <!-- role: advice -->

Use color rather than size for the secondary quantitative field when the primary quantitative field is already on x or y and users must read individual values exactly. For example, in a dot plot or scatterplot with a positional primary value, keep the secondary value in color instead of varying point size.

## Why color is the safer distractor here <!-- role: reason -->

A secondary size encoding changes mark area and competes with positional reading of the primary value. Color still adds another field, but it disrupted exact value tasks less than size in the tested multivariate point plots.

**Mechanism:** Varying point size acts as a stronger distractor than color when readers are trying to decode a primary quantitative field from position.

**Evidence:** For value tasks, charts with the secondary quantitative field encoded by size took longer than matched charts that encoded that same secondary field with color while the primary field stayed on x or y [@kimAssessingEffectsTask2018].

## Use when one quantity is primary and exact reading matters <!-- role: context -->

- **User Goal:** Read or compare the primary quantitative value at the point level.
- **Task:** Exact lookup or exact pairwise comparison.
- **Data:** Two quantitative fields shown together in the same point-based chart.
- **Chart Setting:** The primary quantitative field is already encoded on x or y, and a secondary quantitative field still needs encoding.
- **Success Criterion:** Preserve speed and accuracy for the primary value.

## Do not use when the study's value-task condition does not hold <!-- role: exceptions -->

**Break it when:** The task is not exact individual-value reading or comparison. **Why:** The measured slowdown from size interference was reported for value tasks, not as a general rule for all tasks.

## What this costs <!-- role: costs -->

**Sacrifice:** The secondary quantitative field may become less directly readable than it would be with size.
**Risk:** If the secondary field also needs precise quantitative decoding, color may underserve that second task.
**Mitigation:** Prioritize the field that the user must read exactly, and protect its positional decoding first.

## Common failure around this move <!-- role: mistakes -->

**Mistake:** Add a size encoding for a secondary quantity on top of a positional primary quantity in a value task. **Why it fails:** The size variation slows down decoding of the primary positional value.

## How to test the choice <!-- role: check -->

**Failure Sign:** Primary-value lookups get slower once point sizes start varying.
**Quick Check:** Compare the chart against a version that keeps the same primary positional encoding but moves the secondary quantity from size to color.
**Stronger Test:** Run one marked-point read task or compare-values task on both versions and keep the faster one if error stays comparable.

## What to change <!-- role: fix -->

- Move the secondary quantitative field from size to color.
- Keep the primary quantitative field on x or y.
- If both quantitative fields need strong value reading, give them positional encodings rather than adding a size encoding.
