---
id: encode-primary-quantity-with-position-for-value-tasks
title: Encode the primary quantitative field with position for exact value tasks
bibliography: references.bib
description: For exact individual-value tasks, use position encoding for the primary
  quantitative field on multivariate point plots to improve fidelity and mitigate
  misreads from less precise size or color encodings for readers performing lookup
  and pairwise comparison.
labels:
- purpose:refine
- basis:empirical
- lever:encoding
- channel:position:use
- operator:lookup
- reading-mode:exact
- measure:multi
- quality:fidelity
---

## Position the primary quantitative field <!-- role: advice -->

Put the quantitative field people must read or compare exactly on x or y. For example, in a trivariate point plot, map the primary quantity to a positional axis and leave size or color for a secondary quantity or a category instead of putting the primary quantity on size or color.

## Why positional encoding works here <!-- role: reason -->

Exact reading tasks depend on a fast, stable visual lookup. Position made the primary value easier to decode than retinal channels when participants had to read a marked point or compare two marked points.

**Mechanism:** Position supports more precise value lookup and pairwise comparison than size or color when readers must inspect individual records.

**Evidence:** Across value tasks, encodings that placed the primary quantitative field on x or y ranked higher overall than encodings that placed it on size or color [@kimAssessingEffectsTask2018].

## Use when exact value reading is the job <!-- role: context -->

- **User Goal:** Read a value from a marked point or decide which of two points is larger or smaller.
- **Task:** Exact lookup or exact pairwise comparison of individual records.
- **Data:** A point-based view with one primary quantitative field and at least one additional field competing for encoding channels.
- **Chart Setting:** A multivariate point plot where x and y are available for assignment.
- **Success Criterion:** Lower error and faster completion on individual-value questions.

## Do not use when the task is group summary <!-- role: exceptions -->

**Break it when:** The task is to compare group averages or identify which category contains the maximum. **Why:** In the study, size encoding of the primary quantity performed well for these summary tasks, so the value-task advantage of position does not transfer cleanly.

## What this costs <!-- role: costs -->

**Sacrifice:** You give positional priority to one quantity rather than another field.
**Risk:** A less important field may be pushed to a weaker or more interfering channel.
**Mitigation:** Keep the primary task field on position and move the less critical field to a non-positional channel.

## Common failure around this move <!-- role: mistakes -->

**Mistake:** Put the primary quantitative field on size or color because another field already occupies position. **Why it fails:** The chart becomes worse for exact value reading and comparison, which were the tasks where position was most effective.

## How to test the choice <!-- role: check -->

**Failure Sign:** Readers hesitate or make mistakes on marked-point value questions.
**Quick Check:** Compare the current chart against a version where the primary quantitative field is moved to x or y.
**Stronger Test:** Ask one read-value question and one compare-values question on both versions and keep the lower-error, faster version.

## What to change <!-- role: fix -->

- Move the primary quantitative field to x or y.
- Reassign the displaced field to color, size, or faceting.
- If both positional axes are occupied, rebuild the point plot so the task-critical quantity gets a positional axis.
