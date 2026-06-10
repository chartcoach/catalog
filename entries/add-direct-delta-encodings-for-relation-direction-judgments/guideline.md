---
id: add-direct-delta-encodings-for-relation-direction-judgments
title: Add direct delta encodings for relation-direction judgments
bibliography: references.bib
description: For compare tasks on grouped paired quantitative displays, use direct
  delta encoding on paired-value charts to improve fidelity and mitigate slow, error-prone
  extraction of increase-versus-decrease relations for viewers.
labels:
- purpose:refine
- basis:empirical
- task:compare
- scope:grouped-result
- data:quantitative
- quality:fidelity:use
- lever:encoding
- operator:difference
---

## Direct delta marks for direction <!-- role: advice -->

Encode each pairwise difference with one signed delta mark when readers need to detect increase-versus-decrease relations. For example, replace separate point pairs, bar pairs, or slope pairs with one delta mark per pair when readers must find the lone opposite relation or decide whether increases or decreases are more common.

## Why direct delta marks work for direction judgments <!-- role: reason -->

A direct delta mark turns the relation itself into the thing the reader sees. That removes the need to infer direction by comparing two separate values in every pair.

**Mechanism:** A single signed difference makes increase versus decrease explicit, so readers do not have to extract a relation from two separate marks before answering the question.

**Evidence:** In the collated record, direct delta encodings outperformed matched individual-value encodings for target-relation search time and for judging which relation direction was more prevalent across paired quantitative displays; the original study reports large advantages for delta encodings on both tasks across position, length, and slope-based variants [@zengReviewCollationGraphical2023; @nothelferMeasuresBenefitDirect2020].

**Notes:** The reported advantage was strongest for finding a target relation and remained substantial for judging which direction was more prevalent.

## Use when direct relation direction is the job <!-- role: context -->

- **User Goal:** Identify whether paired values increase or decrease.
- **Task:** Find one target relation or judge which relation direction is more prevalent across many pairs.
- **Data:** Paired quantitative values, with one relation per category or item.
- **Chart Setting:** The current display shows each member of a pair separately and can be revised to show one derived difference per pair.
- **Success Criterion:** Faster search or higher accuracy for relation-direction judgments.

## Do not use when the original values are still required <!-- role: exceptions -->

- **Break it when:** Readers must use the original individual values, not just the difference between them. **Why:** A delta-only encoding removes the original-value context.
- **Break it when:** Readers must connect deltas back to conditions on the original values, such as filtering by an original-value threshold. **Why:** The needed base-value information is no longer visible in the delta-only view.
- **Break it when:** Showing every possible pairing would require too many delta encodings. **Why:** The number of pairings can grow combinatorially and consume too much space.

## Costs of direct delta marks for direction judgments <!-- role: costs -->

**Sacrifice:** You give up direct visibility of the original values when you show only deltas.
**Risk:** Insights tied to the original data points can become harder to notice.
**Mitigation:** Use the delta-focused view only when relation direction is the central question, and limit it to the pairings readers actually need.

## Common failure mode with direct delta marks <!-- role: mistakes -->

**Mistake:** Replacing a paired-value view with only deltas when the reader still needs the base values to interpret the result. **Why it fails:** The chart no longer supports decisions that depend on the original values or their thresholds.

## Check whether direct delta marks are needed <!-- role: check -->

**Failure Sign:** Readers scan pair by pair to work out which pairs increase, decrease, or reverse the dominant pattern.
**Quick Check:** Build a matched delta version of the same display and ask a reviewer to answer one target-relation question and one majority-direction question in both versions.
**Stronger Test:** Time the answers or compare accuracy across the two versions; keep the delta version if it is faster or more accurate.

## Fix the relation-direction view <!-- role: fix -->

- Compute one signed difference for each pair.
- Replace the task-focused pairwise view with one delta mark per pair instead of showing only separate values.
- Put positive and negative deltas on opposite sides of a baseline, or use opposite slope direction, so increase and decrease are explicit.
- Limit delta encodings to the pairings the reader actually needs to judge.
