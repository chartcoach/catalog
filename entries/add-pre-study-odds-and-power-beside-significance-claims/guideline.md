---
id: add-pre-study-odds-and-power-beside-significance-claims
title: Add pre-study odds and study power beside significance claims
bibliography: references.bib
description: For interpreting a claimed statistically significant finding from a single
  study, use text annotation on result displays to improve trust and mitigate p-value-only
  interpretation for audiences judging research credibility.
labels:
- purpose:refine
- basis:empirical
- quality:trust:use
- lever:text-annotation
- communication:context
- component:annotation:use
- operator:uncertainty
---

## Add post-study probability context <!-- role: advice -->

Add annotation that states the pre-study odds and study power behind a claimed statistically significant finding. For example, pair the p-value threshold crossing with an estimated PPV or false-positive-risk readout and name the assumed R value used to interpret the result.

## Why context beyond p-values works <!-- role: reason -->

A significance threshold alone invites readers to equate statistical significance with truth when the paper shows that truth depends on more than the p-value.

**Mechanism:** Adding pre-study odds and power changes the readout from “the result passed 0.05” to “the result is more or less believable under explicit assumptions.”

**Evidence:** The paper argues that research should not be interpreted based only on p-values and shows that the post-study probability a finding is true depends on prior probability, study power, and the significance level [@ioannidisWhyMostPublished2005].

## Use when a display reports a positive significance claim <!-- role: context -->

- **User Goal:** Judge whether a claimed relationship is likely true after one study.
- **Task:** Interpret a significance claim rather than only detect threshold crossing.
- **Data:** One or a few statistically significant findings from a single study.
- **Chart Setting:** A chart or table reports p-values, significance labels, or claimed effects.
- **Audience:** Readers assessing research credibility.
- **Success Criterion:** Readers can see the assumptions that make the claim more or less believable.

## Do not use when there is no positive claim to interpret <!-- role: exceptions -->

**Break it when:** The display does not make a positive research claim reaching statistical significance. **Why:** The paper defines PPV for claimed findings and focuses its argument on relationships investigators claim exist.

## Costs of adding PPV context <!-- role: costs -->

**Sacrifice:** You must expose assumptions about pre-study odds and power.
**Risk:** Those assumptions can be debated because they are partly subjective.
**Mitigation:** State the assumed values directly on the display.

## Common p-value-only mistake <!-- role: mistakes -->

**Mistake:** Report only p-values or threshold labels without stating prior-odds or power context. **Why it fails:** It leaves out the terms that the paper says determine whether a claimed finding is likely true.

## Check whether significance is overinterpreted <!-- role: check -->

**Failure Sign:** A significance claim has no stated R, power, PPV, or false-positive-risk context.
**Quick Check:** Ask whether a reader could explain why the result is likely true without using only `p < 0.05`.
**Stronger Test:** Verify that the display provides enough information to compute or inspect PPV under the stated assumptions.

## Fix the p-value-only display <!-- role: fix -->

- Add a PPV or false-positive-risk annotation next to each claimed finding.
- State the assumed pre-study odds or R value used for that readout.
- Add the study power used to interpret the claim.
