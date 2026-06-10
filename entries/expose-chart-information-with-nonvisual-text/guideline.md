---
id: expose-chart-information-with-nonvisual-text
title: Expose chart information through non-visual text alternatives
bibliography: references.bib
description: For reading charts without visuals in static, interactive, or animated
  displays, use screen-reader-accessible text alternatives on chart content, annotations,
  and narrative elements to maximize accessibility and address information that would
  otherwise be communicated only visually for screen-reader and braille-reader users.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:interaction-access
- needs:screen-reader
- access:screen-reader:use
---

## Expose the non-visual text layer <!-- role: advice -->

Expose every meaningful chart element through screen-reader-readable text instead of leaving the chart as a visual-only graphic. For example, provide non-visual access to each data value, each annotation and visually apparent trend or feature, and each major narrative element, and add synchronized audio descriptions when the chart appears in video, presentation, or animation.

## Why non-visual text exposure works <!-- role: reason -->

Screen readers and braille readers can only present information that exists in exposed text or semantics. If the non-visual layer omits annotations, trends, or narrative takeaways, a reader who cannot use the visual misses part of the chart's meaning.

**Mechanism:** Exposing chart content as text lets assistive technology present both the low-level data and the higher-level features that sighted readers infer from the picture.

**Evidence:** Chartability marks visual-only chart content as a critical failure and requires all chart information, annotations, visually apparent trends or features, and major narrative elements to be available without visuals and tested with screen readers across platforms [@elavskyHowAccessibleMy2022]. WCAG text-alternative guidance and the accessible chart demonstration both describe exposing non-text chart content so it can be read through screen readers or braille instead of relying on the visual presentation alone [@w3c_wcag_quick; @youtube_accessible_chart].

**Notes:** For video, presentation, and animation contexts, the required non-visual access is synchronized audio description.

## Use when chart meaning must survive without sight <!-- role: context -->

- **User Goal:** Understand the chart and its main takeaways without looking at the visual.
- **Task:** Access data values and interpret annotations, trends, features, or narrative points.
- **Chart Setting:** Static charts, interactive charts, videos, presentations, or animations.
- **Audience:** Screen reader users and braille reader users.
- **Success Criterion:** All chart information is available without visuals.

## When text exposure alone is not enough <!-- role: exceptions -->

**Break it when:** The chart is delivered through video, presentation, or animation and the non-visual layer is only unsynchronized text. **Why:** This setting requires synchronized audio descriptions, so text exposure alone does not cover the timed visual content.

## Tradeoffs of full non-visual exposure <!-- role: costs -->

**Sacrifice:** You must author and maintain a non-visual layer for data values, annotations, trends, and narrative elements.\
**Risk:** Providing only partial text exposure can leave the chart technically present but still missing key meaning.\
**Mitigation:** Include both the chart's individual information and the features that are visually apparent in the graphic.

## Common failures in non-visual exposure <!-- role: mistakes -->

- **Mistake:** Exposing the chart only as a generic image or graphic. **Why it fails:** Assistive technology cannot access the chart's data, annotations, or takeaways from a visual-only object.
- **Mistake:** Providing raw data values but omitting annotations, visually apparent trends or features, or major narrative elements. **Why it fails:** The non-visual experience loses meaning that sighted readers get from the visual presentation.

## Check non-visual access with screen readers <!-- role: check -->

**Failure Sign:** A screen reader cannot reach part of the chart, or it misses annotations, trends, features, narrative elements, or timed visual explanation.\
**Quick Check:** Read the chart without looking at it and verify that all meaningful chart information is available through the screen reader.\
**Stronger Test:** At minimum, test with JAWS + Chrome, NVDA + Firefox, VoiceOver + Safari on Mac, and VoiceOver + Safari on iOS, and confirm that videos, presentations, and animations include synchronized audio descriptions.

## Repair visual-only chart content <!-- role: fix -->

- Add exposed text or semantics for each meaningful chart value and element.
- Add non-visual text for annotations, visually apparent trends or features, and major narrative elements.
- Add synchronized audio descriptions when the chart is presented in video, presentation, or animation.
- Retest with the required screen reader and browser combinations until all chart information is available without sight.
