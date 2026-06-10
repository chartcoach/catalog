---
id: use-hues-for-unordered-categories
title: Use hue differences for categories without inherent order
bibliography: references.bib
description: For comparison of unordered categorical values, use hue-based color encoding
  on charts that color categories to improve readability and mitigate false rank cues
  for readers distinguishing group identity.
labels:
- purpose:refine
- basis:heuristic
- data:categorical
- quality:readability
- lever:encoding
- channel:color-hue:use
---

## Hue coding for unordered categories <!-- role: advice -->

Use different hues when color identifies categories that cannot be ranked. For example, encode countries or industries with distinct hues, and do not switch to a light-to-dark ramp unless the labels themselves have an order.

## Why hue works here <!-- role: reason -->

Hue differences tell readers that the colors mark separate identities rather than a low-to-high scale. A lightness ramp invites readers to infer order, so it gives the wrong cue when the labels are peer categories.

**Mechanism:** Hue separates categories without implying magnitude, while light-to-dark encoding suggests a ranked progression.

**Evidence:** The article presents hue-based qualitative scales as the default choice when color-encoded values have no inherent order, using examples such as industries and countries [@muth_quantitative_vs_qualitative_2021].

## Use when categories are peers <!-- role: context -->

- **User Goal:** Distinguish categories quickly.
- **Task:** Compare or identify groups, not rank them by color.
- **Data:** Category labels have no inherent order.
- **Chart Setting:** Color is carrying category identity.
- **Success Criterion:** Readers can tell categories apart without reading dark and light as more and less.

## Do not use when the labels are ordered <!-- role: exceptions -->

**Break it when:** The color-encoded values have an inherent order, including ordered text labels. **Why:** A lightness scale communicates that order more directly.

## What this choice costs <!-- role: costs -->

**Sacrifice:** You give up a low-to-high meaning in the colors.
**Risk:** If order matters, hue differences hide that relation.
**Mitigation:** Switch to an ordered color scale when the labels can truly be ranked.

## Common palette failure <!-- role: mistakes -->

**Mistake:** Use a sequential lightness ramp for unordered categories. **Why it fails:** Readers search for an order that the data do not have.

## How to test the palette choice <!-- role: check -->

**Failure Sign:** Darker categories seem to imply “more” or “higher.”
**Quick Check:** Ask whether every color-encoded label can be placed in a true less-to-more order.
**Stronger Test:** Ask a reviewer what darker versus lighter means; if they invent a ranking, the palette is cueing the wrong structure.

## How to revise it <!-- role: fix -->

- Replace the lightness ramp with clearly different hues.
- Keep light-to-dark encoding only for values with a real order.
- If order becomes the story, remap color to that ordered variable instead of category identity.
