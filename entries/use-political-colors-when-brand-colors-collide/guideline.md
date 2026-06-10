---
id: use-political-colors-when-brand-colors-collide
title: Use political colors when party brand colors collide
bibliography: references.bib
description: For compare tasks in grouped election-result reporting, prefer political
  color assignments on charts and maps with party categories to improve readability
  and mitigate confusion from overlapping party brand colors for readers following
  election coverage.
labels:
- purpose:refine
- basis:heuristic
- task:compare
- scope:grouped-result
- quality:readability
- lever:encoding
- aesthetic:color:use
- channel:color-hue:use
---

## Political color assignment <!-- role: advice -->

Switch the party-color mapping from brand colors to political colors when official party colors overlap. For example, replace two nearly identical logo reds with the distinct ideological colors already used in election charts and maps, such as red, black, green, yellow, blue, or purple for different parties.

## Why political colors work here <!-- role: reason -->

Political colors can separate party categories when official branding compresses multiple parties into the same hue. That lets readers distinguish parties faster in result graphics that rely on color recognition.

**Mechanism:** A one-party-one-hue mapping works better when each hue is visually distinct, and political colors can create that separation when logo colors cannot.

**Evidence:** The post shows German party logo colors colliding, including two major parties using almost the same red, while election reporting based on political colors converges on a much more distinct party palette across charts and maps [@muth_partycolors_2018].

**Notes:** One party's exact purple or pink treatment varied, but the broader political-color mapping still separated parties more clearly than the logo colors did.

## When to use political colors <!-- role: context -->

- **User Goal:** Show how votes are split across several parties.
- **Task:** Help readers distinguish parties quickly in a comparison view.
- **Data:** Multiple party categories are shown together, and official party colors overlap.
- **Chart Setting:** Election-result charts or maps that need one recurring color per party.
- **Audience:** Readers are expected to recognize parties from color in news coverage.
- **Success Criterion:** Each party has a clearly different hue in the same view.

## When not to use political colors alone <!-- role: exceptions -->

**Break it when:** Political-color conventions in your context still collide because too many parties compete for the same hues or there is no settled convention yet. **Why:** Switching away from brand colors no longer guarantees distinct party coding.

## Costs of switching color logic <!-- role: costs -->

**Sacrifice:** You give up literal fidelity to the party's own branding.
**Risk:** Readers who expect the logo color may need a legend or a short period of adjustment.
**Mitigation:** Follow the established reporting convention in your context and keep the chosen mapping stable.

## Common failure with party-color mapping <!-- role: mistakes -->

**Mistake:** Reusing official logo colors even after two major parties land on almost the same hue. **Why it fails:** The palette preserves branding but does not separate the parties in the comparison.

## How to test the color source <!-- role: check -->

**Failure Sign:** Two parties look nearly the same when their swatches are placed side by side.
**Quick Check:** Line up all assigned party colors and inspect whether any concurrently shown parties share almost the same hue.
**Stronger Test:** Plot the assigned colors on a color wheel and check whether two concurrently shown parties occupy nearly the same region.

## How to fix overlapping brand colors <!-- role: fix -->

- Replace overlapping logo colors with the established ideological colors used in comparable election reporting.
- Recheck the full party set and confirm that each concurrently shown party now has its own hue.
- If one party's conventional shade is unresolved, choose one hue and reuse it across the package.
