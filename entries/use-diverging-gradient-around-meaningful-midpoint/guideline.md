---
id: use-diverging-gradient-around-meaningful-midpoint
title: Use a diverging color gradient when values split around a meaningful midpoint
bibliography: references.bib
description: For communicating values around a meaningful midpoint, use a diverging
  color gradient on the chosen chart to improve fidelity and mitigate hidden direction
  around the center for readers comparing both sides of the middle.
labels:
- purpose:refine
- basis:heuristic
- data:quantitative
- quality:fidelity
- lever:encoding
- aesthetic:color:use
---

## Center a diverging gradient on the midpoint <!-- role: advice -->

Use a diverging gradient when the color-encoded values move away from a meaningful middle in two directions. For example, center the scale on a bright middle value and use different hues for negative versus positive values, election outcomes on opposite sides, or ordered responses around neutral.

## Why diverging gradients show two-sided values <!-- role: reason -->

Diverging gradients make the midpoint explicit and separate the two directions away from it. Readers can see not just magnitude but which side of the center a value sits on.

**Mechanism:** A bright middle plus two darker arms in different hues signals both distance from the center and direction away from it.

**Evidence:** The article recommends diverging scales for values with a bright middle and darker ends in different hues, with examples including negative and positive values, election results, and Likert scales [@muth_which_color_scale_2021].

## Use when the center matters as much as the extremes <!-- role: context -->

- **User Goal:** Compare values on both sides of a meaningful center.
- **Task:** See direction away from a middle value as well as magnitude.
- **Data:** The color-encoded field extends in two directions from a central value.
- **Chart Setting:** Color is being used to encode ordered value ranges rather than unordered categories.
- **Audience:** Readers who need to tell which side of the midpoint each mark falls on.
- **Success Criterion:** The chart makes the midpoint and both directions away from it visually explicit.

## Do not use when the data only runs from low to high <!-- role: exceptions -->

**Break it when:** The values do not have a meaningful middle value. **Why:** A diverging scale implies a two-sided split that the data does not have.

## Tradeoffs of a diverging gradient <!-- role: costs -->

**Sacrifice:** The midpoint gets special visual treatment.
**Risk:** Using a diverging scale without a real center suggests an artificial divide.
**Mitigation:** Use a sequential gradient when values only run from low to high.

## Common midpoint mistake <!-- role: mistakes -->

**Mistake:** Apply a diverging scale to values such as age or income that simply increase. **Why it fails:** The two-ended palette invents a central split instead of showing one continuous progression.

## Check whether the midpoint is real and visible <!-- role: check -->

**Failure Sign:** The scale uses two hue directions but no clear middle value can be named.
**Quick Check:** Identify the exact value or response that the scale centers on; if you cannot name one, do not use a diverging scale.
**Stronger Test:** Verify that the legend changes direction at a visible center rather than reading as one continuous low-to-high run.

## Fix the midpoint encoding <!-- role: fix -->

- Define the middle value that separates the two directions.
- Use one hue on one side of the middle and a different hue on the other with a bright center.
- Replace the diverging scale with a sequential one if the data does not center on a meaningful midpoint.
