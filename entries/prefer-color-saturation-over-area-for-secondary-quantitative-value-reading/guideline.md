---
id: prefer-color-saturation-over-area-for-secondary-quantitative-value-reading
title: Prefer color-saturation over area for a secondary quantitative field during
  exact value reading
bibliography: references.bib
description: For exact value lookup and pairwise comparison, prefer color-saturation
  for a secondary quantitative field on point-based multivariate views to improve
  fidelity and mitigate interference from varying mark area for readers inspecting
  individual values.
labels:
- purpose:refine
- basis:empirical
- quality:fidelity:use
- lever:encoding
- operator:lookup
- reading-mode:exact
- measure:multi
- channel:color-saturation:use
---

## Encode the secondary quantitative field with color-saturation <!-- role: advice -->

Encode the secondary quantitative field with color-saturation when the main quantitative field must be read from position. For example, keep the main quantitative field on x or y and map the other quantitative field to color-saturation instead of varying mark area when readers must read exact values or compare two values.

## Why color-saturation helps here <!-- role: reason -->

Varying mark area acts as a distractor when the reader is trying to decode a different quantitative field from position. Color-saturation preserved better value-reading performance for the positioned field in these exact-reading tasks.

**Mechanism:** Color-saturation leaves the positioned readout visually stable, while changing mark area makes the positioned field harder to decode quickly and accurately.

**Evidence:** In controlled tests of trivariate point-based views, the designs with the main quantitative field on position and the secondary quantitative field on color-saturation outperformed the corresponding area-based designs for retrieve-value and compare-values tasks in both accuracy and completion time [@zengReviewCollationGraphical2023; @kimAssessingEffectsTask2018].

**Notes:** This rule is about protecting the readability of the primary positioned field, not about maximizing readability of the secondary field.

## Use when exact value reading is the priority <!-- role: context -->

- **User Goal:** Read exact values or compare two individual values of a main quantitative field.
- **Task:** Exact lookup or pairwise value comparison.
- **Data:** One categorical field and two quantitative fields.
- **Chart Setting:** A point-based multivariate view already uses position for the main quantitative field and still needs to show a second quantitative field.
- **Success Criterion:** Lower error and faster responses on individual-value tasks.

## Do not use this as a summary-task default <!-- role: exceptions -->

**Break it when:** The main task is to find group maxima or compare group averages. **Why:** The value-task advantage of color-saturation over area does not define the best choice for those summary tasks, where size-based encodings performed well.

## What you give up <!-- role: costs -->

**Sacrifice:** You give up the size-based summary cue that can help on some summary judgments.
**Risk:** Applying this rule to summary tasks can miss the benefit that area-based encodings showed there.
**Mitigation:** Use this rule only when exact reading of the positioned field is the main requirement.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Encode the secondary quantitative field with varying mark area while expecting fast, exact reading of the primary positioned field. **Why it fails:** The changing area interferes with decoding the positioned field.

## Compare the two encodings directly <!-- role: check -->

**Failure Sign:** Readers hesitate or misread the main positioned value when mark sizes vary.
**Quick Check:** Make two versions of the same chart, changing only the secondary quantitative field from area to color-saturation, and compare one lookup question and one pairwise comparison question.
**Stronger Test:** Measure answer time and error on a small set of representative exact-reading prompts.

## Edit the secondary encoding <!-- role: fix -->

- Remap the secondary quantitative field from area to color-saturation.
- Keep the main quantitative field on x or y.
- Revisit the encoding only if the task shifts from exact value reading to group-level summaries.
