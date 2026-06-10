---
id: keep-bars-unwrapped-for-maximum-lookup
title: Keep oversized bars unwrapped when the maximum must be found quickly
bibliography: references.bib
description: For maximum-value lookup in single-view categorical bar charts, prefer
  the standard unwrapped bar layout on bar charts with disproportionate values to
  improve readability and mitigate counting burden for readers scanning the tallest
  category.
labels:
- purpose:refine
- basis:empirical
- task:extreme
- chart:bar
- data:categorical
- quality:readability:use
- lever:layout-structure
- shape:outlier-rich
---

## Keep the maximum bar unwrapped <!-- role: advice -->

Use a standard bar chart instead of a wrapped-bar layout when the main job is to spot the largest category quickly. For example, avoid wrapping a dominant bar when readers would need to count several folds to confirm which category is the maximum.

## Why standard bars help maximum lookup <!-- role: reason -->

A continuous bar length is easier to scan for a maximum than a wrapped bar split into repeated segments. Once wrapping forces readers to count folds or mentally sum segments, the largest bar becomes less immediate to read.

**Mechanism:** Standard bars preserve a single continuous length cue for the maximum, while wrapped bars replace that cue with a segmented structure that can slow or disrupt largest-bar detection.

**Evidence:** The source study reports that wrapped bars were less accurate for largest-bar identification on higher H-spread datasets and took longer on largest-bar identification tasks, while participant feedback also described many wraps as cumbersome [@karduniBoisWrappedBar2020; @zengReviewCollationGraphical2023].

## Use when the maximum bar is the message <!-- role: context -->

- **User Goal:** Identify the largest category quickly and correctly.
- **Task:** Find the high-end extreme in a category comparison.
- **Data:** A dominant category creates a very tall bar relative to the rest.
- **Chart Setting:** Single-view, single-series bar chart on a linear scale.
- **Audience:** Readers are scanning for which category is highest.
- **Success Criterion:** Faster and more accurate identification of the maximum bar.

## Do not use when low-end readability is the priority <!-- role: exceptions -->

**Break it when:** The smallest categories are hard to distinguish in the standard bar chart and low-end extreme identification matters more than fastest maximum lookup. **Why:** In that situation, wrapping can recover readability for the smallest bars.

## Tradeoffs of keeping bars unwrapped <!-- role: costs -->

**Sacrifice:** You keep the dominant bar easy to scan but may leave the smallest bars visually compressed.
**Risk:** Readers may miss or confuse the smallest categories when one bar dominates the chart.
**Mitigation:** Use an unwrapped layout only when maximum lookup matters more than low-end accuracy.

## Common misuse of standard bars <!-- role: mistakes -->

**Mistake:** Keep a standard bar chart when one oversized bar flattens the smallest bars but the chart still needs accurate low-end reading. **Why it fails:** The continuous maximum cue remains strong, but the smallest categories stay hard to see.

## How to test the choice <!-- role: check -->

**Failure Sign:** Reviewers hesitate over the tallest category in the wrapped version or misread which bar is largest.
**Quick Check:** Compare standard and wrapped versions and ask reviewers to identify the largest category; keep the standard version if it yields cleaner maximum selection.
**Stronger Test:** Count how many folds the dominant bar would need; treat multiple wraps as a warning sign for maximum-bar lookup.

## What to change <!-- role: fix -->

- Replace the wrapped-bar layout with a standard bar layout.
- Remove repeated folds from the dominant bar so its full length remains one continuous cue.
- Reserve wrapped bars for cases where smallest-bar readability is more important than fastest maximum detection.
