---
id: use-the-title-or-description-as-a-color-key
title: Use the title or description as a color key
bibliography: references.bib
description: For visualizations whose titles or descriptions can name the colored
  groups, use color-coded headline text on title or description copy to improve readability
  and mitigate separate legend lookup for readers entering through the surrounding
  text.
labels:
- purpose:refine
- basis:heuristic
- quality:readability:use
- lever:text-annotation
- component:title:use
- communication:framing
- aesthetic:color:use
---

## Title-based color key <!-- role: advice -->

Color category names in the title or description when that text can explain the palette before readers enter the chart. For example, use colored group names in the headline to teach the mapping, and keep direct labels or a classic key as extra reminders if readers may start elsewhere.

## Why title-based color keys work <!-- role: reason -->

The headline is often the first text readers see. When it names the groups in their chart colors, it explains the palette before the reader reaches the plotting area and can sometimes replace a separate legend.

**Mechanism:** The title or description becomes an immediate decoding aid, so readers learn the color mapping from the framing text instead of making a separate legend lookup.

**Evidence:** The article shows titles and descriptions that name categories in their chart colors, says this can remove the need for an additional classic color key and save space, and also notes that extra reminders such as direct labels or a legend can still help readers who start reading elsewhere [@muth_remind_colors_2023].

## When to use a title-based color key <!-- role: context -->

- **User Goal:** Explain the color mapping before readers study the chart itself.
- **Data:** The visualization uses named categories that can be mentioned in text.
- **Chart Setting:** The title or description can naturally include the relevant group names.
- **Success Criterion:** Readers can infer the color mapping from the headline text without a separate legend lookup.

## When not to use a title-based color key <!-- role: exceptions -->

**Break it when:** The category text would be blue in a way that looks like a link. **Why:** Readers may interpret the colored text as clickable instead of as a color key.

## Costs of a title-based color key <!-- role: costs -->

**Sacrifice:** The title or description must explicitly name the colored groups.
**Risk:** A headline-only explanation can be missed when readers start in the middle of the visualization.
**Mitigation:** Keep direct labels or a traditional legend as a second reminder when readers may enter elsewhere.

## Common title-key mistake <!-- role: mistakes -->

**Mistake:** Removing every other color reminder once the title explains the palette. **Why it fails:** Readers who begin with the chart body may miss the headline-based key.

## How to test a title-based color key <!-- role: check -->

**Failure Sign:** The title uses color, but a reader still cannot restate which group each colored word refers to in the chart.
**Quick Check:** Hide the classic legend and check whether the title or description alone teaches the intended mapping.
**Stronger Test:** Start reading from the middle of the visualization and confirm that another reminder remains if the headline is no longer in view.

## How to fix a weak title-based color key <!-- role: fix -->

- Rewrite the title or description so it names the colored groups directly.
- Apply the matching category colors to those group names in the text.
- Add direct labels or a traditional legend when readers can start away from the headline.
