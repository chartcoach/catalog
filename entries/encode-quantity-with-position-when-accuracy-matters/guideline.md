---
id: encode-quantity-with-position-when-accuracy-matters
title: Encode quantitative values with position when reading accuracy matters
bibliography: references.bib
description: For exact quantitative lookup or comparison, use position encoding instead
  of area encoding on quantitative displays to improve fidelity and mitigate magnitude
  misjudgment for readers making precise value readings.
labels:
- purpose:refine
- basis:empirical
- task:retrieve
- quality:fidelity:use
- lever:encoding
- reading-mode:exact
- channel:position:use
- channel:area:avoid
---

## Change the quantitative channel to position <!-- role: advice -->

Encode the critical quantitative field with position when readers need accurate value judgments. For example, move a magnitude from circle area or rectangle area into x or y position, especially when the current readout depends on bubble-chart or treemap-style area judgments.

## Use the more accurate perceptual channel <!-- role: reason -->

Position supports more accurate quantitative perception than area. Area judgments, including circular and rectangular area, make precise reading harder and can push readers toward wrong magnitude estimates.

**Mechanism:** Position lets readers judge magnitude more accurately than area, so exact value lookup and comparison become more reliable.

**Evidence:** Position encoding has the highest accuracy, followed by length, angle and rotation, and then area; circular and rectangular area encodings are especially low in accuracy, which helps explain why bubble charts and treemaps are harder to read [@bornerDataVisualizationLiteracy2019].

## Use when the quantitative readout must be precise <!-- role: context -->

- **User Goal:** Read or compare quantitative values accurately.
- **Task:** Exact lookup or exact comparison.
- **Data:** Quantitative values encoded visually.
- **Chart Setting:** A display currently uses, or could use, area to encode magnitude.
- **Audience:** Readers making precise value readings.
- **Success Criterion:** Readers judge magnitudes accurately.

## Do not use when exact quantitative judgment is not the success criterion <!-- role: exceptions -->

**Break it when:** Precise value reading is not the success criterion. **Why:** This rule is specifically about perceptual accuracy of quantitative encoding.

## Accept the cost of changing the encoding <!-- role: costs -->

**Sacrifice:** Area-based magnitude displays such as circular or rectangular size coding.
**Risk:** The chart form may need to change if it currently depends on area as the main quantitative channel.
**Mitigation:** Keep the same data but remap the critical quantitative field to x or y position.

## Avoid leaving the critical number in area <!-- role: mistakes -->

**Mistake:** Keeping the main quantitative readout in circle area or rectangle area when readers need exact values. **Why it fails:** Area is perceived less accurately than position, so magnitude judgments become harder.

## Compare the area version to a position version <!-- role: check -->

**Failure Sign:** Reviewers disagree or hesitate when reading values from size alone.
**Quick Check:** Redraw one key quantitative readout with position instead of area and see whether the value is easier to read.
**Stronger Test:** Ask a reviewer to retrieve or compare the same values from an area version and a position version; keep the position version if answers are more accurate.

## Remap the magnitude to position <!-- role: fix -->

- Move the critical quantitative field from area into x or y position.
- Rebuild bubble-chart or treemap-style quantity readouts with position-based marks when exact reading matters.
- Keep the data values the same so the main change is the encoding channel.
