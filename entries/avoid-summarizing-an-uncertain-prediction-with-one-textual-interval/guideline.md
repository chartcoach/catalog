---
id: avoid-summarizing-an-uncertain-prediction-with-one-textual-interval
title: Avoid summarizing an uncertain prediction with one textual interval
bibliography: references.bib
description: For repeated uncertainty decisions with changing stakes, avoid single-interval
  text on predictive displays to prevent decision quality from depending on one chosen
  interval and address inflexible risk communication for non-expert users.
labels:
- purpose:refine
- basis:empirical
- chart:text:avoid
- quality:fidelity:use
- lever:text-annotation
- operator:uncertainty
- communication:framing
---

## Single-interval text summaries <!-- role: advice -->

Do not make one textual probability interval the only uncertainty cue when users need to adjust risk across situations. For example, avoid reducing the forecast to a sentence like "85% chance after X minutes"; the study's 60%, 85%, and 99% text variants led to materially different decisions, and the 85% version learned poorly.

## Why single-interval text fails across changing stakes <!-- role: reason -->

A single textual interval hard-codes one risk threshold into the display. When the costs of waiting and missing change from one decision to the next, readers cannot adapt that fixed interval to the new tradeoff as well as they can with a more expressive uncertainty display.

**Mechanism:** Single-interval text exposes only one cut through the distribution, so the display becomes sensitive to the chosen probability level instead of letting readers inspect the threshold that best matches the current situation.

**Evidence:** Text displays were highly sensitive to the communicated interval: text99 and text60 approached lower-performing dotplot performance, while text85 produced poor decisions with little learning, leading the paper to attribute the weakness to the lower expressiveness of single-interval text [@fernandesUncertaintyDisplaysUsing2018].

## Use when stakes and acceptable risk change across decisions <!-- role: context -->

- **User Goal:** Adjust action timing as the cost of waiting and the cost of missing change.
- **Task:** Repeatedly choose among several possible threshold times under uncertainty.
- **Data:** A predictive distribution where different probability cutoffs may be appropriate in different situations.
- **Chart Setting:** A predictive display that may otherwise be tempting to compress into a short sentence.
- **Audience:** Non-experts making repeated decisions.
- **Success Criterion:** Decision quality should not depend heavily on one arbitrarily chosen probability interval.

## Do not apply this rule when one fixed threshold is all that matters <!-- role: exceptions -->

**Break it when:** One fixed risk threshold is the only quantity that matters across uses. **Why:** The main weakness of single-interval text is inflexibility when the best threshold changes from situation to situation.

## Tradeoffs of avoiding single-interval text <!-- role: costs -->

**Sacrifice:** A more expressive uncertainty display takes more space and attention than one short sentence.
**Risk:** If the situation truly has one fixed risk threshold, the richer display may add unnecessary detail.
**Mitigation:** Reserve richer uncertainty displays for settings where waiting and missing costs vary.

## Common failure with single-interval text <!-- role: mistakes -->

**Mistake:** Reusing one confidence level as the sole textual summary across changing situations. **Why it fails:** The chosen interval level steers the decision toward that single threshold and can underperform when the stakes differ.

## Check whether the text summary is too rigid <!-- role: check -->

**Failure Sign:** The display states only one probability interval in text and offers no other uncertainty structure.
**Quick Check:** Ask whether two scenarios with different waiting and missing costs would still receive the same text summary and the same implied threshold.
**Stronger Test:** Test several interval levels; if decision quality changes materially with the chosen level, the text summary is too rigid.

## Fix single-interval text summaries <!-- role: fix -->

- Remove the single interval sentence as the only uncertainty encoding.
- Replace it with a low-density quantile dotplot when users need to inspect multiple possible thresholds.
- Replace it with a complementary cumulative distribution plot when the main question is the chance remaining after a chosen time.
