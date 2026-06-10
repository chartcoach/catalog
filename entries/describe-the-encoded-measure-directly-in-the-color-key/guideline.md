---
id: describe-the-encoded-measure-directly-in-the-color-key
title: Describe the encoded measure directly in the color key
bibliography: references.bib
description: For explanatory reading of a color-encoded chart, use direct measure
  labels in the color key to improve readability and mitigate extra abstraction for
  readers interpreting the scale.
labels:
- purpose:refine
- basis:heuristic
- quality:readability
- lever:text-annotation
- component:legend:use
---

## Legend as direct measure <!-- role: advice -->

Name the measured variable in the color key instead of a proxy rating. For example, replace star categories with value ranges and include the unit or threshold that the colors actually encode.

## Why direct legend labels work <!-- role: reason -->

A direct legend lets readers decode the colors in one step. A proxy scale adds a second decoding task before readers can interpret the mapped values.

**Mechanism:** Removing an extra abstraction layer makes the legend match the encoded data more closely, so readers can move from color to meaning without translating through a separate rating system.

**Evidence:** The post recommends cutting the star rating system from the color key and explaining the forecast measure directly there because it is one less layer of abstraction for readers to deal with [@mintzer_fix_my_chart_text_elements_2024].

## Use when the legend currently uses a proxy scale <!-- role: context -->

- **User Goal:** Help readers understand what the color scale means without extra decoding.
- **Data:** Quantitative values are grouped into color ranges.
- **Chart Setting:** The chart uses a color key, and the key currently relies on shorthand or a derived rating system.
- **Success Criterion:** A reader can identify the encoded variable and each range from the color key alone.

## Do not use when the key already states the measure directly <!-- role: exceptions -->

**Break it when:** The color key already names the encoded variable directly rather than through a separate rating system. **Why:** This recommendation targets the added abstraction created by proxy labels.

## Tradeoffs of direct measure labels <!-- role: costs -->

**Sacrifice:** You lose the compactness of a short rating shorthand.\
**Risk:** The legend can become wordy if every bin label is long.\
**Mitigation:** Use concise value ranges that still name the actual measure.

## Common legend failure <!-- role: mistakes -->

**Mistake:** Put proxy categories in the color key and explain the actual variable somewhere else. **Why it fails:** Readers must translate the proxy before they can read the colors.

## Check whether the legend explains the data directly <!-- role: check -->

**Failure Sign:** A reviewer needs the title or footnote to know what the colors encode.\
**Quick Check:** Read the color key alone and ask whether it states the variable and the ranges directly.\
**Stronger Test:** If a reviewer can repeat the rating labels but not the actual measure, the key is still too abstract.

## Fix the color key <!-- role: fix -->

- Replace proxy labels with direct value ranges.
- Add the encoded variable and its unit or threshold to the color key.
- Remove the extra rating system from the legend.
