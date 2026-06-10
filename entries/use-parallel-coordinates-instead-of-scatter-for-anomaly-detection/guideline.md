---
id: use-parallel-coordinates-instead-of-scatter-for-anomaly-detection
title: Use a parallel coordinates plot instead of a scatter plot for anomaly detection
bibliography: references.bib
description: For anomaly-detection tasks on sparse multivariate quantitative data,
  prefer a parallel coordinates plot over a scatter plot to improve fidelity and mitigate
  missed anomalous records in static views.
labels:
- purpose:select
- basis:empirical
- chart:parallel:use
- chart:scatter:avoid
- data:quantitative
- quality:fidelity:use
- lever:chart-family
- measure:multi
- density:sparse
---

## Choose the anomaly-finding view <!-- role: advice -->

Use a parallel coordinates plot when the job is to detect anomalous records in multivariate quantitative data. For example, replace a scatter plot view with a parallel coordinates plot when readers must choose one or two anomalous records in a 4-attribute, 8-record display.

## Why parallel coordinates help anomaly detection <!-- role: reason -->

A parallel coordinates plot can show a record separating from the overall multivariate pattern across several attributes at once, while a scatter plot view spreads the evidence across pairwise plots.

**Mechanism:** Parallel coordinates keep each record together as one line across all shown attributes. This helps readers spot records that depart from the rest by value range or by relationship pattern.

**Evidence:** The collated record ranks the parallel coordinates plot above the scatter plot on anomaly-detection accuracy, and the original experiment concluded that parallel coordinates plots generally outperformed the other tested representations on outlier detection [@zengReviewCollationGraphical2023; @kanjanaboseMultitaskComparativeStudy2015].

**Notes:** Do not assume a large improvement on every performance measure; the clearest supported gain is better anomaly-detection performance.

## Use when anomaly finding is the job <!-- role: context -->

- **User Goal:** Choose one or two anomalous records.
- **Data:** 8 records with 4 quantitative attributes.
- **Chart Setting:** Static representations of the same records and attributes with no interaction.
- **Success Criterion:** More correct anomaly choices.

## Do not use this choice for exact lookup <!-- role: exceptions -->

**Break it when:** The user goal is exact value retrieval rather than anomaly detection. **Why:** In the same study, the table was faster for direct value lookup.

## Tradeoffs of replacing a scatter plot with parallel coordinates <!-- role: costs -->

**Sacrifice:** You should not expect the switch to solve every speed problem by itself.
**Risk:** Changing to parallel coordinates only for speed may not deliver a strong payoff.
**Mitigation:** Use this change when anomaly-detection accuracy is the main success criterion.

## Common anomaly-finding failure <!-- role: mistakes -->

**Mistake:** Keeping a scatter plot view when anomaly-detection accuracy is the main success criterion. **Why it fails:** The scatter plot view underperformed the parallel coordinates plot for this task in the studied multivariate setup.

## Check the anomaly-detection choice <!-- role: check -->

**Failure Sign:** Reviewers miss the anomalous record or choose the wrong pair in the scatter plot view.
**Quick Check:** Show the same anomaly-detection prompt in a scatter plot view and in a parallel coordinates plot, and compare which version produces the correct anomaly choice more often.
**Stronger Test:** Repeat matched anomaly prompts and compare accuracy first, then completion time.

## Fix the anomaly-finding view <!-- role: fix -->

- Replace the scatter plot view with a parallel coordinates plot for anomaly-detection tasks.
- Show each record as one polyline across shared attribute axes instead of distributing the evidence across scatter plots.
- Switch back to a table only when the task changes to exact value retrieval.
