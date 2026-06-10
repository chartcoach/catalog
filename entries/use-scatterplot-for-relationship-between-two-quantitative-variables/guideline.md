---
id: use-scatterplot-for-relationship-between-two-quantitative-variables
title: Use a Cartesian scatterplot for the relationship between two quantitative variables
bibliography: references.bib
description: For showing the relationship between paired quantitative values, use
  a Cartesian scatterplot on paired-value data to maximize insight and mitigate relationship-hiding
  paired-bar displays for readers looking for form and nonlinearity.
labels:
- purpose:select
- basis:empirical
- task:relate
- chart:scatter:use
- chart:bar:avoid
- data:quantitative
- quality:insight
- lever:chart-family
---

## Scatterplot choice <!-- role: advice -->

Use a Cartesian scatterplot when the point of the display is the relationship between two quantitative variables. For example, plot each x,y pair as a point so readers can see slope and nonlinearity, instead of showing the same pairs as adjacent bars.

## Why the scatterplot works <!-- role: reason -->

A scatterplot makes the relationship visible through the directions of line segments that readers can imagine between neighboring points. Paired bars preserve separate magnitudes but remove that slope cue, so the pattern in the relationship is hard to see.

**Mechanism:** Position on two axes lets readers perceive changes in direction from point to point. Those perceived slopes reveal whether the relation is linear or bends across the range.

**Evidence:** The paper shows the same paired values as a Cartesian graph and as paired bars; the scatterplot makes the nonlinear relation visible because readers can judge direction between neighboring points, while the paired bars remove that cue [@clevelandGraphicalPerceptionTheory1984].

## Use when the chart's job is the relationship <!-- role: context -->

- **User Goal:** Understand how one quantitative variable changes with another.
- **Task:** See overall form, slope changes, or nonlinearity.
- **Data:** Paired quantitative values.
- **Chart Setting:** You are choosing between a scatterplot and a bar-based display of the same pairs.
- **Audience:** Readers looking for pattern rather than isolated one-dimensional values.
- **Success Criterion:** The relationship becomes visible without mental reconstruction.

## Do not use when separate values are the only target <!-- role: exceptions -->

**Break it when:** The reader's job is to read the x and y values separately rather than to understand their relationship. **Why:** The source's advantage for the Cartesian graph comes specifically from relationship judgments via slope.

## Tradeoffs of using the scatterplot <!-- role: costs -->

**Sacrifice:** The display stops treating x and y as separate one-dimensional bars.
**Risk:** A paired-bar design can seem attractive if separate magnitudes are overemphasized, even though it hides the relationship.
**Mitigation:** Keep both axes explicit so the separate x and y values remain readable from position.

## Common failure with paired values <!-- role: mistakes -->

**Mistake:** Turn each x,y pair into adjacent bars. **Why it fails:** That removes the slope judgments that make the relationship visible.

## Check whether the relationship is visible <!-- role: check -->

**Failure Sign:** Readers can read individual values but cannot tell whether the relationship bends or where it steepens.
**Quick Check:** Show the same data as a scatterplot and as paired bars, then ask where the relation rises faster or departs from a straight pattern.
**Stronger Test:** If only the scatterplot makes the nonlinear pattern clear without mental reconstruction, use the scatterplot.

## Fix the display <!-- role: fix -->

- Replace each pair of bars with one point at the corresponding x and y positions.
- Keep both axes readable so separate coordinate values are still available.
- Inspect the resulting point pattern for the slope changes that the paired bars hid.
