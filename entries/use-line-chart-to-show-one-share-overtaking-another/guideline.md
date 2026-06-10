---
id: use-line-chart-to-show-one-share-overtaking-another
title: Use a line chart to show one share overtaking another
bibliography: references.bib
description: For ordered-time comparison when the message is that one share overtook
  another, use a line chart instead of stacked columns to improve readability and
  mitigate hidden crossover patterns for readers tracking changes between series.
labels:
- purpose:select
- basis:heuristic
- time:ordered-time
- chart:line:use
- chart:bar:avoid
- operator:difference
- quality:readability
- lever:chart-family
---

## Focus the chart on the crossover <!-- role: advice -->

Replace stacked columns with a line chart when the message is that one share overtook another over time. For example, plot the two relevant shares as lines instead of showing every share in a full stacked column series.

## Why the crossover becomes clearer <!-- role: reason -->

A stacked column chart keeps the part-to-whole structure visible, but that structure can hide the simpler story that one share crossed another. A line chart puts the comparison directly on the page.

**Mechanism:** The line chart makes the crossing and relative ordering between the two shares easy to see without requiring the reader to decode all shares of the total.

**Evidence:** The post says that for time data, a line chart should be considered when the aim is to show that one share overtook another, because it communicates the message more clearly and does not require showing all shares of the total [@muth_stacked_columns_2018].

## Use when the crossover is the message <!-- role: context -->

- **User Goal:** Show that one share became larger than another over time.
- **Task:** Compare two changing shares and locate the crossover.
- **Data:** Time data with shares that are part of a total.
- **Chart Setting:** A stacked column chart is being considered for a crossover story.
- **Audience:** Readers need the main comparison to be obvious.
- **Success Criterion:** The change in ordering between the two shares is immediately visible.

## Do not use when the full part-to-whole structure must stay explicit <!-- role: exceptions -->

**Break it when:** The chart must show all shares together as parts of the whole. **Why:** A line chart no longer signals that part-to-whole relationship intuitively.

## What you give up <!-- role: costs -->

**Sacrifice:** You give up the intuitive stacked display of all shares in one total.
**Risk:** Readers may not read the chart as a part-to-whole display anymore.
**Mitigation:** Use this switch only when the crossover itself is the point of the chart.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keeping all shares in stacked columns when only one crossover matters. **Why it fails:** The message gets buried inside a more complex part-to-whole display.

## Test the chart choice <!-- role: check -->

**Failure Sign:** The intended takeaway is about one share passing another, but the crossing is hard to spot.
**Quick Check:** Draft the relevant shares as lines and compare that version with the stacked columns; if the line version makes the overtaking obvious, use it.
**Stronger Test:** Ask whether the message still works after removing the other shares; if it does, the stacked columns are unnecessary.

## Revise the design <!-- role: fix -->

- Replace the stacked columns with a line chart for the shares that need to be compared.
- Remove shares that do not support the overtaking message.
- Make the crossover the main visual event in the chart.
