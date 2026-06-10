---
id: calibrate-size-encodings-across-point-shapes
title: Calibrate size encodings across different point shapes
bibliography: references.bib
description: For point-to-point size comparison, prefer calibrated size encodings
  on scatterplots that use different point shapes to improve fidelity and mitigate
  apparent-size bias for viewers comparing multivariate points.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:scatter
- quality:fidelity:use
- lever:encoding
- channel:shape
- operator:difference
---

## Size calibration across shapes <!-- role: advice -->

Adjust point sizes across shape categories instead of giving every shape the same nominal diameter. For example, equal-sized squares, outline squares, and `⊤` shapes were seen as larger than stars, diamonds, or plus shapes, so mixed-shape size encodings need calibration before viewers compare values.

## Why equal diameter is not equal apparent size <!-- role: reason -->

Point shape changes perceived size. Readers do not judge diameter in isolation, so the same nominal size can overstate some categories and understate others.

**Mechanism:** Shape adds visual mass and edge structure that bias size judgments, which distorts direct comparisons when shape and size are both encoded on the same scatterplot points.

**Evidence:** The experiment found a strong effect of shape on size perception: shapes with more visual density on the top or bottom, including `⊤`, filled squares, and outline squares, were perceived as larger, while stars and diamonds were perceived as smaller at the same nominal size. The paper also built models to normalize size computations across shapes, and the review collated this study as evidence that shape biases size perception in scatterplots [@smartMeasuringSeparabilityShape2019; @zengReviewCollationGraphical2023].

**Notes:** The paper reports that shape affected size perception much more than size affected shape perception over the tested range.

## Use when size is compared across shape categories <!-- role: context -->

- **User Goal:** Compare magnitudes from point size.
- **Task:** Judge which point encodes the larger value.
- **Data:** Scatterplot data where shape distinguishes categories and size encodes another attribute.
- **Chart Setting:** A scatterplot that uses multiple point-shape categories with equal or similar nominal sizes.
- **Audience:** Readers comparing quantitative values across shaped points.
- **Success Criterion:** Equal values look equal in size across the chosen shape set.

## Do not use when all compared marks share one shape <!-- role: exceptions -->

**Break it when:** Every directly compared mark uses the same point shape. **Why:** The reported bias was between different shape categories, not within a single shared shape.

## Tradeoffs of calibrating size <!-- role: costs -->

**Sacrifice:** You give up raw one-scale diameter consistency across all shapes.
**Risk:** Leaving one diameter scale unadjusted across mixed shapes can misstate value differences.
**Mitigation:** Apply calibration only to the mixed-shape comparisons readers actually need to make.

## Common failure with mixed-shape size encoding <!-- role: mistakes -->

**Mistake:** Assigning equal nominal diameters to filled and unfilled shape variants and assuming they will look equal. **Why it fails:** Some shapes were judged larger far more often than others even when rendered at the same nominal size.

## How to review apparent size bias <!-- role: check -->

**Failure Sign:** Equal-valued points of different shapes do not look equal in size.
**Quick Check:** Place equal-diameter examples of two candidate shapes side by side and ask which looks larger.
**Stronger Test:** Repeat the comparison at the smallest and largest planned sizes and reject pairs that produce consistent bias.

## What to change <!-- role: fix -->

- Normalize rendered sizes across the chosen shape set instead of applying one raw diameter scale to every shape.
- Test same-value pairs of candidate shapes before finalizing the size encoding.
- If you cannot calibrate mixed shapes, keep direct size comparisons within a single shape category.
