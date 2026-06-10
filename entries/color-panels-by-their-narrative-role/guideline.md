---
id: color-panels-by-their-narrative-role
title: Color panels by their narrative role
bibliography: references.bib
description: For relate tasks in multi-panel charts where measures push an outcome
  in opposite directions, use role-based color on the panels to improve readability
  and mitigate ambiguous panel roles for readers following a deliberate sequence.
labels:
- purpose:refine
- basis:heuristic
- task:relate
- structure:small-multiples
- quality:readability
- lever:encoding
- channel:color-hue:use
- polish:palette
---

## Role-based panel color <!-- role: advice -->

Use color to show which panels play the same role in the story. For example, give the panel that reduces the final outcome one hue and the panels that increase it another hue so readers can see the opposing roles before the concluding panel.

## Why role-based color works <!-- role: reason -->

Color can group panels before readers parse every number. When the hues encode narrative role, readers can quickly separate opposing influences from aligned ones.

**Mechanism:** Shared color makes same-role panels feel related, while contrasting color marks panels that push the outcome in the opposite direction.

**Evidence:** The post says color will clarify the role each panel is playing, and demonstrates one hue for the trend that reduces the outcome and another hue for the trends that increase it [@mintzer_sequential_storytelling_2024].

## Use when panel roles differ within the story <!-- role: context -->

- **User Goal:** Show how related indicators contribute differently to a final outcome.
- **Task:** Help readers see which measures work in opposite directions.
- **Data:** At least one paneled trend reduces the outcome while others increase it.
- **Chart Setting:** A multi-panel chart already being read as a sequence.
- **Audience:** Readers who need help distinguishing panel roles quickly.
- **Success Criterion:** Readers can tell which panels share a role and which do not.

## Do not use when the panels do not have contrasting roles <!-- role: exceptions -->

**Break it when:** The panels do not carry different roles in the story. **Why:** The palette no longer clarifies a distinction that matters.

## Costs of role-based color <!-- role: costs -->

**Sacrifice:** Color is committed to role instead of neutral panel styling.
**Risk:** If same-role panels do not share the same hue, the palette stops clarifying the story.
**Mitigation:** Reserve one hue for the reducing role and another for the increasing role.

## Common color failure <!-- role: mistakes -->

**Mistake:** Coloring each panel decoratively or independently from its role in the outcome. **Why it fails:** The palette does not help readers tell which measures work in opposite directions.

## How to test the palette <!-- role: check -->

**Failure Sign:** Readers can see trend direction but cannot tell which panels support the same story role.
**Quick Check:** Inspect the same-role panels; they should share one hue, while opposite-role panels should not.
**Stronger Test:** Hide the annotations and see whether the palette alone still separates the opposing roles.

## What to change <!-- role: fix -->

- Assign one hue to panels that reduce the outcome.
- Assign a second hue to panels that increase the outcome.
- Recolor panels by role, not just by measure identity.
