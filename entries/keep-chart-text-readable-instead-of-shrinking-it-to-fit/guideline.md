---
id: keep-chart-text-readable-instead-of-shrinking-it-to-fit
title: Keep chart text readable instead of shrinking it to fit
bibliography: references.bib
description: For chart text in web visualizations, use readable font settings and
  avoid shrinking or narrowing type to fit to improve readability and mitigate uncomfortable
  reading in tight layouts for readers viewing titles, labels, and annotations.
labels:
- purpose:refine
- basis:heuristic
- quality:readability
- lever:text-annotation
- channel:text:use
---

## Readable font settings <!-- role: advice -->

Use font settings that match comfortable web reading, and do not make text tiny or narrow just because it does not fit. For example, keep important text sans-serif, regular, sentence case, near-black, and above 12px, then shorten sentences, enlarge the chart, or move low-priority text into tooltips or below the visualization when space is tight.

## Why readable text should win over fit <!-- role: reason -->

Readers are already used to a small set of text conventions on the web. When chart text departs from those conventions only to squeeze into the available space, reading becomes less comfortable.

**Mechanism:** Familiar, adequately sized text reduces reading friction, while tiny or narrow text creates avoidable effort before readers can even engage with the data.

**Evidence:** The source identifies easy-to-read web text as sans-serif, regular, sentence case, neither overly narrow nor wide, above 12px, and almost black, and it recommends increasing chart size, shortening sentences, hiding less important text, or using tooltips instead of shrinking text to fit. [@muth_text_in_data_visualizations_2022]

## Use when text competes with tight space <!-- role: context -->

- **User Goal:** Read titles, labels, or annotations comfortably.
- **Task:** Understand chart text without zooming or deciphering cramped typography.
- **Chart Setting:** The visualization is read on the web and available space is limited.
- **Audience:** Readers encounter the text as part of normal on-screen reading.
- **Success Criterion:** Important text remains easy to read at first glance.

## Do not use when unreadable text is the only way to keep everything visible <!-- role: exceptions -->

**Break it when:** The only way to keep every text element in place is to make some of it tiny or narrow. **Why:** The source recommends changing the layout or hiding lower-priority text instead of forcing unreadable type into the chart.

## Tradeoffs of prioritizing readability <!-- role: costs -->

**Sacrifice:** You may have to show less text inside the chart at once.\
**Risk:** If you hide or move the wrong text, readers can lose useful context.\
**Mitigation:** Remove or move the least important annotations first, and keep the most important text readable in place.

## Common typography failure <!-- role: mistakes -->

**Mistake:** Reduce font size or width until the text fits. **Why it fails:** The chart keeps all its words but becomes less comfortable to read.

## Check text legibility <!-- role: check -->

**Failure Sign:** Important text looks unusually tiny, compressed, or faint.\
**Quick Check:** Scan the chart for text that was shrunk to fit instead of rewritten or moved.\
**Stronger Test:** On a small screen, see whether the least important annotations can be hidden or moved below the chart while the main message still holds.

## Fix text fit <!-- role: fix -->

- Increase the overall size of the visualization when possible.
- Shorten sentences instead of compressing the type.
- Move low-priority text into tooltips.
- Hide the least important annotations on mobile or move them below the visualization.
