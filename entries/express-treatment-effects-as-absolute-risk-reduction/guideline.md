---
id: express-treatment-effects-as-absolute-risk-reduction
title: Express treatment effects as absolute risk reduction
bibliography: references.bib
description: For treatment-benefit comparison in non-temporal numerical risk displays,
  prefer absolute risk reduction wording on baseline-versus-treatment summaries to
  improve fidelity and mitigate misreading of treatment benefit for mixed-numeracy
  audiences.
labels:
- purpose:refine
- basis:empirical
- task:compare
- quality:fidelity:use
- lever:text-annotation
- operator:difference
- communication:framing
- knowledge:mixed
---

## Rewrite benefit as baseline versus treated risk <!-- role: advice -->

State treatment benefit as absolute risk reduction rather than as a relative percentage reduction when readers must understand the size of the effect. For example, say how many out of a fixed population are affected without treatment and with treatment instead of giving only a statement such as “reduces risk by 13%.”

## Why absolute wording improves understanding <!-- role: reason -->

Absolute risk reduction exposes both the starting risk and the treated risk directly. That removes a conversion step readers would otherwise have to do from a relative percentage reduction.

**Mechanism:** Readers can compare two stated risks directly instead of reconstructing the effect from a relative claim.

**Evidence:** In the experiment, numerical descriptions using absolute rather than relative risk reduction produced much higher accuracy in older adults and students; icon arrays added further gains, but the advantage of absolute wording remained large [@galesicUsingIconArrays2009].

## Use when the message is a reduction from baseline to treatment <!-- role: context -->

- **User Goal:** Explain the size of a treatment or screening benefit in numbers.
- **Task:** Compare baseline risk with treated risk.
- **Data:** Two risks for the same outcome, without treatment and with treatment.
- **Chart Setting:** The message is carried in numerical text or labels accompanying a display.
- **Audience:** Readers with mixed numeracy.
- **Success Criterion:** Readers can correctly state the size of the risk reduction.

## Do not use when there is no baseline-versus-treatment comparison <!-- role: exceptions -->

**Break it when:** The message is not a reduction from a baseline risk to a treated risk. **Why:** The source only tests absolute versus relative wording for benefit comparisons built from two risk values.

## What you trade away <!-- role: costs -->

**Sacrifice:** A brief relative-percentage claim can sound more dramatic than the equivalent absolute statement.
**Risk:** Using relative reduction alone can make a modest benefit seem larger than readers can accurately recover from the display.
**Mitigation:** If you want stronger comprehension without reverting to relative-only wording, pair the absolute statement with icon arrays.

## Common failure mode with benefit wording <!-- role: mistakes -->

**Mistake:** Labeling benefit only as a relative reduction while omitting the baseline and treated risks. **Why it fails:** Readers are less accurate at recovering the actual size of the effect.

## How to test the revision <!-- role: check -->

**Failure Sign:** Readers cannot tell how many people are affected before and after treatment from the wording alone.
**Quick Check:** Compare a relative-risk-reduction phrasing against an absolute-risk-reduction phrasing for the same scenario and ask for the untreated and treated counts out of a fixed population.
**Stronger Test:** Score whether readers derive the reduction correctly within a small tolerance rather than only recognizing that the treatment helps.

## What to change <!-- role: fix -->

- Replace a lone relative-percentage reduction with both the untreated risk and the treated risk.
- Express those two risks over the same denominator as counts or percentages.
- Keep the comparison explicit in one sentence or one compact summary.
- If you need additional support, add paired icon arrays rather than reverting to relative-only wording.
