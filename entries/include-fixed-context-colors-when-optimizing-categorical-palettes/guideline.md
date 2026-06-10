---
id: include-fixed-context-colors-when-optimizing-categorical-palettes
title: Include fixed background and foreground colors when optimizing a categorical
  palette
bibliography: references.bib
description: For categorical encoding in repeated-use views, use palette optimization
  that includes fixed background or foreground colors on the target chart or map context
  to improve readability and mitigate category colors blending into surrounding display
  colors for analysts and designers.
labels:
- purpose:refine
- basis:empirical
- data:categorical
- quality:readability:use
- lever:encoding
- polish:palette
- aesthetic:color:use
---

## Optimize against the actual display colors <!-- role: advice -->

Treat fixed background and foreground colors as part of the palette optimization problem. For example, lock a white canvas, land or ocean fills, or black border and text colors before optimizing category colors, rather than optimizing the category palette in isolation.

## Why display-context colors matter <!-- role: reason -->

Category colors are judged against their surroundings, not in a vacuum. When the surrounding colors are fixed, including them in the optimization pushes category colors away from conflicts with the actual canvas and foreground elements.

**Mechanism:** Fixed context colors change which category colors remain visually distinct on the final view, so conditioning the optimization on those colors improves practical separability.

**Evidence:** The paper shows that optimizing with a fixed white background produces a noticeably different palette from optimization without a background, and its case studies fix background and foreground colors so category colors remain distinguishable in the actual displays; the review includes this work under nominal color-hue knowledge relevant to visualization refinement [@fangCategoricalColormapOptimization2017; @zengReviewCollationGraphical2023].

**Notes:** The paper treats fixed background and foreground colors as a common practical constraint, especially for reused views.

## Use when surrounding colors are stable <!-- role: context -->

- **User Goal:** Make category colors stand apart from the actual canvas and other fixed display colors.
- **Data:** Nominal categories encoded by color.
- **Chart Setting:** The view uses stable surrounding colors such as a white background, map layers, borders, or fixed text color.
- **Audience:** Designers or analysts working with repeated-use views.
- **Success Criterion:** Category colors remain distinguishable from each other and from the fixed surrounding colors.

## Do not use when display context will not stay fixed <!-- role: exceptions -->

**Break it when:** The chart will not keep the same background or foreground colors across use. **Why:** The optimization result is conditioned on those fixed surrounding colors.

## Tradeoffs of context-aware optimization <!-- role: costs -->

**Sacrifice:** You give up some portability across different themes or display contexts.
**Risk:** A palette optimized for one fixed background may work less well when reused on another.
**Mitigation:** Optimize the palette with the actual surrounding colors used in the target view.

## Common failure mode: optimizing the palette alone <!-- role: mistakes -->

**Mistake:** Optimize category colors without including the actual background and foreground colors. **Why it fails:** Colors that look separated on their own can still blend into the real display context.

## Check category colors against the real canvas <!-- role: check -->

**Failure Sign:** One or more category colors disappear into the background or compete with fixed display colors.
**Quick Check:** Review the palette against the real background and fixed foreground colors, not only as isolated swatches.
**Stronger Test:** Compare an isolated optimization with a context-aware optimization and inspect which version keeps more category colors distinct on the final view.

## Fix background conflicts with context-aware palette edits <!-- role: fix -->

- Lock the background color before optimizing the category palette.
- Lock any fixed foreground colors that occupy meaningful visual space, such as borders or labels.
- Re-optimize the category colors with those fixed colors included in the constraint set.
- If the palette must be reused in a different fixed context, optimize a separate version for that context.
