---
id: use-uppercase-only-for-short-chart-text
title: Use uppercase only for short chart text
bibliography: references.bib
description: For labels and headings in charts, use uppercase only on short text elements
  to improve readability and mitigate dense, hard-to-scan all-caps text for readers
  skimming labels.
labels:
- purpose:refine
- basis:heuristic
- quality:readability
- lever:text-annotation
- polish:hierarchy
---

## Restrict uppercase to short labels <!-- role: advice -->

Use uppercase only on short text elements that must stand apart from surrounding text. For example, apply all caps to a short group label, axis label, table header, tooltip category label, filter control, or map region label, but keep longer explanations in sentence case.

## Why limited uppercase works <!-- role: reason -->

Uppercase removes the word shapes created by mixed upper- and lowercase letters. That makes long text harder to read, even though short uppercase labels can look tidy and distinct.

**Mechanism:** Sentence case preserves recognizable word shapes, while short uppercase labels trade some readability for stronger visual separation and a tidier outline.

**Evidence:** The article says uppercase text is harder to read than sentence case because words lose their distinctive shapes, but also shows it being used effectively for short labels and headlines such as filters, tooltip labels, group labels, axis labels, table headers, and region labels in maps [@muth_fonts_2022].

## When to use limited uppercase <!-- role: context -->

- **User Goal:** Make a short label feel distinct from surrounding text.
- **Chart Setting:** The visualization includes labels, headers, tooltip categories, or map region names.
- **Audience:** Readers are scanning short interface-like text quickly.
- **Success Criterion:** Short labels stand out without reducing overall readability.

## When to break the uppercase rule <!-- role: exceptions -->

**Break it when:** The text is part of a long sentence, note, or explanation. **Why:** Uppercase removes word shapes and makes longer text wider and denser.

## Tradeoffs of limited uppercase <!-- role: costs -->

**Sacrifice:** You give up some uniform all-caps styling across the chart.
**Risk:** Uppercase text becomes wider and denser than sentence case.
**Mitigation:** Limit uppercase to a few short words.

## Common uppercase mistake <!-- role: mistakes -->

**Mistake:** Turning long labels or explanations into all caps. **Why it fails:** The text loses word shapes and takes more space while becoming harder to read.

## How to check uppercase use <!-- role: check -->

**Failure Sign:** Whole phrases or many labels are set in all caps.
**Quick Check:** Convert the text back to sentence case and compare width and density.
**Stronger Test:** Keep uppercase only where the wording stays short and clearly distinct from surrounding text.

## How to fix uppercase use <!-- role: fix -->

- Convert long all-caps text to sentence case.
- Keep uppercase for short labels and headers only.
- Shorten the wording before uppercasing it.
