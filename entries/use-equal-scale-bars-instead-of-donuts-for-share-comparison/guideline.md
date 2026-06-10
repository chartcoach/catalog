---
id: use-equal-scale-bars-instead-of-donuts-for-share-comparison
title: Use equal-scale bars instead of donuts for share comparison
bibliography: references.bib
description: For compare tasks on record lists of part-to-whole percentages, prefer
  equal-scale bar charts over donut charts to improve readability and mitigate weak
  within-record and between-record comparisons for readers scanning across categories
  and across records.
labels:
- purpose:select
- basis:heuristic
- task:compare
- scope:record-list
- chart:bar:use
- chart:pie-donut:avoid
- quality:readability
- lever:chart-family
---

## Replace donuts with equal-scale bars <!-- role: advice -->

Replace donut charts with equal-scale bars when readers need to compare category shares within records and between records. For example, unroll each donut into a 0–100 bar instead of repeating similar-looking donuts with percentages and a total in the center.

## Why equal-scale bars work better here <!-- role: reason -->

Bars give each category share a common linear scale, so readers can compare the three parts inside one record and the same part across many records without judging angles around a ring.

**Mechanism:** A shared 0–100 baseline makes the category breakdown easier to scan than donut slices, especially when many records use the same three categories.

**Evidence:** The post recommends “unrolling” the donuts into bars because bars make it easier to compare categories both within and between records, and the revised display uses mini bars on an equal 0–100 scale [@mintzer_donuts_into_bars_2025].

## Use when comparison is the job <!-- role: context -->

- **User Goal:** Compare the category breakdown for one record and compare the same categories across many records.
- **Task:** Read part-to-whole percentages accurately across a record list.
- **Data:** Many records, each split into the same few percentage categories.
- **Chart Setting:** The current design repeats many donut charts that look similar at a glance.
- **Audience:** Readers who need to scan across categories and across records.
- **Success Criterion:** Readers can judge one record’s breakdown and compare it with other records without struggling with the shape of the marks.

## Do not use when that comparison is not required <!-- role: exceptions -->

**Break it when:** The display is not meant to support within-record and between-record comparison of the category shares. **Why:** The source recommends bars specifically to improve those two comparison paths.

## What you trade away <!-- role: costs -->

**Sacrifice:** You lose the donut hole as a place to park the total.
**Risk:** If you switch to bars without relocating the total, the count summary can disappear.
**Mitigation:** Move the total into its own column or adjacent text field instead of keeping it inside the mark.

## Common failure around this change <!-- role: mistakes -->

**Mistake:** Keep the donuts and only add a total in the center. **Why it fails:** The donuts still look alike, and the extra number does not make the category shares easier to compare.

## How to test the choice <!-- role: check -->

**Failure Sign:** Many donuts look almost the same at a glance.
**Quick Check:** Compare two versions and ask which makes it easier to judge the middle category for one record and then compare that category across two records.
**Stronger Test:** Ask a reviewer to rank a few records on one category in the donut version and the bar version; choose bars if the answers come faster and with more confidence.

## What to change <!-- role: fix -->

- Convert each donut into a bar that runs from 0 to 100%.
- Keep every bar on the same 0–100 scale.
- Move any total now shown in the donut hole into a separate column or label.
- Keep one row per record so the same categories line up for comparison.
