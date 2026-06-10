---
id: sort-comparable-categories-by-rank-when-the-task-is-to-find-top-contributors
title: Sort comparable categories by rank when the task is to find top contributors
bibliography: references.bib
description: For comparison and lookup tasks on grouped quantitative categories, use
  descending rank order to improve readability and mitigate slow scanning for analysts
  identifying top contributors.
labels:
- purpose:refine
- basis:empirical
- task:compare
- operator:rank
- reading-mode:lookup
- group-cardinality:many
- quality:readability:use
- lever:scale-order
---

## Order categories by contribution rank <!-- role: advice -->

Sort comparable categories in explicit descending order when the viewer needs to find the largest contributors quickly. For example, arrange clusters within a list or stack by their rank contribution, and keep sequential order only for fields whose position itself carries meaning, such as age groups or years.

## Turn scanning into direct rank lookup <!-- role: reason -->

When comparable categories are ordered by contribution, the viewer can find the top items immediately. When sequence itself carries meaning, that sequence should stay intact instead of being overwritten by magnitude order.

**Mechanism:** Rank order supports direct top-item lookup, while natural sequence supports progression reading; each ordering serves a different task.

**Evidence:** The paper repeatedly places comparable cause, risk, and location clusters in rank order to support comparison and ranking tasks, while it uses sequential ordering for age groups and years so users can understand their progression and classification [@olaSimpleChartsDesign2016].

## Use when rank is the question <!-- role: context -->

- **User Goal:** Identify the largest or most important contributors.
- **Task:** Rank, compare, or scan a many-category set.
- **Data:** A grouped set of comparable categories with quantitative contribution values.
- **Chart Setting:** Lists, stacks, or similar ordered category displays.
- **Success Criterion:** Reviewers can find the top contributors without scanning the full set in arbitrary order.

## Do not use when the order itself communicates progression <!-- role: exceptions -->

**Break it when:** The category order itself carries meaning, such as chronological progression or age sequence. **Why:** Reordering by value would hide the sequence that users need to understand.

## Trade off natural order against top-item lookup <!-- role: costs -->

**Sacrifice:** You give up the original category sequence for that display.
**Risk:** If you apply rank order to sequence fields, you obscure progression.
**Mitigation:** Reserve rank ordering for comparable category sets and preserve natural order for time- and age-based structures.

## Avoid arbitrary order for ranking tasks <!-- role: mistakes -->

**Mistake:** Leaving comparable categories in an unsorted order when the task is to find the top contributors. **Why it fails:** The viewer must scan the whole display to infer rank instead of reading it directly from position.

## Test whether the top contributor is visually obvious <!-- role: check -->

**Failure Sign:** A reviewer has to inspect many labels or marks before identifying the largest category.
**Quick Check:** Ask whether the top few contributors can be named directly from position alone.
**Stronger Test:** Compare the ranked version with an unsorted version and check which one supports faster top-contributor lookup without losing a meaningful sequence.

## Reorder the categories to match the lookup task <!-- role: fix -->

- Sort comparable categories into descending contribution order.
- Keep the same rank direction throughout that ordered set.
- Preserve natural sequential order for age- or time-based structures instead of rank-sorting them.
