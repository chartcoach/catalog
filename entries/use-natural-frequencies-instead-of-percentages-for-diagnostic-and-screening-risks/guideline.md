---
id: use-natural-frequencies-instead-of-percentages-for-diagnostic-and-screening-risks
title: Use natural frequencies instead of percentages for diagnostic and screening
  risks
bibliography: references.bib
description: For interpreting single-risk results in diagnostic or screening contexts,
  prefer natural-frequency wording on quantitative risk labels and captions to improve
  fidelity and mitigate incorrect risk estimates for health professionals and consumers.
labels:
- purpose:refine
- basis:empirical
- scope:single-result
- data:quantitative
- quality:fidelity:use
- lever:text-annotation
- operator:uncertainty
- component:label:use
---

## Use frequency counts with a shared denominator <!-- role: advice -->

Rewrite diagnostic and screening risks as counts out of a common population size instead of standalone percentages. For example, show the base rate, the number of positive results among affected cases, and the number of positive results among unaffected cases as counts such as “100 of 10,000,” “90 of 100,” and “99 of 9,900” rather than only as percentages.

## Why frequency counts work here <!-- role: reason -->

Natural frequencies keep the reference class visible. That makes it easier to combine the base rate with true-positive and false-positive information and infer the actual post-test risk.

**Mechanism:** Frequency counts anchor each part of the problem to the same pool of cases, so readers can reason from cases instead of translating between disconnected percentages.

**Evidence:** In the review, health professionals and consumers understood risks better when diagnostic or screening information was presented as natural frequencies rather than percentages, with a moderate overall effect on objective understanding. [@aklUsingAlternativeStatistical2011]

## Use when the display communicates post-test risk <!-- role: context -->

- **User Goal:** Explain the chance of a condition after a diagnostic or screening result.
- **Task:** Help readers estimate or interpret a single risk correctly.
- **Data:** One risk statement built from a base rate and test-result information.
- **Chart Setting:** Risk is communicated numerically in labels, captions, table cells, or scenario text.
- **Audience:** Health professionals or consumers.
- **Success Criterion:** Readers give a more accurate risk estimate or interpretation.

## Do not use when the message is about treatment benefits or harms <!-- role: exceptions -->

**Break it when:** The display communicates intervention effects rather than diagnostic or screening test results. **Why:** The review’s evidence for natural frequencies versus percentages was limited to diagnostic and screening contexts and did not test treatment-effect communication.

## Costs of rewriting percentages as frequencies <!-- role: costs -->

**Sacrifice:** You give up the shortest numeric phrasing.
**Risk:** The statement can become longer and use larger numbers.
**Mitigation:** Keep all counts on one clearly repeated denominator.

## Common failure with frequency wording <!-- role: mistakes -->

**Mistake:** Mix percentages with counts or use different denominators inside the same risk statement. **Why it fails:** Readers lose the shared reference class needed to infer the post-test risk.

## How to review this choice <!-- role: check -->

**Failure Sign:** Readers can repeat the input percentages but cannot estimate the chance of disease after a positive result.
**Quick Check:** Scan the display for prevalence, sensitivity, and false-positive information shown only as percentages.
**Stronger Test:** Ask readers to estimate the post-test risk and compare the percentage version with a frequency version; keep the version that yields more answers close to the correct value.

## What to change <!-- role: fix -->

- Convert each percentage into counts on a common denominator.
- State affected positives and unaffected positives explicitly as case counts.
- Replace a percentage-only answer prompt with an “x out of y” readout.
- Remove mixed-format wording that forces readers to translate between percentages and counts.
