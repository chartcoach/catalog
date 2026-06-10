---
id: assign-the-most-important-measure-to-the-most-accurate-channel
title: Assign the most important measure to the most accurate channel
bibliography: references.bib
description: For multi-measure quantitative displays, prefer higher-accuracy encodings
  on the most important measures to improve fidelity and mitigate channel-allocation
  mistakes for viewers reading prioritized information.
labels:
- purpose:refine
- basis:empirical
- data:quantitative
- quality:fidelity:use
- lever:encoding
- channel:position:use
- measure:multi
- reading-mode:exact
---

## Match channel accuracy to measure importance <!-- role: advice -->

Assign the highest-ranked visual channels to the most important measures. For example, in a three-measure display, keep the two more important quantitative measures on x and y position and place the less important measure in area rather than reversing that assignment.

## Why importance should control channel assignment <!-- role: reason -->

When a display cannot give every measure the best channel, the main design choice is which measure gets the most accurate encoding. Putting the most important information on the strongest channel preserves the accuracy of the comparisons readers care about most.

**Mechanism:** Higher-ranked channels such as position support more accurate reading, so giving them to the most important measure improves interpretation where errors matter most.

**Evidence:** The paper extends its perceptual ranking with a principle of importance ordering and contrasts two three-variable scatter plots, preferring the one that assigns position to the more important measures and area to the less important one [@mackinlayAutomatingDesignGraphical1986].

## Use when measures compete for strong channels <!-- role: context -->

- **User Goal:** Preserve the accuracy of the most important quantitative information.
- **Task:** Read several measures from one display when all of them cannot use the best encoding.
- **Data:** Multiple quantitative relations are shown together.
- **Chart Setting:** A chosen display has limited high-accuracy channels, especially x and y position.
- **Success Criterion:** The most important measure is the easiest one to read accurately.

## Do not apply this when there is no channel-allocation conflict <!-- role: exceptions -->

**Break it when:** The display shows only one quantitative measure or there is no competition for the strongest channels. **Why:** Then there is no importance-ordering choice to make.

## Tradeoffs of prioritizing one measure <!-- role: costs -->

**Sacrifice:** Less important measures may move to weaker channels.
**Risk:** A secondary field can become harder to read exactly if it is pushed to area or another lower-ranked channel.
**Mitigation:** Make the importance ordering explicit before assigning channels.

## Common failure mode in multivariate encoding <!-- role: mistakes -->

**Mistake:** Give a less important measure position while a more important measure is left in area. **Why it fails:** The display spends its most accurate channel on secondary information and weakens the primary reading task.

## Check the priority-to-channel match <!-- role: check -->

**Failure Sign:** A secondary measure uses position while the main measure uses a weaker channel.
**Quick Check:** List the measures in importance order, then list the channels in accuracy order and verify that the lists match from top to bottom.
**Stronger Test:** Ask which measure a reader should read most accurately; if it is not on the strongest channel, reassign the encodings.

## Fix the priority mismatch <!-- role: fix -->

- Move the most important quantitative measure onto position.
- Demote the less important quantitative measure to area or another weaker channel.
- Reorder the encoding plan before adding extra measures to the display.
