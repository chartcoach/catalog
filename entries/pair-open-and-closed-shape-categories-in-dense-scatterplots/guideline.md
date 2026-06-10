---
id: pair-open-and-closed-shape-categories-in-dense-scatterplots
title: Pair different open and closed shape categories in dense mixed scatterplots
bibliography: references.bib
description: For numerosity and linear-relationship judgments in dense single-view
  scatterplots, prefer mixing open and closed shape categories in the symbol encoding
  on multi-class plots to improve speed and accuracy and mitigate within-category
  symbol confusion for viewers distinguishing heterogeneous mark sets.
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

## Shape-category pairing <!-- role: advice -->

Pair symbol classes from different open/closed shape categories when two classes must be distinguished inside one dense scatterplot. For example, use one closed shape and one open shape in the same plot, and avoid pairing two closed shapes such as square with triangle or two open shapes such as plus with asterisk when readers must judge numerosity or linear trend.

## Why mixed open and closed pairs separate faster <!-- role: reason -->

Different shapes that share the same open/closed category interfere with each other more than shapes split across the two categories. That interference matters most when readers must separate intermixed marks inside one cluttered view.

**Mechanism:** Cross-category shape pairs are easier to tell apart, so readers spend less time separating the two symbol classes before making a numerosity or trend judgment.

**Evidence:** Across a flanker task, a same/different task, and mixed-symbol scatterplot tasks, responses were slower and less accurate when competing shapes came from the same open/closed category, and single-plot numerosity and linear-relationship judgments were especially impaired by same-category distractors compared with different-category distractors [@burlinsonOpenVsClosed2018].

**Notes:** The paper reports this effect most clearly for dense, heterogeneous single-plot displays.

## Use when classes are intermixed inside one plot <!-- role: context -->

- **User Goal:** Decide which of two symbol classes is more numerous or which one shows the linear relationship.
- **Task:** Separate two categorical classes that occupy the same plotting area.
- **Data:** Two categories are encoded with shape and mixed together in one dense display.
- **Chart Setting:** A single scatterplot contains heterogeneous symbols rather than separate homogeneous plots.
- **Success Criterion:** Readers distinguish the two classes quickly and accurately.

## Do not use when the task or layout removes the interference <!-- role: exceptions -->

- **Break it when:** The classes are shown in separate side-by-side plots or are otherwise not mixed in one cluttered display. **Why:** The paper did not find an open/closed category effect in separate homogeneous displays and states the effect is most important under clutter and heterogeneity.
- **Break it when:** The task is average-value judgment rather than numerosity or linear relationship. **Why:** The single-plot average-value task did not show reliable effects for this shape-category manipulation.

## Tradeoffs of constraining the shape pair <!-- role: costs -->

**Sacrifice:** You give up some freedom in which two shapes can appear together inside one mixed plot.\
**Risk:** Applying this rule to sparse or separate displays may change little.\
**Mitigation:** Prioritize this edit only where two symbol classes are intermixed and visually crowded.

## Common pairing failure <!-- role: mistakes -->

**Mistake:** Use two open shapes or two closed shapes in the same dense mixed plot and expect their individual outlines alone to separate the classes. **Why it fails:** Same-category pairs produced more interference than open-versus-closed pairs.

## How to test the pairing <!-- role: check -->

**Failure Sign:** Readers hesitate or make more errors when the two classes share the same broad shape category.\
**Quick Check:** Compare the same dense scatterplot twice, once with an open-plus-closed pair and once with a same-category pair, and see which version yields faster or more accurate numerosity or trend judgments.\
**Stronger Test:** Run the comparison on the actual cluttered single-plot task rather than on separate plots.

## What to change in the shape pair <!-- role: fix -->

- Replace one symbol in a same-category pair with a symbol from the other open/closed category.
- If two closed shapes are paired in one dense plot, swap one to an open shape.
- If two open shapes are paired in one dense plot, swap one to a closed shape.
- Leave separate homogeneous plots unchanged unless the symbol classes are being mixed into one crowded view.
