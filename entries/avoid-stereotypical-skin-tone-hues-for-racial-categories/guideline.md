---
id: avoid-stereotypical-skin-tone-hues-for-racial-categories
title: Avoid stereotypical skin-tone hues for racial categories
bibliography: references.bib
description: For non-temporal comparison of racial, ethnic, or world-region groups,
  avoid stereotypical skin-tone category colors on categorical chart and map palettes
  to prevent disrespectful interpretation and mitigate reinforcement of racial stereotypes
  for readers of people-focused graphics.
labels:
- purpose:refine
- basis:heuristic
- data:categorical
- quality:trust
- lever:encoding
- polish:palette
- aesthetic:color:avoid
- channel:color-hue:avoid
---

## Skin-tone hue avoidance <!-- role: advice -->

Use category hues that do not mimic racialized skin-color stereotypes. For example, do not color categories with black for Black people, white for white people, yellow for Asian people, or similar direct skin-tone stand-ins for world regions.

## Why skin-tone matches are risky <!-- role: reason -->

Category colors communicate meaning before readers process the values. When a palette mirrors racial stereotypes, the chart frames people through essentialized color cues instead of a neutral category encoding.

**Mechanism:** Direct skin-tone matches attach identity groups to stereotype-laden colors and can make represented readers feel reduced to those stereotypes.

**Evidence:** The source explicitly advises avoiding black for Black people, white for white people, yellow for Asian people, and similar stereotypical mappings in charts about race and world regions, and notes that modern examples rightly use colors with little to do with skin tones [@muth_race_ethnicity_colors_2024].

## When to avoid skin-tone matches <!-- role: context -->

- **User Goal:** Show data about race, ethnicity, or world regions without reinforcing bias.
- **Task:** Compare or explain differences between categories.
- **Data:** Categorical groups representing people or regions.
- **Chart Setting:** A chart or map that assigns one color per category.
- **Audience:** Mixed readers, including people represented by the data.
- **Success Criterion:** Readers can distinguish categories without reading any group as a skin-color stereotype.

## When skin-tone avoidance can be bent <!-- role: exceptions -->

**Break it when:** white, gray, or black is used only as a backdrop for the least important background category and the categories of interest are shown in more saturated colors. **Why:** the source treats neutral white, gray, or black as an exception when they support a background role rather than a stereotypical identity mapping.

## Costs of removing skin-tone matches <!-- role: costs -->

**Sacrifice:** You give up instantly familiar color-category pairings.
**Risk:** A replacement hue can still feel loaded if it carries another strong association.
**Mitigation:** If the choice feels borderline, ask coworkers or friends for their opinion.

## Common skin-tone matching mistake <!-- role: mistakes -->

**Mistake:** Keeping a color because it “just feels right” for a racial group or region. **Why it fails:** The chart still encodes people through stereotype rather than through a neutral categorical palette.

## How to check for skin-tone matching <!-- role: check -->

**Failure Sign:** The legend or map key contains direct race- or region-to-skin-tone matches.
**Quick Check:** Scan whether people or regions are colored black, white, yellow, or similar skin-tone hues.
**Stronger Test:** If a neutral white, gray, or black category is acting as background, ask a few coworkers or friends whether the palette still reads as a racial stereotype.

## How to fix skin-tone matching <!-- role: fix -->

- Reassign each group to hues that are not direct skin-tone stand-ins.
- Reserve white, gray, or black for a background role only when that group is least important to the story.
- Replace any “it just feels right” color choice with a deliberate non-stereotypical mapping.
