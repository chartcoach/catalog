---
id: add-margin-of-error-ranges-to-poll-estimates
title: Add margin-of-error ranges to poll estimates
bibliography: references.bib
description: For single-poll reporting at a timepoint, use margin-of-error ranges
  on poll estimate charts to improve fidelity and mitigate false precision for readers
  comparing close results.
labels:
- purpose:refine
- basis:heuristic
- scope:single-result
- time:timepoint
- quality:fidelity
- lever:encoding
- operator:uncertainty
- communication:credibility
---

## Margin-of-error ranges <!-- role: advice -->

Show the published margin of error directly on each poll estimate. For example, add a plus/minus range around a bar or value marker and state the margin on the chart instead of presenting one percentage as an exact result.

## Why margin-of-error ranges work <!-- role: reason -->

Uncertainty ranges keep sample-based poll estimates from being read like final election results. They make it visible when an apparent lead may still fall within the plausible range of error.

**Mechanism:** Showing a range changes the reading task from treating a poll as a settled outcome to judging whether differences are meaningful within sampling error.

**Evidence:** The post says election polls are extrapolated from samples of about 1,000 to 3,000 respondents and usually carry a margin of error of roughly plus or minus two to three percentage points, and that ignoring these margins is misleading, especially in tight races. [@jockers_election_polls_2021]

## Where margin-of-error ranges apply <!-- role: context -->

- **User Goal:** Report current standing from a poll without overstating certainty.
- **Task:** Compare close poll values.
- **Data:** Sample-based poll estimates with a published margin of error.
- **Chart Setting:** A single poll graphic at one timepoint with one reported percentage per candidate or party.
- **Audience:** Readers deciding how much confidence to place in a close race.
- **Success Criterion:** Readers can see both the reported estimate and the plausible range around it.

## When margin-of-error ranges fail <!-- role: exceptions -->

**Break it when:** The graphic shows actual election results rather than sample-based poll estimates. **Why:** The rule is for sampled estimates with statistical error, not realized vote counts.

## Tradeoffs of margin-of-error ranges <!-- role: costs -->

**Sacrifice:** You give up some exact-looking simplicity.
**Risk:** Readers must interpret a range instead of a single number.
**Mitigation:** State the plus/minus value directly on the chart so the range is easy to read.

## Common mistakes with margin-of-error ranges <!-- role: mistakes -->

**Mistake:** Reporting the poll percentage alone and leaving the margin of error out of the chart. **Why it fails:** Readers still see the estimate as if it were a precise result.

## How to check margin-of-error ranges <!-- role: check -->

**Failure Sign:** Close poll values appear as exact percentages with no visible range.
**Quick Check:** Look at each plotted estimate and verify that the chart shows an upper and lower bound, not just one number.
**Stronger Test:** Compare the displayed range against the published plus/minus margin and confirm they match.

## How to fix missing margin-of-error ranges <!-- role: fix -->

- Add a visible range around each poll estimate using the published plus/minus margin.
- State the margin of error on the chart, not only in surrounding text.
- Redraw any exact-looking single value so the estimate and its uncertainty are shown together.
