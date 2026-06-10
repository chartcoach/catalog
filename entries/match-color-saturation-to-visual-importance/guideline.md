---
id: match-color-saturation-to-visual-importance
title: Match color saturation to the party's visual importance
bibliography: references.bib
description: For grouped election-result reporting, use color saturation and lightness
  on party encodings to improve readability and mitigate under- or over-emphasis of
  parties for readers scanning the overall result.
labels:
- purpose:refine
- basis:heuristic
- scope:grouped-result
- quality:readability
- lever:encoding
- polish:hierarchy
- aesthetic:color:use
- channel:color-saturation:use
---

## Saturation for emphasis <!-- role: advice -->

Use color saturation and darkness to match a party's intended visual weight. For example, keep a minor party in a light desaturated hue when it is only a small entry, then move it to a darker more saturated version once it becomes a major focus in the result view.

## Why saturation changes emphasis <!-- role: reason -->

Color does not only identify parties; it also controls which party attracts attention first. Stronger saturation and darker color make a party feel more present in the overview.

**Mechanism:** Saturated and darker colors visually stick out, while lighter and more desaturated colors recede, so color strength can signal whether a party should read as marginal, equal, or especially prominent.

**Evidence:** The post explicitly notes that color is an excellent way to make elements stick out visually and shows one party moving from a light desaturated blue to a much darker and more saturated blue as its importance in election coverage increased, with other newsrooms likewise making it the most saturated party color in the palette [@muth_partycolors_2018].

## When to tune saturation deliberately <!-- role: context -->

- **User Goal:** Control which parties feel minor, equal, or prominent in an election overview.
- **Task:** Use color to set visual hierarchy within a multi-party result display.
- **Data:** Several parties share the view, but they do not all need the same visual weight.
- **Chart Setting:** An overview chart, map, or tracker where color is already assigned by party.
- **Audience:** Readers are scanning for the main political actors in the result.
- **Success Criterion:** Visual prominence matches the intended editorial weight of each party.

## When not to use saturation for hierarchy <!-- role: exceptions -->

**Break it when:** You want all shown parties to carry equal visual weight. **Why:** A more saturated or darker color makes one party stand out more than the others.

## Costs of using saturation for weight <!-- role: costs -->

**Sacrifice:** You give up perfectly equal emphasis across the palette.
**Risk:** Blind use can amplify a party more than intended.
**Mitigation:** Decide the intended visual hierarchy before adjusting saturation or darkness.

## Common failure with color emphasis <!-- role: mistakes -->

**Mistake:** Leaving a newly central party in the palest color or giving the strongest saturation to a party that should not dominate. **Why it fails:** The palette communicates the wrong hierarchy before readers process the numbers.

## How to test visual weight <!-- role: check -->

**Failure Sign:** The party that should matter most does not visually stand out, or a minor party is the strongest color in the view.
**Quick Check:** Compare saturation and darkness across the party swatches and see whether the strongest color matches the intended focal party.
**Stronger Test:** Step back to overview distance and check whether visual prominence matches the hierarchy you intended.

## How to fix mismatched emphasis <!-- role: fix -->

- Darken or saturate the party that should carry more visual weight.
- Lighten or desaturate parties that should recede.
- If equal emphasis is the goal, bring the saturation levels of the major parties closer together.
