---
id: left-align-lengthy-chart-text
title: Left-align lengthy chart text
bibliography: references.bib
description: For multi-line chart text longer than short labels, use left alignment
  on titles and annotations to improve readability and mitigate messy edges and slower
  line-to-line reading for readers scanning longer text.
labels:
- purpose:refine
- basis:heuristic
- quality:readability
- lever:text-annotation
- aesthetic:composition:use
---

## Left alignment for long text <!-- role: advice -->

Left-align lengthy chart text instead of centering it. For example, use left alignment for multi-line titles or annotations above roughly 10 words so each line starts in the same place and the text block aligns neatly with nearby chart elements.

## Why left alignment helps longer reading <!-- role: reason -->

Longer text is easier to scan when each line begins at a predictable position. Centered text creates irregular edges and makes readers spend extra time finding the next line.

**Mechanism:** Left alignment creates a clean shared edge for line starts, which speeds multi-line reading and makes the text block sit more tidily beside chart elements.

**Evidence:** The source states that left- or right-aligned text looks tidier than centered text and specifically warns against center- and right-aligned annotations for lengthy text above roughly 10 words because readers need longer to find the beginning of the next line. [@muth_text_in_data_visualizations_2022]

## Use when text wraps into multiple lines <!-- role: context -->

- **User Goal:** Read a title or annotation smoothly.
- **Task:** Follow multi-line chart text without hesitation between lines.
- **Chart Setting:** The text block contains more than a short label and wraps onto multiple lines.
- **Audience:** Readers are scanning chart text alongside visual elements.
- **Success Criterion:** The next line is easy to find and the text block forms a clean edge.

## Do not use when the text is only a short label <!-- role: exceptions -->

**Break it when:** The text is short enough that readers do not need to find the start of a new line. **Why:** The source's stronger readability warning applies to longer text where line-to-line scanning matters.

## Tradeoffs of left alignment <!-- role: costs -->

**Sacrifice:** You give up centered symmetry.\
**Risk:** Centered text can look balanced at first glance but leaves uneven edges and gaps in multi-line blocks.\
**Mitigation:** Align the left edge of the text block with a nearby chart edge or element.

## Common alignment failure <!-- role: mistakes -->

**Mistake:** Center-align a multi-line title or annotation. **Why it fails:** The text block loses a clear edge, and readers need longer to find where each new line begins.

## Check line starts <!-- role: check -->

**Failure Sign:** The text block has uneven left edges and obvious gaps beside short lines.\
**Quick Check:** Look at any multi-line text block and see whether each line begins at the same x-position.\
**Stronger Test:** Read from the first line to the second line and note whether you hesitate finding the next line start.

## Fix text alignment <!-- role: fix -->

- Switch multi-line titles from centered to left-aligned.
- Switch lengthy annotations from centered to left-aligned.
- Align the text block with a nearby chart edge so its left edge feels deliberate.
- Keep non-left alignment only for short text that does not need multi-line scanning.
