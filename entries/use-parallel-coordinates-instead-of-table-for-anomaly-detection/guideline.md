---
id: use-parallel-coordinates-instead-of-table-for-anomaly-detection
title: Use a parallel coordinates plot instead of a table for anomaly detection
bibliography: references.bib
description: For anomaly-detection tasks on sparse multivariate quantitative data,
  prefer a parallel coordinates plot over a table to improve fidelity and address
  slow cell-by-cell outlier search in static views.
labels:
- purpose:select
- basis:empirical
- chart:parallel:use
- chart:table:avoid
- data:quantitative
- quality:fidelity:use
- lever:chart-family
- measure:multi
- density:sparse
---

## Replace the table for anomaly search <!-- role: advice -->

Use a parallel coordinates plot when the job is to find anomalous records in multivariate quantitative data. For example, replace a table with a parallel coordinates plot when readers must identify one or two anomalies in a 4-attribute, 8-record display.

## Why parallel coordinates help anomaly search <!-- role: reason -->

A table forces readers to scan cells across many records, while a parallel coordinates plot exposes records that separate from the overall multivariate pattern.

**Mechanism:** Parallel coordinates make departures across several attributes visible in one integrated line pattern. This reduces the cell-by-cell comparison burden of a table during anomaly search.

**Evidence:** The collated record ranks the parallel coordinates plot above the table on anomaly-detection accuracy and time, and the original experiment found tables worst on outlier detection while parallel coordinates plots performed best overall [@zengReviewCollationGraphical2023; @kanjanaboseMultitaskComparativeStudy2015].

## Use when anomaly finding matters more than exact lookup <!-- role: context -->

- **User Goal:** Choose one or two anomalous records.
- **Data:** 8 records with 4 quantitative attributes.
- **Chart Setting:** Static representations of the same records and attributes with no interaction.
- **Success Criterion:** More correct and faster anomaly choices.

## Do not use this choice for exact lookup <!-- role: exceptions -->

**Break it when:** The user goal is exact value retrieval rather than anomaly detection. **Why:** In the same study, the table was the fastest representation for direct value lookup.

## Tradeoffs of replacing a table with parallel coordinates <!-- role: costs -->

**Sacrifice:** You give up the fastest form for exact value lookup.
**Risk:** Replacing the table when the task is still direct lookup adds unnecessary tracing work.
**Mitigation:** Keep the table for lookup prompts and switch to parallel coordinates for anomaly search.

## Common anomaly-search failure <!-- role: mistakes -->

**Mistake:** Leaving the data in table form when the task is to find anomalies. **Why it fails:** The table forced slower and less accurate multivariate anomaly judgments than the parallel coordinates plot.

## Check the anomaly-detection choice <!-- role: check -->

**Failure Sign:** Reviewers scan rows and columns for a long time and still miss the anomalous record.
**Quick Check:** Show the same anomaly-detection prompt in a table and in a parallel coordinates plot, and compare which version gets the correct answer faster.
**Stronger Test:** Repeat matched anomaly prompts and compare both accuracy and completion time.

## Fix the anomaly view <!-- role: fix -->

- Replace the table with a parallel coordinates plot for anomaly-detection tasks.
- Move the same records and attributes from cells into shared axes with one polyline per record.
- Keep the table only for exact value-retrieval prompts.
