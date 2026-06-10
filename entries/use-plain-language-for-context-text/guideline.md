---
id: use-plain-language-for-context-text
title: Use plain language for context text
bibliography: references.bib
description: For explanatory context in visualizations, use plain-language text annotation
  on captions, annotations, labels, and titles to improve readability and mitigate
  confusion from technical or abstract wording for audiences with low domain knowledge.
labels:
- purpose:refine
- basis:rhetorical
- quality:readability
- lever:text-annotation
- communication:context
- needs:low-domain-knowledge
- access:plain-language:use
---

## Plain-language context text <!-- role: advice -->

Write captions, annotations, labels, and titles that explain context in plain language. For example, replace technical terms and high-level wording in future-scenario descriptions and in notes about uncertainty or data processing with everyday phrasing that states the message directly.

## Why plain-language context text works <!-- role: reason -->

Plain-language context text lets readers focus on the chart's message instead of first decoding scientific or abstract wording. This matters most when the text explains scenarios, methods, or uncertainty to people without strong domain background.

**Mechanism:** Plain-language captions and annotations reduce interpretation effort, help readers distill the main narrative, and prevent context text from becoming a barrier to understanding.

**Evidence:** Viewers and practitioners criticized complex or abstract wording in captions, annotations, labels, and titles; lay viewers especially struggled with technical future-scenario descriptions, older scientific captions were harder to distill into messages than newer plain-language captions, and simplifying wording was emphasized as essential advice for newcomers [@schuster_being_2024; @koesten_what_2023; @schuster_who_2023].

## Use when context text explains the chart <!-- role: context -->

- **User Goal:** Understand what the chart is saying and what surrounding scenario or method text means.
- **Task:** Read explanatory context that frames the visualization's message.
- **Data:** The visualization includes scenario, uncertainty, or data-processing context that needs text explanation.
- **Chart Setting:** Captions, annotations, labels, or titles are carrying part of the explanation.
- **Audience:** Lay viewers, mixed audiences, or newcomers with low domain knowledge.
- **Success Criterion:** Readers can restate the chart's main message and context without getting stuck on terminology.

## Do not use outside context-setting text <!-- role: exceptions -->

**Break it when:** The chart is not relying on captions, annotations, labels, or titles to convey explanatory context. **Why:** This guidance is specifically about rewriting context-setting text, not about changing other parts of the visualization.

## Tradeoffs of plain-language context text <!-- role: costs -->

**Sacrifice:** You give up some high-level scientific vocabulary in the chart text.\
**Risk:** If you simplify too aggressively, you can strip out the essential point the text needs to convey.\
**Mitigation:** Keep the core scenario, method, or uncertainty point, then rewrite it in everyday language.

## Common jargon mistakes <!-- role: mistakes -->

- **Mistake:** Leaving technical terms or abstract phrases in captions and annotations. **Why it fails:** Readers with low domain knowledge struggle to interpret the context, especially in future-scenario descriptions.
- **Mistake:** Describing uncertainty or data processing in high-level scientific language instead of a direct message. **Why it fails:** Readers have a harder time distilling the chart's main narrative.

## Check context wording <!-- role: check -->

**Failure Sign:** Reviewers describe the caption or annotation as technical, abstract, or hard to turn into a clear message.\
**Quick Check:** Highlight every term used to explain a scenario, uncertainty, or data-processing step; if several terms require domain knowledge to unpack, rewrite them.\
**Stronger Test:** Ask a newcomer to paraphrase the caption, annotation, label, or title in everyday language; if they cannot state the main point cleanly, simplify the wording.

## Fix technical wording <!-- role: fix -->

- Replace technical terms in captions and annotations with everyday wording.
- Rewrite high-level scenario descriptions as direct statements of what the scenario means.
- Rewrite uncertainty and data-processing notes as short plain-language explanations.
- Simplify titles and labels to the essential wording a newcomer can follow.
