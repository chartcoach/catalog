---
id: assign-closed-shapes-to-the-focal-class-in-cluttered-scatterplots
title: Assign a closed shape to the focal class in cluttered scatterplots
bibliography: references.bib
description: For target-focused reading in dense single-view scatterplots, prefer
  closed-shape symbols for the focal category on heterogeneous plots to improve speed
  and accuracy and mitigate missed or delayed target discrimination for viewers tracking
  one class among distractors.
labels:
- purpose:refine
- basis:empirical
- chart:scatter
- data:categorical
- density:dense
- quality:fidelity
- lever:encoding
- channel:shape:use
---

## Focal symbol assignment <!-- role: advice -->

Assign a closed shape to the symbol class readers must pick out or follow in a dense mixed-symbol scatterplot. For example, use a circle, square, or triangle for the target class rather than a plus, x, or asterisk when readers must identify that class amid distractors or read a linear relationship from the same plot.

## Why closed focal shapes are easier to track <!-- role: reason -->

Closed shapes were processed faster and more accurately than open shapes when they served as targets. That advantage carries into cluttered mixed-symbol plots when readers must focus on one class and ignore others.

**Mechanism:** A closed focal shape is selected more efficiently, so readers spend less time resolving which marks belong to the target class before responding.

**Evidence:** In both perceptual tasks, closed targets produced faster and more accurate responses than open targets, and in single-plot linear-relationship judgments closed targets were read more quickly while same-feature distractors created stronger interference than different-feature distractors [@burlinsonOpenVsClosed2018].

**Notes:** The paper reports that distractor category matters too, with same-category distractors interfering more than different-category distractors.

## Use when one class is the visual target <!-- role: context -->

- **User Goal:** Pick out one symbol class quickly or follow one class through a mixed display.
- **Task:** Identify a target category while ignoring distractor symbols, or judge a linear relationship for one class inside a mixed plot.
- **Data:** A focal categorical class appears among other symbol classes in a cluttered display.
- **Chart Setting:** A single scatterplot contains heterogeneous symbols and the reader must attend to one class over the others.
- **Success Criterion:** Faster and more accurate responses to the focal class.

## Do not use when the target is not competing inside clutter <!-- role: exceptions -->

- **Break it when:** Symbols are shown alone in homogeneous side-by-side plots rather than intermixed in one display. **Why:** The study did not find a consistent open-versus-closed response-time advantage in separate-plot displays.
- **Break it when:** The task is average-value judgment rather than target identification or linear relationship. **Why:** The paper did not show reliable target-feature effects there.

## Tradeoffs of prioritizing a closed focal shape <!-- role: costs -->

**Sacrifice:** You constrain which symbol can represent the focal class.\
**Risk:** A closed focal shape can still be hard to read if distractors are also closed.\
**Mitigation:** Pair the closed focal shape with distractors from the open category when possible.

## Common focal-shape failure <!-- role: mistakes -->

**Mistake:** Give the focal class an open shape, or pair a closed focal shape with same-category distractors, in a dense mixed plot. **Why it fails:** Open targets were slower overall, and same-feature distractors especially interfered with closed targets.

## How to test the focal shape choice <!-- role: check -->

**Failure Sign:** Readers are slower or less accurate when picking out the focal class than expected for the same data and density.\
**Quick Check:** Compare otherwise identical dense plots that differ only in whether the focal class uses a closed or open shape.\
**Stronger Test:** Repeat the comparison with same-category and different-category distractors to see whether the focal class still suffers interference.

## What to change in the focal encoding <!-- role: fix -->

- Switch the focal class from an open symbol to a closed symbol.
- If the focal class already uses a closed symbol, move distractor classes to the open category when possible.
- Apply this change first in dense mixed plots where readers must track one class through distractors.
