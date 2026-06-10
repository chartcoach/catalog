---
id: lower-opacity-on-lower-priority-categories-when-hues-must-stay-distinct
title: Lower opacity on lower-priority categories when each category needs its own
  hue
bibliography: references.bib
description: For overview comparison in charts with a few distinguishable categories,
  use lower opacity on lower-priority category colors to improve hierarchy and address
  the loss of category identity caused by giving every background mark the same color
  for readers comparing several groups.
labels:
- purpose:refine
- basis:heuristic
- quality:insight
- lever:encoding
- group-cardinality:few
- polish:hierarchy
- aesthetic:color:use
- channel:opacity:use
---

## Fade lower-priority colors without changing their hue <!-- role: advice -->

Keep each category's hue, but reduce opacity on lower-priority categories. For example, leave the key series fully opaque and fade the other series to pastel versions so readers can still tell them apart while seeing which one matters most.

## Why opacity preserves distinction while reducing emphasis <!-- role: reason -->

Using one background color for every secondary category removes category identity. Lowering opacity keeps the original hue visible, so categories remain distinguishable while the main category still pulls the eye first.

**Mechanism:** Opacity reduction lowers visual weight without fully removing hue identity, which lets readers compare several categories while still reading a clear priority order.

**Evidence:** The post presents this approach for charts with just a few categories, explains that making every non-highlighted category the same color makes them harder to distinguish, notes that hover states often reduce the opacity of everything else, and recommends using the same effect in static charts as well [@muth_emphasize_color_2023].

## Use when a few categories must remain distinguishable <!-- role: context -->

- **User Goal:** Emphasize one category while preserving the identity of the other categories.
- **Task:** Compare several categories but guide attention to one or a few of them first.
- **Data:** A small number of categories, each still worth distinguishing from the others.
- **Chart Setting:** A static or interactive chart where all categories already have their own hues.
- **Audience:** Readers need both a clear focus and the ability to compare the remaining categories.
- **Success Criterion:** The key category stands out first, but the faded categories still read as different categories.

## Do not use when the background categories can merge into one group <!-- role: exceptions -->

**Break it when:** You have many categories or do not need readers to distinguish the lower-priority categories from one another. **Why:** This technique is introduced for a few categories and specifically solves the problem that uniform background color removes category distinctions.

## Tradeoffs of opacity-based deemphasis <!-- role: costs -->

**Sacrifice:** Lower-priority categories lose contrast.
**Risk:** If opacity is reduced too far, the faded categories become hard to read.
**Mitigation:** Keep the priority category fully opaque and fade the others only enough to create hierarchy.

## Common failures in opacity-based hierarchy <!-- role: mistakes -->

- **Mistake:** Fading categories until they stop looking distinguishable. **Why it fails:** This method is meant to preserve category identity, not erase it.
- **Mistake:** Leaving every category fully opaque. **Why it fails:** Readers lose the intended order of importance.

## Check whether faded categories still work <!-- role: check -->

**Failure Sign:** Lower-priority categories either compete equally with the highlight or disappear into the background.
**Quick Check:** Confirm that the key category is the strongest, most opaque version while the others still visibly retain their own hues.
**Stronger Test:** If the faded categories all collapse into one indistinct background color, the opacity reduction has gone too far.

## Fix weak or excessive fading <!-- role: fix -->

- Restore each category's original hue before adjusting opacity.
- Reduce opacity on lower-priority categories instead of recoloring them all the same way.
- Keep the highest-priority category fully opaque.
- Increase opacity again if the faded categories no longer remain distinguishable.
