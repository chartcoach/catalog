---
id: add-confidence-intervals-to-latest-poll-bars
title: Add confidence intervals to latest-poll bar or column charts
bibliography: references.bib
description: For comparison at a single timepoint, use uncertainty intervals on bar
  or column charts of poll estimates to improve trust and address exact-looking summaries
  for readers who might mistake estimates for final results.
labels:
- purpose:refine
- basis:heuristic
- time:timepoint
- chart:bar
- quality:trust:use
- lever:encoding
- operator:uncertainty
---

## Add the uncertainty range <!-- role: advice -->

Add confidence intervals when a bar or column chart shows poll estimates rather than final results. For example, pair each party bar with an uncertainty range around the latest poll, the latest-polls average, or a forecast so the graphic does not read like certified results.

## Why the uncertainty range works <!-- role: reason -->

The interval makes the chart say “estimate” instead of “final count,” which helps readers carry the uncertainty into their interpretation.

**Mechanism:** Showing a range around each value makes the provisional nature of the estimate visible at the point of comparison.

**Evidence:** The post explicitly recommends showing confidence intervals on latest-poll bar or column charts to communicate uncertainty and the fact that polls are not the final results [@muth_german_election_2021].

## Use when the chart shows estimates, not outcomes <!-- role: context -->

- **User Goal:** Compare the latest standing without hiding uncertainty.
- **Task:** Read current estimates and their plausible range together.
- **Data:** Poll or forecast values at one timepoint.
- **Chart Setting:** A bar or column chart already summarizes the latest estimate.
- **Success Criterion:** Readers see both the central estimate and that it is not final.

## Do not use when the numbers are final results <!-- role: exceptions -->

**Break it when:** The chart is showing final election results rather than polls or forecasts. **Why:** The interval is introduced here specifically to signal uncertainty and non-finality.

## Tradeoffs of the uncertainty range <!-- role: costs -->

**Sacrifice:** The chart no longer presents each value as one exact-looking number.
**Risk:** Readers who want only a single headline value may see a less tidy snapshot.
**Mitigation:** Keep the central estimate visible and add the interval around that same value.

## Common failure around the uncertainty range <!-- role: mistakes -->

**Mistake:** Show latest-poll bars as precise endpoints with no interval. **Why it fails:** The chart hides uncertainty and can look like a final-results graphic.

## Check whether the estimate still looks final <!-- role: check -->

**Failure Sign:** Each bar ends at one precise point with no visible range.
**Quick Check:** Ask whether the chart could be mistaken for final results; if yes, the uncertainty is not visible enough.
**Stronger Test:** Verify that every estimate has an explicit interval that can be seen without reading the data table.

## Fix the exact-looking estimate <!-- role: fix -->

- Add a confidence interval to each bar or column.
- Keep the poll estimate visible as the central value inside that interval.
- State that the chart shows estimates rather than final results.
