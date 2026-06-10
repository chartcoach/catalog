---
id: define-technical-terms-and-thresholds-on-the-display
title: Define technical terms and thresholds on the display
bibliography: references.bib
description: For communicating uncertainty on labels, legends, or captions, use operational
  definitions and familiar wording to improve fidelity and address term misinterpretation
  for readers outside the field.
labels:
- purpose:refine
- basis:empirical
- quality:fidelity:use
- lever:text-annotation
- component:label:use
- communication:context
- access:plain-language:use
- needs:low-domain-knowledge
---

## Defined term labels <!-- role: advice -->

Add the operational meaning of specialist terms and thresholds directly to the display, and replace expert jargon when testing shows it fails. For example, define what counts as the forecasted or measured event, state any threshold or measurement rule, and use a familiar phrase instead of a field-specific status label when the familiar phrase communicates better.

## Why defined term labels work <!-- role: reason -->

Readers map familiar-looking words to everyday meanings unless the display tells them otherwise. A label that looks ordinary but carries a technical meaning can mislead even when the numbers around it are correct.

**Mechanism:** Operational definitions and familiar wording align the reader’s interpretation with the expert’s intended meaning before the reader interprets the uncertainty or the recommendation.

**Evidence:** The paper gives examples where common words used in uncommon ways misled readers, argues that clarity is an empirical question answered by user testing, and recommends more familiar wording when scientists’ preferred terms fail to communicate [@fischhoffCommunicatingScientificUncertainty2014].

## When to use defined term labels <!-- role: context -->

- **User Goal:** Interpret a category, threshold, or forecast term correctly.
- **Data:** The display uses a named event, status category, or measurement threshold that could have a technical definition.
- **Chart Setting:** Key terms appear in labels, legends, captions, or headlines.
- **Audience:** Readers do not share the field’s specialist vocabulary.
- **Success Criterion:** Readers paraphrase the term and threshold the way the display intends.

## When not to rely on this rule alone <!-- role: exceptions -->

**Break it when:** User testing shows the intended audience already interprets the expert term and threshold correctly. **Why:** The paper says a more familiar term is needed when the preferred term fails to communicate, not automatically in every case.

## Tradeoffs of defined term labels <!-- role: costs -->

**Sacrifice:** You give up some label brevity and some formal field terminology.
**Risk:** Longer definitions can crowd a compact display.
**Mitigation:** Keep the short term in the main label and move the operational definition to a caption, legend note, or annotation.

## Common failure with defined term labels <!-- role: mistakes -->

**Mistake:** Keeping a technical label because it looks like an everyday word. **Why it fails:** Readers apply the everyday meaning and can misread the chart’s event, severity, or threshold.

## How to check defined term labels <!-- role: check -->

**Failure Sign:** Readers can repeat the label text but cannot explain what the label means here.
**Quick Check:** Ask a reviewer, “What does this term count, and what threshold defines it?” and see whether the answer matches the display.
**Stronger Test:** User-test the label with intended readers and compare their paraphrases before and after adding the definition.

## How to fix defined term labels <!-- role: fix -->

- Add the event definition and threshold directly to the caption or legend.
- Replace a specialist label with a more familiar phrase when testing shows the familiar phrase is understood more accurately.
- Keep the formal term only if you also add a plain-language gloss.
- Revise the headline or status label if a technical category name hides the actual severity of the condition being shown.
