---
id: explain-every-data-carrying-color-with-a-color-key
title: Explain every data-carrying color with a color key
bibliography: references.bib
description: For charts where color encodes values or variables, use explicit color
  keys on the chart to improve readability and mitigate ambiguous color meaning for
  readers.
labels:
- purpose:refine
- basis:heuristic
- quality:readability
- lever:text-annotation
- component:legend:use
- aesthetic:color:use
---

## Color key <!-- role: advice -->

Add a color key whenever color represents data rather than only making marks visible. For example, state what each category hue stands for or show what the low and high ends of a color gradient represent.

## Why color keys are necessary <!-- role: reason -->

A reader cannot decode a color encoding reliably if the chart never states what the colors mean.

**Mechanism:** A color key turns hue or lightness from decoration into an interpretable variable mapping.

**Evidence:** The post says that every visual mark representing a value or variable should be explained and that the same is true for colors, then recommends adding a color key to tell readers what the colors encode [@muth_colors_2018].

## When to add a color key <!-- role: context -->

- **User Goal:** Interpret what a color encoding means.
- **Data:** Color carries category or value information.
- **Chart Setting:** The chart uses multiple hues or a gradient as a data encoding.
- **Success Criterion:** Readers can tell what each data-carrying color means from the chart itself.

## When a color key is unnecessary <!-- role: exceptions -->

**Break it when:** Color only makes marks visible and does not encode a value or variable. **Why:** The rule applies to colors that carry data meaning.

## Tradeoffs of adding a color key <!-- role: costs -->

**Sacrifice:** The chart uses more space for explanatory labeling.
**Risk:** A vague or incomplete key still leaves colors ambiguous.
**Mitigation:** Name every data-carrying hue or gradient endpoint explicitly.

## Common color-key mistake <!-- role: mistakes -->

**Mistake:** Leaving a data-carrying color unexplained. **Why it fails:** Readers cannot know whether the color signals a category, a value range, or nothing important.

## How to check color explanation <!-- role: check -->

**Failure Sign:** At least one plotted color has no stated meaning.
**Quick Check:** Point to each data-carrying color and ask what it encodes.
**Stronger Test:** Verify that both category hues and gradient ranges are explained in the chart.

## How to fix missing color explanation <!-- role: fix -->

- Add a key that maps each category hue to its category.
- Add a key that labels the ends of a value gradient.
- Ensure every color that represents data is named in the chart’s key.
