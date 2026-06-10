---
id: format-displayed-data-text-for-human-reading
title: Format displayed data text as human-readable values
bibliography: references.bib
description: For accessibility review of chart text, use human-readable value formatting
  on labels, axes, annotations, tables, and legends to improve accessibility and mitigate
  hard-to-parse numeric strings and unfamiliar terms for screen-reader users and readers
  with cognitive accessibility needs.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:text-annotation
- needs:screen-reader
- needs:cognitive
- access:screen-reader:use
- access:plain-language:use
---

## Format displayed data text <!-- role: advice -->

Format displayed chart text into human-readable values before release. For example, shorten a long visual number such as `6500000000` to a readable label such as `6.5b`, and expose the screen-reader version as fully spoken text such as “six point five billion”; apply the same formatting to axes, data labels, annotations, tables, and legends.

## Why human-readable value formatting works <!-- role: reason -->

Raw numeric strings and compressed terms force readers to translate the display before they can understand the data. A paired visual form and screen-reader form reduces that decoding work and makes the same value easier to interpret across visual and nonvisual reading.

**Mechanism:** Human-readable formatting reduces cognitive and functional labor by turning raw strings into values that can be understood directly on sight and parsed comfortably when read aloud.

**Evidence:** Chartability requires all displayed textual information in labels, annotations, axes, tables, and legends to be formatted to a human-readable level and to have versions that screen readers can parse comfortably, including the example of showing `6500000000` visually as `6.5b` and exposing it to screen readers as “six point five billion” [@elavskyHowAccessibleMy2022]. The linked WCAG understanding document supports explaining unusual words, jargon, and acronyms so people with cognitive disabilities and screen-reader users can understand the content [@w3c_understanding_unusual].

**Notes:** This guidance applies to displayed data text broadly, not only to axis labels.

## Use when displayed chart text needs decoding help <!-- role: context -->

- **User Goal:** Read values and terms directly without mentally expanding raw strings.
- **Data:** Large numbers, abbreviations, acronyms, or other hard-to-parse text appear in displayed chart text.
- **Chart Setting:** The chart exposes text in axes, data labels, annotations, tables, legends, alt text, or other screen-reader labels.
- **Audience:** Includes screen-reader users and readers who benefit from more understandable wording.
- **Success Criterion:** The visual text and the screen-reader text can each be understood comfortably without manual translation.

## Do not rely on this when the information is only visual <!-- role: exceptions -->

**Break it when:** the value or term is not exposed as text at all and remains only visual. **Why:** reformatting text cannot help readers or screen readers if the information is missing from labels, annotations, tables, legends, or other text outputs.

## Costs of parallel value formatting <!-- role: costs -->

**Sacrifice:** The visible label may show a shortened form instead of the full raw string.
**Risk:** Visual shorthand and screen-reader wording can drift apart if they are edited separately.
**Mitigation:** Keep the visual abbreviation and the screen-reader expansion aligned to the same underlying value.

## Common text-formatting failures <!-- role: mistakes -->

- **Mistake:** Leaving raw numeric strings or unexplained abbreviations in axis labels, legends, or annotations. **Why it fails:** readers must reformat the text mentally before they can understand the value.
- **Mistake:** Reusing the same compressed visual string in screen-reader labels or alt text. **Why it fails:** the screen-reader version is not the comfortably parsed spoken form this guideline requires.

## Check displayed text and screen-reader text together <!-- role: check -->

**Failure Sign:** Axis labels, data labels, table cells, legends, or annotations contain long digit runs, abbreviations, acronyms, or other strings that are hard to parse directly.
**Quick Check:** Scan each displayed text element and ask whether a reader can understand it without expanding or decoding it mentally.
**Stronger Test:** Inspect the screen-reader label or alt text for a large value and confirm that it expands the visual shorthand into a fully spoken form.

## Fix the formatting of data text <!-- role: fix -->

- Rewrite long numeric strings in visible axes, labels, tables, legends, and annotations into compact human-readable forms.
- Add screen-reader labels or alt text that expand visual shorthand into fully spoken values.
- Replace unexplained acronyms, jargon, or unusual terms with clearer wording, or add an explanation where the term must remain.
- Apply the same formatting rule consistently across all displayed text elements in the chart.
