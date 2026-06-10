---
id: add-direct-delta-encodings-for-average-difference-judgments
title: Add direct delta encodings for average-difference judgments
bibliography: references.bib
description: For overview judgments of paired quantitative differences in grouped
  displays, use direct delta encoding on paired-value charts to improve fidelity and
  mitigate errors from mentally subtracting each pair before averaging for viewers.
labels:
- purpose:refine
- basis:empirical
- scope:grouped-result
- data:quantitative
- quality:fidelity:use
- lever:encoding
- operator:difference
- reading-mode:overview
---

## Direct delta marks for average difference <!-- role: advice -->

Encode each pairwise difference with one delta mark when readers need the average difference across many pairs. For example, replace separate point pairs or bar pairs with one delta mark per pair when readers must estimate the mean delta across the display.

## Why direct delta marks work for averaging <!-- role: reason -->

A direct delta mark lets readers average the differences themselves. It avoids forcing them to first infer a difference from every pair and only then summarize those inferred values.

**Mechanism:** Readers can average already-visible differences more precisely than differences they must first mentally extract from separate paired values.

**Evidence:** In the collated record, the direct delta version of the paired-value display produced lower error than matched individual-value encodings for the aggregate task; the original study reports significantly lower average-difference error for direct delta encodings than for separate point-pair and bar-pair encodings [@zengReviewCollationGraphical2023; @nothelferMeasuresBenefitDirect2020].

**Notes:** The reported improvement for average-difference estimation was smaller than the search advantage, but it was still consistent and statistically reliable.

## Use when readers must summarize many pairwise differences <!-- role: context -->

- **User Goal:** Judge the overall size of the difference across many pairs.
- **Task:** Estimate the average delta across the display.
- **Data:** Paired quantitative values with one derived difference per pair.
- **Chart Setting:** The current display shows each member of a pair separately and can be revised to show one computed difference per pair.
- **Success Criterion:** Lower error in estimating the average difference.

## Do not use when the original values are still part of the question <!-- role: exceptions -->

- **Break it when:** Readers must interpret the average difference together with the original values. **Why:** A delta-only encoding removes the original-value context.
- **Break it when:** Readers must subset or interpret differences by conditions on the original values. **Why:** Those source values are not visible in the delta-only view.
- **Break it when:** The number of required pairings would force too many delta encodings into the display. **Why:** The added pairwise views can consume too much space.

## Costs of direct delta marks for average-difference judgments <!-- role: costs -->

**Sacrifice:** You lose direct visibility of the original values when you show only deltas.
**Risk:** Readers may miss patterns that are tied to the individual data points rather than to their differences.
**Mitigation:** Use the delta-focused view only when the average difference is the main question, and restrict it to the needed pairings.

## Common failure mode with direct delta marks for averaging <!-- role: mistakes -->

**Mistake:** Asking readers to estimate an average difference from a display that still requires mental subtraction for every pair. **Why it fails:** The reader has to perform pairwise difference extraction before they can even start averaging.

## Check whether the average-difference view needs deltas <!-- role: check -->

**Failure Sign:** Readers appear to mentally subtract each pair before giving an overall average-difference estimate.
**Quick Check:** Build a matched delta version of the same display and ask a reviewer to estimate the average difference from both versions.
**Stronger Test:** Compare the absolute error of the two estimates; keep the delta version if the error drops.

## Fix the average-difference view <!-- role: fix -->

- Compute one difference value for each pair.
- Replace the separate paired-value marks in the summary view with one delta mark per pair.
- Encode positive and negative deltas with opposite direction relative to a baseline so the sign of the difference remains explicit.
- Limit delta encodings to the pairings that actually feed the average-difference judgment.
