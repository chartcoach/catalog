---
id: use-sans-serif-typefaces-for-most-chart-text
title: Use sans-serif typefaces for most chart text
bibliography: references.bib
description: For skim reading of short labels and numbers in charts and tables, prefer
  sans-serif typefaces on chart text to improve readability and mitigate paragraph-like
  typography for readers scanning web visualizations.
labels:
- purpose:refine
- basis:heuristic
- quality:readability
- lever:text-annotation
- aesthetic:style:use
---

## Use sans-serif chart text <!-- role: advice -->

Set most chart labels, numbers, and other short text in a regular sans-serif typeface. For example, keep axes, table values, and annotations in sans-serif, and use a serif face only for a title when you want a more traditional or branded look.

## Why sans-serif chart text works <!-- role: reason -->

Short chart text is usually scanned, not read in a long reading flow. Sans-serif faces keep labels and numbers cleaner and easier to skim, especially when readers move quickly across values.

**Mechanism:** Sans-serif letterforms reduce ornamental detail, so short labels and numbers are easier to scan than paragraph-oriented serif text.

**Evidence:** The article recommends sans-serif for most visualization text because it looks cleaner and is often easier to skim, especially for numbers, while serif faces are described as better suited to long reading flow and more selectively useful in titles or distinctive designs [@muth_fonts_2022].

**Notes:** Common free options named in the source include Roboto, Lato, Open Sans, Source Sans Pro, and Noto Sans.

## When to use sans-serif chart text <!-- role: context -->

- **User Goal:** Help readers skim labels and numbers quickly.
- **Data:** The display contains many short labels or numeric values.
- **Chart Setting:** A chart or table uses text in labels, ticks, annotations, or notes.
- **Audience:** Readers are scanning a visualization rather than reading long prose.
- **Success Criterion:** The text feels fast to skim and pleasant to look at.

## When to break the sans-serif default <!-- role: exceptions -->

**Break it when:** You want a more classy, traditional, or distinctive tone, or you need the chart title to match surrounding serif typography. **Why:** Serif faces can signal that tone and are most often workable in titles, and sometimes in labels and numbers.

## Tradeoffs of sans-serif chart text <!-- role: costs -->

**Sacrifice:** You give up some literary, traditional, or highly distinctive typographic character.
**Risk:** The visualization may blend in with many other web charts.
**Mitigation:** Keep labels and numbers sans-serif, but use a serif title if you need a stronger publication style.

## Common sans-serif chart text mistake <!-- role: mistakes -->

**Mistake:** Setting most labels and numbers in a serif face when the chart's job is fast scanning. **Why it fails:** Serif faces are better for reading flow in longer text than for skimming short chart text and numbers.

## How to check sans-serif chart text <!-- role: check -->

**Failure Sign:** Labels and values feel more like paragraph text than skimmable chart text.
**Quick Check:** Inspect the main label and number font and confirm whether it is serif or sans-serif.
**Stronger Test:** Compare the same labels and numbers in a sans-serif version and keep the version that is easier to skim.

## How to fix sans-serif chart text <!-- role: fix -->

- Switch labels, numbers, and annotations to a regular sans-serif typeface.
- Keep a serif face only for the title if you need a more traditional or branded look.
- Replace decorative or novelty text styles with a plain sans-serif default.
