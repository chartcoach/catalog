---
id: keep-icon-array-denominator-size-consistent
title: Keep denominator size consistent across equivalent icon arrays
bibliography: references.bib
description: For comparison of equivalent medical risks in non-temporal icon-array
  displays, prefer a fixed denominator size across otherwise matched views to improve
  fidelity and mitigate denominator-size bias for audiences comparing treatment effects.
labels:
- purpose:refine
- basis:empirical
- task:compare
- quality:fidelity:use
- lever:encoding
---

## Keep the total icon count fixed across comparisons <!-- role: advice -->

Keep the total number of icons consistent when comparing equivalent risks or treatment effects. For example, do not switch between 100-icon and 1,000-icon arrays for the same percentage, because the larger array makes the baseline risk and especially the treatment benefit look larger.

## Why denominator size changes perception <!-- role: reason -->

A larger denominator makes more people appear affected or helped even when the proportion is unchanged. That shifts perceived seriousness and helpfulness away from the underlying rate.

**Mechanism:** Readers react to the larger absolute count of marked icons, not only to the proportion they represent.

**Evidence:** In the experiment, 1,000-icon arrays produced somewhat higher seriousness ratings than 100-icon arrays for equivalent baseline risks and significantly higher helpfulness ratings for equivalent screening benefits [@galesicUsingIconArrays2009].

## Use when equal rates must remain comparable <!-- role: context -->

- **User Goal:** Compare risks or benefits fairly across displays.
- **Task:** Show equivalent rates without changing their perceived size.
- **Data:** The same proportion can be rendered with different possible denominators.
- **Chart Setting:** Icon arrays are used for untreated and treated outcomes.
- **Audience:** Readers interpreting baseline risk and treatment benefit.
- **Success Criterion:** Equivalent rates are not made to feel larger or smaller by denominator choice.

## Do not use when the absolute count itself is the message <!-- role: exceptions -->

**Break it when:** The absolute number of people represented is itself the message rather than an interchangeable presentation of the same rate. **Why:** The source tests denominator size as an alternative display choice for equivalent risks.

## What you trade away <!-- role: costs -->

**Sacrifice:** You give up a presentation lever that can make the same rate feel larger.
**Risk:** Switching from 100 to 1,000 icons can make equal risks and especially equal risk reductions seem bigger for reasons unrelated to the data.
**Mitigation:** Use one denominator size consistently for every comparable icon array in the set.

## Common failure mode with denominator choice <!-- role: mistakes -->

**Mistake:** Varying total icon count across otherwise equal icon arrays while treating them as directly comparable. **Why it fails:** Readers infer different seriousness and helpfulness from denominator size alone.

## How to test the revision <!-- role: check -->

**Failure Sign:** The same percentage appears in matched views with different total icon counts.
**Quick Check:** Scan all comparable icon arrays and verify that they use the same denominator.
**Stronger Test:** A/B test 100-icon and 1,000-icon versions of the same rate and check whether seriousness or helpfulness ratings drift.

## What to change <!-- role: fix -->

- Choose one denominator size for a comparison set and apply it to every icon array in that set.
- If you revise one view from 100 to 1,000 icons, revise all matched views.
- Do not enlarge the icon array just to make the same rate or benefit feel more important.
- Keep the untreated and treated icon arrays matched within each comparison.
