---
id: provide-24px-pointer-targets-or-an-alternative-interaction-path
title: "Provide 24\xD724 px pointer targets or an alternative interaction path"
bibliography: references.bib
description: For interactive selection and activation, use minimum-size pointer targets
  or an alternative interaction path on charts with small or data-scaled interactive
  marks to improve accessibility and mitigate missed or imprecise selection for people
  with motor impairments or non-precise pointer input.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:interaction-access
- needs:motor
- access:keyboard:use
---

## Pointer target size <!-- role: advice -->

Make each pointer-activated interaction target at least 24×24 px, or add a separate interaction path that reaches the same information and task when the visible mark cannot be enlarged. For example, keep a data-scaled mark visually small if size encodes data, but add a minimum-size text label, an accompanying data table or search control, or a keyboard, zoom, or filter path that lets users select or activate the same item.

## Why larger targets or alternatives matter <!-- role: reason -->

Small pointer targets demand precise motor control. Minimum-size targets or a parallel interaction path let users select, activate, or inspect the same information without depending on fine pointer accuracy.

**Mechanism:** Larger or alternate targets reduce the precision required to hit a mark and make the same represented item reachable through a more tolerant control path.

**Evidence:** Pointer-activated controls should be at least 24×24 px, and when data-scaled marks cannot meet that size the chart should provide another way to select, activate, or interact with the same information or task; supported alternatives include labels, tables, search, keyboard input, zooming, and filtering, while Voronoi-style overlays alone may still leave motor barriers [@elavskyHowAccessibleMy2022; @w3c_understanding_target].

## Use when marks must be selected precisely <!-- role: context -->

- **User Goal:** Select, activate, or otherwise interact with a represented item.
- **Task:** Reach a specific mark or trigger an item-level action.
- **Data:** The chart uses small interactive elements, including marks whose size is mapped to data values.
- **Chart Setting:** Mouse or touch pointer interaction is offered.
- **Audience:** People with motor impairments, people using non-precise touch input, or users who need an alternative to precise pointing.
- **Success Criterion:** The same represented item can be reached and operated without fine pointer precision.

## Do not enlarge the visible mark when size encodes data <!-- role: exceptions -->

**Break it when:** The visible mark size is itself a data encoding and enlarging the mark would change what the chart means. **Why:** Changing the visible mark would distort the encoding, so the repair must be a separate interaction path instead.

## Tradeoffs of larger or alternate targets <!-- role: costs -->

**Sacrifice:** Larger targets or parallel controls take extra interface space or implementation work.\
**Risk:** Hidden target-expansion tricks alone can still leave substantial operability barriers.\
**Mitigation:** Add one visible, discoverable alternative control that reaches the same represented item or task.

## Common target-size failures <!-- role: mistakes -->

- **Mistake:** Keep tiny, data-scaled marks as the only selectable elements. **Why it fails:** Users must hit a very small target to reach the information or action.
- **Mistake:** Rely only on a Voronoi-style overlay to make marks easier to hit. **Why it fails:** The source notes that this can still leave significant operability barriers for people with motor impairments.

## How to review target size <!-- role: check -->

**Failure Sign:** An interactive mark or control is smaller than 24×24 px and no other control reaches the same information or task.\
**Quick Check:** Measure the target area of any pointer-activated element and flag anything under 24×24 px.\
**Stronger Test:** For any tiny or data-scaled mark, verify that the same item can also be selected, activated, or inspected through a non-precise path such as a label, table, search, keyboard path, zoom, or filtering control.

## How to repair small targets <!-- role: fix -->

- Increase the interaction target to at least 24×24 px.
- Add a minimum-size text label that can be selected or activated instead of the tiny mark.
- Add an accompanying data table or search control that reaches the same represented items.
- Add an alternative interaction path such as keyboard navigation, zooming, or filtering when the visible mark cannot be enlarged.
