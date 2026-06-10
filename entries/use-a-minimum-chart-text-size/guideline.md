---
id: use-a-minimum-chart-text-size
title: Keep chart text at or above 9 pt / 12 px
bibliography: references.bib
description: For chart reading, use text sizing of at least 9 pt / 12 px on chart
  text to improve accessibility and mitigate unreadable small-text failures for readers
  with low vision.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:text-annotation
- needs:low-vision
---

## Minimum text size <!-- role: advice -->

Set every chart text element to at least 9 pt / 12 px. For example, keep only minor text such as axis labels at 9 pt, and make other chart text larger than that minimum.

## Why the minimum matters <!-- role: reason -->

Small chart text is harder to discriminate and read, so labels and other chart text become less accessible, especially for readers with low vision.

**Mechanism:** Raising text to at least the minimum size improves legibility and reduces the chance that readers miss or struggle to read chart text.

**Evidence:** Chartability treats small text as a critical perceivable failure and states that text must not be smaller than 9 pt / 12 px, with only minor text ideally rendered at that minimum [@elavskyHowAccessibleMy2022]. The linked research summary reports that text smaller than about 9 pt significantly reduces readability and reading speed, supporting that threshold for chart labels and annotations [@arditi_rethinking_ada_2017].

**Notes:** The 9 pt / 12 px threshold is a minimum, not a default size for all text.

## Use when chart text must be readable <!-- role: context -->

- **User Goal:** Read chart text directly from the visualization.
- **Chart Setting:** The visualization includes rendered text, and its font size can be set or reviewed.
- **Audience:** Readers include people with low vision.
- **Success Criterion:** No chart text is smaller than 9 pt / 12 px, and only minor text sits at that minimum.

## Do not rely on visual guessing alone <!-- role: exceptions -->

**Break it when:** the rendered font size cannot be determined from design specs, code, or metadata. **Why:** the source says font-size testing is highly complex and difficult without that information, so compliance cannot be verified reliably.

## Costs of enforcing and auditing the minimum <!-- role: costs -->

**Sacrifice:** Font-size review becomes a manual audit task when size is not stored or documented.
**Risk:** Visual spot checks can misjudge whether text actually meets the minimum.
**Mitigation:** Keep font sizes available in design specs, code, or metadata so reviewers can verify them.

## Common small-text mistake <!-- role: mistakes -->

**Mistake:** Using 9 pt / 12 px as the default size for all chart text. **Why it fails:** the source defines that size as the minimum and says only minor text should ideally be rendered at that size.

## How to verify text size <!-- role: check -->

**Failure Sign:** Any chart text is smaller than 9 pt / 12 px.
**Quick Check:** Inspect code, design specs, or metadata for font-size values and flag anything below the minimum.
**Stronger Test:** If size data is missing, confirm the rendered font size with the designer or developer instead of relying only on visual estimation.

## How to repair small text <!-- role: fix -->

- Increase any chart text below 9 pt / 12 px until it meets the minimum.
- Keep only minor text, such as axis labels, at 9 pt / 12 px.
- Increase other chart text beyond the minimum instead of leaving it at 9 pt / 12 px.
- Record font sizes in design specs, code, or metadata so the chart can be audited reliably.
