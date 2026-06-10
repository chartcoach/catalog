---
id: use-parallel-coordinates-instead-of-table-for-cluster-identification
title: Use a parallel coordinates plot instead of a table for cluster identification
bibliography: references.bib
description: For cluster-identification tasks on sparse multivariate quantitative
  data, prefer a parallel coordinates plot over a table to improve fidelity and address
  slow cell-by-cell similarity search in static views.
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

## Replace the table for cluster search <!-- role: advice -->

Use a parallel coordinates plot when the job is to find a cluster in multivariate quantitative data. For example, replace a table with a parallel coordinates plot when readers must identify the clustered subset inside a 4-attribute, 8-record display.

## Why parallel coordinates help cluster search <!-- role: reason -->

A table makes readers compare many cells across records, while a parallel coordinates plot turns multivariate similarity into visible line patterns across shared axes.

**Mechanism:** Parallel coordinates expose similarity across several attributes at once. This reduces the cell-by-cell comparison burden of a table.

**Evidence:** The collated record ranks the parallel coordinates plot above the table on both clustering accuracy and time, and the original experiment found tables worst on clustering while parallel coordinates plots were best overall [@zengReviewCollationGraphical2023; @kanjanaboseMultitaskComparativeStudy2015].

## Use when cluster finding matters more than exact lookup <!-- role: context -->

- **User Goal:** Choose the subset of records that forms a cluster.
- **Data:** 8 records with 4 quantitative attributes.
- **Chart Setting:** Static representations of the same records and attributes with no interaction.
- **Success Criterion:** More correct and faster cluster choices.

## Do not use this choice for exact lookup <!-- role: exceptions -->

**Break it when:** The user goal is exact value retrieval rather than cluster identification. **Why:** In the same study, the table was the fastest representation for direct value lookup.

## Tradeoffs of replacing a table with parallel coordinates <!-- role: costs -->

**Sacrifice:** You give up the fastest form for exact value lookup.
**Risk:** Replacing the table when the task is still direct lookup adds unnecessary tracing work.
**Mitigation:** Keep the table for lookup prompts and switch to parallel coordinates for cluster search.

## Common clustering failure <!-- role: mistakes -->

**Mistake:** Leaving the data in table form when the task is to identify a cluster. **Why it fails:** The table forced slower and less accurate multivariate similarity judgments than the parallel coordinates plot.

## Check the clustering choice <!-- role: check -->

**Failure Sign:** Reviewers scan across many rows and columns and still miss the intended cluster.
**Quick Check:** Show the same clustering prompt in a table and in a parallel coordinates plot, and compare which version gets the correct subset faster.
**Stronger Test:** Repeat matched clustering prompts and compare both accuracy and completion time.

## Fix the clustering view <!-- role: fix -->

- Replace the table with a parallel coordinates plot for cluster-identification tasks.
- Move the same records and attributes from cells into shared axes with one polyline per record.
- Keep the table only for exact value-retrieval prompts.
