---
id: use-mortality-framing-when-comparing-treatment-curves-across-time-spans
title: Use mortality framing when comparing treatment curves across different time
  spans
bibliography: references.bib
description: For ordered-time treatment comparisons, use mortality framing on line
  charts to improve fidelity and mitigate temporal inconsistency bias when readers
  compare effectiveness across displays with different year spans.
labels:
- purpose:refine
- basis:empirical
- task:compare
- time:ordered-time
- chart:line
- quality:fidelity
- lever:encoding
- communication:framing
---

## Mortality framing on treatment curves <!-- role: advice -->

Encode and label the outcome as mortality rather than survival when readers must compare treatment effectiveness across curves that span different lengths of time. For example, present mortality curves for shorter and longer follow-up windows instead of survival curves when the relative treatment effect stays constant but the year range changes.

## Why mortality framing reduces cross-span distortion <!-- role: reason -->

Survival framing makes shorter time spans look less effective even when the relative effect is unchanged. Mortality framing reduces that inconsistency when readers compare displays across different follow-up lengths.

**Mechanism:** Mortality curves reduce the tendency to treat shorter-span and longer-span displays as if the different endpoint framing changed the treatment effect.

**Evidence:** The paper reports that, with survival curves, treatment efficacy is perceived as poorer when the data span fewer rather than more years even when relative effectiveness stays constant, and that this temporal inconsistency bias is attenuated with mortality curves [@lipkusNumericVerbalVisual2007].

## Use when the same treatment effect is shown over different year spans <!-- role: context -->

- **User Goal:** Compare treatment effectiveness across options or displays.
- **Task:** Compare time-based outcome curves.
- **Data:** The same relative effectiveness shown over different year spans.
- **Chart Setting:** Line-based survival or mortality curves used side by side or across conditions.
- **Audience:** Readers interpreting treatment effects from the curves.
- **Success Criterion:** Judgments of effectiveness stay consistent across shorter and longer follow-up windows.

## Do not use as a special correction when time span is constant <!-- role: exceptions -->

**Break it when:** All compared curves use the same time span and cross-span inconsistency is not the issue. **Why:** The reported bias arose when the same relative effectiveness was shown across shorter and longer year ranges.

## Tradeoffs of switching to mortality framing <!-- role: costs -->

**Sacrifice:** You give up the more positive survival framing.\
**Risk:** Readers may focus more on deaths than survivals.\
**Mitigation:** Use mortality framing when consistency across time spans matters more than positive wording.

## Common failure mode in time-span comparisons <!-- role: mistakes -->

**Mistake:** Using survival curves to compare options across shorter and longer time spans as if the frame were neutral. **Why it fails:** Shorter-span survival curves can make the treatment look less effective even when the relative effect is unchanged.

## How to test for temporal inconsistency bias <!-- role: check -->

**Failure Sign:** Shorter-span curves are judged less effective than longer-span curves despite the same relative effect.\
**Quick Check:** Compare reader judgments from a survival version and a mortality version of the same data.\
**Stronger Test:** Test whether effectiveness ratings stay stable when you change only the time span.

## What to change <!-- role: fix -->

- Relabel and replot the outcome as mortality over time.
- Use the same data with mortality curves for the shorter and longer spans.
- Keep the relative treatment effect constant across the paired displays.
