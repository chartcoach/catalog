---
id: use-linear-bar-layout-for-exact-reading-of-daily-patterns
title: Use a linear bar layout for exact reading of daily patterns
bibliography: references.bib
description: For exact lookup and comparison in cyclic-time daily patterns, use a
  linear layout on bar charts to improve fidelity and mitigate slow value decoding
  and AM/PM selection mistakes for non-expert readers.
labels:
- purpose:refine
- basis:empirical
- time:cyclic-time
- chart:bar
- quality:fidelity
- lever:layout-structure
- reading-mode:exact
- audience:general-public
---

## Choose the linear bar layout <!-- role: advice -->

Use a linear bar layout when readers must locate hours, read values, compare paired hours, or find the maximum in a daily pattern. For example, use a 24-hour or 2×12-hour linear bar chart instead of a clock-like rose chart when the chart’s job is exact reading rather than decorative presentation.

## Why the linear layout works <!-- role: reason -->

Linear bars keep hourly positions on one straight reading path and avoid the extra radial decoding step. That reduces time spent locating hours and reading values, and it lowers common mistakes such as swapping AM and PM or misreading how far a bar extends from the center.

**Mechanism:** A linear layout supports direct left-to-right lookup and length comparison, while a radial layout asks readers to decode angle, ring position, and radial extent before answering.

**Evidence:** In the daily-pattern study, linear charts were faster than radial charts for locating a specified hour, reading a value, finding the maximum, and comparing paired AM/PM intervals, and linear charts were preferred overall by non-expert readers [@waldnerComparisonRadialLinear2020; @zengReviewCollationGraphical2023].

**Notes:** The clock-like 12-hour radial layout did not produce more unguided observations than the linear layout.

## Use when exact reading matters <!-- role: context -->

- **User Goal:** Read or compare hourly values correctly and quickly.
- **Task:** Locate a specific hour, read an hourly value, compare paired AM/PM hours, or find the daily maximum.
- **Data:** One aggregated value per hour across a 24-hour cycle.
- **Chart Setting:** Static daily-pattern display shown as a bar-based chart in a web or report setting.
- **Audience:** Non-expert or untrained readers.
- **Success Criterion:** Faster answers, fewer reading errors, and higher reader acceptance.

## When to break the rule <!-- role: exceptions -->

**Break it when:** Visual novelty or engagement matters more than accurate and efficient reading. **Why:** Some readers described the radial versions as more appealing or fun even though they performed worse with them.

## What you trade away <!-- role: costs -->

**Sacrifice:** You give up the more unusual radial look that some readers found more interesting.
**Risk:** A single linear view can take more horizontal space than a radial view.
**Mitigation:** If width is limited, split the linear bar chart into two 12-hour panels instead of switching to a rose chart.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Switching to a clock-like rose chart because daily data feels naturally circular. **Why it fails:** Readers were slower, made more exact-reading errors, and often struggled to decode the chart despite the clock metaphor.

## How to test the choice <!-- role: check -->

**Failure Sign:** Readers hesitate, swap AM and PM, or misread the value on a marked hour.
**Quick Check:** A/B test the linear bar version against the radial version on one locate-time question and one read-value question.
**Stronger Test:** Show each version briefly without instructions and compare how many correct observations readers can report.

## What to change <!-- role: fix -->

- Replace the rose chart with a 24-hour linear bar chart when one continuous view fits.
- If one wide chart does not fit, split the linear bar chart into two 12-hour panels rather than keeping a radial layout.
- Keep the daily pattern in a bar-based linear form for tasks that require exact reading.
