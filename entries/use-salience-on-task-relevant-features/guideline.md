---
id: use-salience-on-task-relevant-features
title: Make task-relevant features more visually salient than competing elements
bibliography: references.bib
description: For decision tasks with competing visual cues, use salient encoding on
  the task-relevant layer in a visualization to improve fidelity and mitigate missed
  or overweighted information for viewers interpreting complex displays.
labels:
- purpose:refine
- basis:empirical
- quality:fidelity:use
- lever:encoding
- polish:focus
---

## Task-relevant salience <!-- role: advice -->

Increase the visual salience of the feature readers must use for the decision, and reduce the salience of features they should not rely on. For example, make the relevant map layer or isolines more prominent than competing layers, and do not let cone boundaries or foreground icons dominate the display when they are not the quantity readers should judge.

## Why salient emphasis works <!-- role: reason -->

Salience changes what readers notice first. When the display makes a non-diagnostic feature visually dominant, readers often anchor on it, miss less salient but relevant information, or let it bias their judgment.

**Mechanism:** Salient color, edges, and foreground objects pull bottom-up attention with little effort, so the first visually dominant element can steer the whole decision process.

**Evidence:** The review reports that salient display features can either improve decisions when they highlight the right variable or harm decisions when borders, icons, or other foreground elements attract attention away from the real target of the task [@padillaDecisionMakingVisualizations2018].

**Notes:** Salience alone may not improve performance unless readers know how to interpret the highlighted feature.

## Use when salient competition exists <!-- role: context -->

- **User Goal:** Make a decision or inference from a visualization.
- **Task:** Identify or compare one variable while other visible features compete for attention.
- **Data:** Multi-layer, uncertain, or otherwise visually busy information.
- **Chart Setting:** Static 2D displays with strong borders, icons, color regions, or multiple overlaid variables.
- **Audience:** Readers have at least minimal instruction about which feature matters.
- **Success Criterion:** Readers use the intended feature quickly and accurately.

## Do not rely on salience alone <!-- role: exceptions -->

**Break it when:** Readers do not know how to interpret the highlighted feature. **Why:** Salience can redirect fixations without improving the decision if the viewer lacks the needed knowledge to use that feature correctly.

## Costs of strong emphasis <!-- role: costs -->

**Sacrifice:** You give up visual neutrality across layers.
**Risk:** If the wrong feature becomes most salient, readers may become more biased, not less.
**Mitigation:** Pair the visual emphasis with brief instruction about which feature should drive the decision.

## Common salience failure <!-- role: mistakes -->

**Mistake:** Make decorative borders, foreground icons, or visually striking summary outlines more prominent than the underlying data readers must evaluate. **Why it fails:** Readers attend to the dominant feature and let it stand in for the real evidence.

## How to verify attention alignment <!-- role: check -->

**Failure Sign:** Readers describe or point to a boundary, icon, or other prominent object instead of the task-relevant variable.
**Quick Check:** Run a saliency model and see whether the most salient regions overlap the feature readers are supposed to use.
**Stronger Test:** Compare decisions before and after muting the competing element; if judgments change substantially, the original salience was steering the decision.

## How to repair salience problems <!-- role: fix -->

- Increase contrast or prominence on the task-relevant layer.
- Mute or thin visually dominant boundaries, icons, or other competing marks.
- Remove nonessential foreground elements that are easier to notice than the data.
- Add a short instruction that names the exact feature readers should read first.
