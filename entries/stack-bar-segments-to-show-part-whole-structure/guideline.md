---
id: stack-bar-segments-to-show-part-whole-structure
title: Stack bar segments to show part-whole structure
bibliography: references.bib
description: For part-whole reading in categorical composition displays, use stacking
  in bar charts to improve readability and mitigate separate-part interpretations
  for readers.
labels:
- purpose:refine
- basis:empirical
- chart:bar
- data:categorical
- operator:part-whole
- quality:readability:use
- lever:layout-structure
---

## Stacking for composition <!-- role: advice -->

Stack bar segments when the message is that several values add up to one whole. For example, use a stacked bar instead of separate bars when the chart must make the part-to-whole relation explicit.

## Why stacking changes the meaning <!-- role: reason -->

Part-whole charts need a part-whole metaphor, not only a precise comparison channel. A stacked bar keeps the total visible and makes each component read as belonging to that total.

**Mechanism:** Stacking embeds each part inside one shared whole, while separate bars frame the same values as independent quantities.

**Evidence:** The paper explicitly contrasts pie charts, stacked bars, and separate bars, arguing that stacked bars and pies express part-to-whole structure while separate bars do not, even though separate bars can be more precise for value comparison [@bertiniWhyShouldntAll2020].

## Use when the whole must stay visible <!-- role: context -->

- **User Goal:** Show that components belong to one total.
- **Task:** Part-whole interpretation rather than only comparison among parts.
- **Data:** Categorical components of a shared whole.
- **Chart Setting:** A bar-based display where you can choose between stacking the parts or separating them.
- **Audience:** Readers who need the composition relationship to be obvious.
- **Success Criterion:** Readers immediately see each segment as part of one total.

## Do not use when exact comparison among parts is primary <!-- role: exceptions -->

**Break it when:** The main job is precise comparison between the parts themselves. **Why:** Separate bars give a more direct comparison frame than stacked segments.

## Costs of stacking the bars <!-- role: costs -->

**Sacrifice:** You give up some comparison precision between individual parts.
**Risk:** Blind stacking can make exact differences between parts harder to judge.
**Mitigation:** Return to separate bars when comparing the parts is more important than expressing the whole.

## Common composition mistake <!-- role: mistakes -->

**Mistake:** Leaving the parts as separate bars when the message is composition. **Why it fails:** The layout removes the part-to-whole metaphor and makes the values look independent.

## Check whether stacking is needed <!-- role: check -->

**Failure Sign:** Reviewers talk about separate values but not about one whole.
**Quick Check:** Show a stacked and separate version of the same parts, then ask which one makes the total obvious at a glance.
**Stronger Test:** Ask a reviewer to explain the relationship among the values; if they do not mention a shared whole, the separate layout is obscuring the message.

## Fix the part-whole structure <!-- role: fix -->

- Combine the separate bars into one stacked total.
- Keep each component inside the shared total so the whole remains visible.
- Remove layouts that isolate the parts when the chart’s message is composition.
