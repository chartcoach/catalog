---
id: separate-party-hues-when-many-parties-share-a-view
title: Spread party hues apart when many parties appear together
bibliography: references.bib
description: For compare tasks in grouped election-result reporting, use clearly separated
  party hues on charts and maps with many concurrently shown parties to improve readability
  and mitigate confusion from overlapping colors for readers scanning election results.
labels:
- purpose:refine
- basis:heuristic
- task:compare
- group-cardinality:many
- quality:readability
- lever:encoding
- polish:palette
- aesthetic:color:use
---

## Hue spacing <!-- role: advice -->

Spread party hues farther apart when many parties share the same view. For example, do not give two simultaneously shown parties red, and do not let a purple party sit so close to the main red party that the categories blur in an overview chart or map.

## Why hue spacing matters <!-- role: reason -->

With many parties, neighboring hues start to compete for the same visual role. A wider spread makes each party easier to separate at a glance.

**Mechanism:** Large hue separation reduces accidental grouping, while overlapping reds, purple-reds, and yellow-orange hues make party categories harder to tell apart in the same display.

**Evidence:** The post contrasts a relatively clean German party palette with a much more chaotic UK palette, where more parties push colors into overlapping regions on the color wheel and create ambiguity between simultaneously shown parties [@muth_partycolors_2018].

## When to spread hues apart <!-- role: context -->

- **User Goal:** Show many parties in one result view without color confusion.
- **Task:** Support rapid party identification in a multi-party comparison.
- **Data:** Many parties are shown together, including smaller parties that still appear in reporting.
- **Chart Setting:** An election chart or map where multiple party colors are visible at once.
- **Audience:** Readers are scanning an overview rather than reading every label first.
- **Success Criterion:** No two simultaneously shown parties sit in nearly the same hue region.

## When hue collisions matter less <!-- role: exceptions -->

**Break it when:** The overview intentionally leaves out very small parties that would otherwise create color collisions. **Why:** Colors that are not shown together in the same overview do not interfere there.

## Costs of wider hue spacing <!-- role: costs -->

**Sacrifice:** You may move away from exact party or ideological colors.
**Risk:** In very crowded party systems, there may not be enough familiar hues to keep every party far apart.
**Mitigation:** Reserve the widest hue separation for the parties that appear together in the same view.

## Common failure with crowded palettes <!-- role: mistakes -->

**Mistake:** Packing many simultaneously shown parties into neighboring hues. **Why it fails:** Readers see color overlap instead of clean category separation.

## How to test hue separation <!-- role: check -->

**Failure Sign:** Two party colors look adjacent or interchangeable when viewed together.
**Quick Check:** Place all party swatches side by side and inspect whether any pair is too close in hue.
**Stronger Test:** Plot the palette on a color wheel and check whether simultaneously shown parties cluster in the same region.

## How to fix crowded party palettes <!-- role: fix -->

- Move one of each conflicting pair to a more distant unused hue.
- Keep the most distinct hues for the parties that appear together in the same view.
- If distinct hues cannot be maintained in an overview, remove very small parties from that overview and cover them separately.
