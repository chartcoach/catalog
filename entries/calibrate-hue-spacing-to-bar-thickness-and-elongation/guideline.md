---
id: calibrate-hue-spacing-to-bar-thickness-and-elongation
title: Calibrate hue spacing to bar thickness and elongation
bibliography: references.bib
description: For color-difference reading in static charts, use hue spacing calibrated
  to bar thickness and elongation on bar charts to improve fidelity and mitigate overly
  conservative palette choices for viewers reading web-based visualizations.
labels:
- purpose:refine
- basis:empirical
- chart:bar
- quality:fidelity:use
- lever:encoding
- channel:color-hue:use
- aesthetic:color:use
---

## Use bar-aware hue thresholds <!-- role: advice -->

Set hue spacing from bar thickness and elongation instead of from point-sized or square-patch assumptions. For example, allow longer bars of the same thickness to carry tighter color spacing than equally thick points, and if final bar lengths are unknown, use the minimum bar thickness as a conservative baseline and validate the rendered bars afterward.

## Why bars can support tighter hue spacing <!-- role: reason -->

Elongated bars expose more visible colored extent than equally thick point marks, so viewers can distinguish smaller color differences on bars than on points. Using bar thickness and elongation prevents wasting palette range by treating all colored marks like square patches.

**Mechanism:** Color discriminability on bars depends on both thickness and elongation, with longer bars of the same thickness becoming easier to distinguish.

**Evidence:** The knowledge collation records this source as experimental evidence about color-hue encodings on bar marks, and the paper reports that colors on bars are generally more discriminable than on equally thick points and that longer bars of equal thickness further improve discriminability [@zengReviewCollationGraphical2023; @szafirModelingColorDifference2018].

**Notes:** The source also reports that area alone was not the significant driver in the bar results.

## Use when bar geometry is known or bounded <!-- role: context -->

- **User Goal:** Keep differently colored bars distinguishable without wasting available color range.
- **Data:** Color is already assigned to bar marks, and minimum bar thickness is known or can be bounded in advance.
- **Chart Setting:** Static bar charts where bar thickness is fixed and bar length may vary across records.
- **Audience:** Viewers reading the rendered bars on standard web or desktop displays.
- **Success Criterion:** The shortest and narrowest relevant bars still show distinct colors.

## Do not rely on thickness alone for very short bars <!-- role: exceptions -->

**Break it when:** Many important bars are very short. **Why:** The source warns that predictive guidance based only on fixed bar thickness is not robust for very short vertical bars and is better used as post-hoc validation there.

## Tradeoffs of bar-aware hue spacing <!-- role: costs -->

**Sacrifice:** A conservative thickness-based baseline can leave some available color range unused.
**Risk:** One global spacing can still fail at the shortest bars if bar lengths vary widely.
**Mitigation:** Validate the rendered shortest bars and widen spacing when the shortest cases still collapse.

## Common failure with bar colors <!-- role: mistakes -->

**Mistake:** Setting bar color spacing from square swatches, area, or point-based thresholds. **Why it fails:** Bar color discrimination changes with thickness and elongation, so these proxies can either waste palette range or miss failures on short bars.

## Check the shortest and narrowest bars <!-- role: check -->

**Failure Sign:** Colors that should differ merge on the shortest or narrowest bars.
**Quick Check:** Inspect the shortest rendered bars at the minimum bar thickness, not only the longest bars or legend samples.
**Stronger Test:** Compute the threshold from bar thickness and elongation when known, or use thickness conservatively and validate the rendered chart afterward.

## Fix the bar-color spacing <!-- role: fix -->

- Widen the hue spacing for bars that must remain distinct.
- Base the spacing on minimum bar thickness and bar elongation when those values are known.
- If bar lengths are unknown at design time, use the minimum thickness as a conservative baseline and validate the rendered bars post hoc.
- Increase bar thickness if the required hue spacing cannot be achieved within the available palette.
