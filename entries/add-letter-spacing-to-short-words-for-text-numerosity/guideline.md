---
id: add-letter-spacing-to-short-words-for-text-numerosity
title: Add letter spacing to short words when text color is used for count comparison
bibliography: references.bib
description: For count comparison in tagged text displays, use letter spacing on short
  labels in text views to improve fidelity and mitigate word-length bias for readers
  making overview estimates.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:text
- data:text
- quality:fidelity
- lever:encoding
- polish:spacing
---

## Text spacing for count comparison <!-- role: advice -->

Add letter spacing to shorter colored words when readers compare how many tokens belong to each text category. For example, extend short words so their overall colored length is closer to longer words before asking viewers to judge which colored class appears more often.

## Why spacing helps text-based numerosity judgments <!-- role: reason -->

In tagged text, readers can confuse token length with token count.

**Mechanism:** Longer words bias viewers toward perceiving a larger quantity, so increasing the spacing of short words reduces the length imbalance and improves numerosity estimation.

**Evidence:** The paper reports that longer words biased quantity judgments in tagged-text displays and describes a corrective design in which increased spacing between letters in short words improved numerosity estimation [@szafirFourTypesEnsemble2016].

## Use when token length varies across compared categories <!-- role: context -->

- **User Goal:** Compare how many text tokens belong to each highlighted category.
- **Task:** Make a relative numerosity judgment from colored words.
- **Data:** Text tokens vary in length.
- **Chart Setting:** A tagged-text display uses color to identify groups.
- **Success Criterion:** Readers do not overcount the group that happens to have longer words.

## Do not use when count comparison is not a task <!-- role: exceptions -->

**Break it when:** The display is not being used for numerosity comparison across text categories. **Why:** The spacing adjustment specifically addresses count-estimation bias.

## Tradeoffs of added letter spacing <!-- role: costs -->

**Sacrifice:** Short words take more visual space.\
**Risk:** Leaving word length unadjusted biases quantity judgments toward the longer tokens.\
**Mitigation:** Apply the spacing adjustment where the text display is meant to support count comparison.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Leaving short and long colored words at their normal spacing when the reader must compare counts by color. **Why it fails:** Word length then leaks into the quantity judgment.

## Check for word-length count bias <!-- role: check -->

**Failure Sign:** Equal-count groups with longer words seem more numerous than groups with shorter words.\
**Quick Check:** Test a sample with equal numbers of short and long colored words and ask which group appears more frequent.\
**Stronger Test:** Compare count-comparison accuracy before and after adding letter spacing to the shorter words.

## Fix the text encoding <!-- role: fix -->

- Increase the spacing between letters in shorter words.
- Bring the overall colored length of shorter words closer to that of longer words before asking for count comparisons.
- Keep the spacing adjustment on the categories whose frequencies are meant to be compared.
