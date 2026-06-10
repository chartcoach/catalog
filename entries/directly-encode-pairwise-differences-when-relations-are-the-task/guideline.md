---
id: directly-encode-pairwise-differences-when-relations-are-the-task
title: Directly encode pairwise differences when relations are the task
bibliography: references.bib
description: For relation judgments over paired quantitative values, use direct delta
  encoding on comparison charts to improve fidelity and mitigate slow, error-prone
  extraction of increases and decreases for viewers scanning or summarizing many pairs.
labels:
- purpose:refine
- basis:empirical
- task:relate
- data:quantitative
- quality:fidelity:use
- lever:encoding
- operator:difference
- group-cardinality:binary
---

## Add direct delta marks <!-- role: advice -->

Encode each pairwise difference with its own delta mark when viewers need to read change or direction across paired values. For example, add a delta bar, delta dash, or delta slope instead of making readers infer change from two separate bars, dashes, or slopes when they must find which pairs increase, judge which direction is more common, or estimate average change.

## Why direct delta marks improve pairwise relation reading <!-- role: reason -->

A delta mark turns a two-mark relation into one readout. That removes the extra step of extracting direction or magnitude from separate marks before searching, counting, or averaging across many pairs.

**Mechanism:** Direct delta encoding reduces pairwise relation reading to a single visual feature, while individual-value encoding forces viewers to compute the relation between two marks for each pair.

**Evidence:** Across three tasks, direct delta encodings outperformed individual-value encodings for pairwise relation perception. The gain ranged from 25% lower error for estimating average delta to 30% higher accuracy for judging which relation was more prevalent, and up to 49-95% faster search rates for locating a target relation among many pairs [@nothelferMeasuresBenefitDirect2020].

**Notes:** The paper found that the size of the benefit depends strongly on the task, with the largest gain in target-relation search.

## Use when pairwise relations are the message <!-- role: context -->

- **User Goal:** Identify increases or decreases, find the one pair with a target relation, decide which relation direction is more common, or estimate average change.
- **Task:** Compare many paired values by their relation rather than by their standalone absolute values.
- **Data:** Quantitative values organized into pairs where the difference between the two values is meaningful.
- **Chart Setting:** The chart currently shows paired values as separate marks, or can add a separate encoding for the pairwise difference.
- **Audience:** Viewers who must make fast or brief-glance relation judgments.
- **Success Criterion:** Faster search, higher accuracy on relation direction, or lower error on average-difference judgments.

## Do not use delta-only encoding when original-value context must stay visible <!-- role: exceptions -->

- **Break it when:** Viewers must connect a difference back to the original values, such as restricting attention to values past a threshold, and the design can only show one representation. **Why:** A delta-only display removes the original-value context and can hide insights tied to the base values.
- **Break it when:** The number of possible pairings is large enough that adding delta encodings would overwhelm the available space. **Why:** Delta encodings consume display real estate, and possible pairings can grow combinatorially.

## Tradeoffs of direct delta encoding <!-- role: costs -->

**Sacrifice:** A delta-only design can remove the original paired values from view.\
**Risk:** Adding deltas for many possible pairings can consume space quickly.\
**Mitigation:** Add delta encoding only for the pairwise relations central to the task, or show deltas alongside the original values when both are needed.

## Common failure mode for pairwise relation charts <!-- role: mistakes -->

**Mistake:** Showing only two separate values per pair when the main question is about the direction or size of change across many pairs. **Why it fails:** Readers must extract each relation from two marks, which was much slower and less accurate than reading a single delta mark.

## Test whether relation extraction is the bottleneck <!-- role: check -->

**Failure Sign:** Reviewers can read individual values, but are slow or error-prone when asked which pairs increased, which direction dominates, or what the average change is.\
**Quick Check:** Compare the current individual-value version to a version with explicit delta marks on the same pairwise question.\
**Stronger Test:** Time a target-relation search or compare accuracy and error on brief majority-direction or average-delta judgments between the two versions.

## Edit the chart to expose differences directly <!-- role: fix -->

- Add one explicit delta mark for each pair whose change is the intended message.
- Recode paired bars, dashes, or slopes as delta bars, delta dashes, or delta slopes for the relation task.
- Keep the original paired values visible alongside the delta encoding when readers also need original-value context.
- Limit delta encodings to the specific pairings readers need to compare when space is constrained.
