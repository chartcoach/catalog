---
id: express-uncertainty-with-numerical-probabilities-or-intervals
title: Express uncertainty with numerical probabilities or intervals
bibliography: references.bib
description: For communicating uncertainty in results or recommendations, use numerical
  uncertainty labels on annotations, legends, or captions to improve fidelity and
  mitigate inconsistent interpretation for readers unfamiliar with scientific verbal
  conventions.
labels:
- purpose:refine
- basis:empirical
- quality:fidelity:use
- lever:text-annotation
- operator:uncertainty
- component:label:use
- audience:decision-maker
- needs:low-domain-knowledge
---

## Quantitative uncertainty labels <!-- role: advice -->

Replace verbal uncertainty words with explicit numerical values or intervals on the display. For example, show a percentage probability, a ±X% variability estimate, or a credible interval instead of labels such as “rare,” “good evidence,” or “stable measurement.”

## Why numerical uncertainty labels work <!-- role: reason -->

Numerical uncertainty labels give readers a concrete readout instead of forcing them to guess what a field-specific word means. When the display uses only verbal qualifiers, different readers can leave with very different levels of confidence from the same message.

**Mechanism:** Explicit numbers reduce reliance on private language conventions and make the intended amount of uncertainty easier to extract from the display.

**Evidence:** The paper reports that laypeople often misinterpret verbal expressions of uncertainty, while most people can use explicit quantitative expressions well enough to extract their main message; it also argues that imprecise summaries leave observers guessing about uncertainty [@fischhoffCommunicatingScientificUncertainty2014].

**Notes:** The paper treats credible intervals as the preferred quantitative summary when uncertainty goes beyond observed variability alone.

## When to use numerical uncertainty labels <!-- role: context -->

- **User Goal:** Judge how uncertain a result or recommendation is.
- **Data:** Uncertainty can be summarized as a probability, variability estimate, or interval.
- **Chart Setting:** The display currently communicates uncertainty through labels, captions, legends, or boxed summaries.
- **Audience:** Readers are outside the field or do not share its verbal uncertainty conventions.
- **Success Criterion:** Readers can state the amount of uncertainty without translating a vague word.

## When not to rely on this rule alone <!-- role: exceptions -->

**Break it when:** The intended audience already shares the field’s verbal conventions and user testing shows the verbal term is interpreted consistently. **Why:** The paper frames misunderstanding as a problem when recipients do not know what experts mean by seemingly common terms, and it treats clarity as an empirical question.

## Tradeoffs of numerical uncertainty labels <!-- role: costs -->

**Sacrifice:** You give up some brevity.
**Risk:** A bare number can suggest more precision than intended.
**Mitigation:** Pair the number with the supporting uncertainty rationale or interval width rather than presenting a lone precise-looking value.

## Common failure with numerical uncertainty labels <!-- role: mistakes -->

**Mistake:** Replacing one vague uncertainty word with another vague uncertainty word. **Why it fails:** Readers still have to infer magnitude from unstated language conventions.

## How to check numerical uncertainty labels <!-- role: check -->

**Failure Sign:** The display says “rare,” “likely,” “good evidence,” or similar phrases without a number.
**Quick Check:** Can a reviewer point to a numerical probability, interval, or ± estimate for each uncertainty claim?
**Stronger Test:** Ask representative readers to paraphrase the uncertainty in their own words and compare whether their interpretations converge.

## How to fix numerical uncertainty labels <!-- role: fix -->

- Replace each verbal uncertainty label with a percentage probability or interval.
- Add a ±X% variability estimate where the display currently says a measure is stable or variable.
- Add a credible interval when the display summarizes an estimated effect or outcome.
- Add the short rationale for that number when the estimate could otherwise look more precise than intended.
