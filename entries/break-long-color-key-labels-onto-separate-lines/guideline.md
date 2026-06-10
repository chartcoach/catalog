---
id: break-long-color-key-labels-onto-separate-lines
title: Break long color-key labels onto separate lines
bibliography: references.bib
description: For lookup in categorical color keys, use multi-line label formatting
  on legends with labels that cannot be shortened to improve readability and mitigate
  cramped wrapping for readers scanning long category names.
labels:
- purpose:refine
- basis:heuristic
- data:categorical
- quality:readability
- lever:text-annotation
- component:legend:use
- channel:text:use
- density:dense
---

## Multi-line key labels <!-- role: advice -->

Break long color-key labels onto separate lines when you cannot shorten them. For example, put each item on its own line or insert line breaks inside a grid item, then left-align the text, use a legible font, and avoid all-uppercase labels.

## Shorter text chunks are easier to read <!-- role: reason -->

Long legend items are hard to scan when they stay in one dense horizontal run. Breaking them into lines and left-aligning them turns each item into a clearer text block.

**Mechanism:** Multi-line labels reduce horizontal crowding and make long items easier to parse quickly.

**Evidence:** The post recommends first rewriting and shortening long labels, but when that is not possible it recommends putting each item on a separate line or adding line breaks in a grid, then left-aligning the labels and avoiding all-uppercase text because lowercase is easier to read. [@muth_color_keys_2023]

## Use when labels are long and stubborn <!-- role: context -->

- **User Goal:** Read category names in the color key without stumbling over long text.
- **Data:** Categorical labels are too long for a compact one-line treatment.
- **Chart Setting:** The color key must keep the full wording, or shortening is not possible.
- **Audience:** Readers are scanning the key for a specific category.
- **Success Criterion:** Each label is readable at a glance instead of wrapping awkwardly or dominating the key width.

## Do not use when shorter wording solves it first <!-- role: exceptions -->

**Break it when:** The labels are already short or can be rewritten shorter. **Why:** A simpler one-line label is more space-efficient and does not need extra line structure.

## Space tradeoff of line breaks <!-- role: costs -->

**Sacrifice:** You use more vertical space in the key.\
**Risk:** Centered or all-uppercase multi-line labels can stay hard to scan even after adding breaks.\
**Mitigation:** Left-align the text and keep the letterforms legible.

## Common text formatting failure <!-- role: mistakes -->

**Mistake:** Leave long labels in one dense run or style them in all caps. **Why it fails:** The labels remain harder to read and scan quickly.

## Quick review for label readability <!-- role: check -->

**Failure Sign:** Long labels dominate the key width or wrap in awkward places.\
**Quick Check:** Read each label once from left to right; if the text feels cramped or visually jumpy, it needs line structure.\
**Stronger Test:** Compare the current label block against a version with manual line breaks and left alignment.

## Concrete edits for long labels <!-- role: fix -->

- Rewrite and shorten the label text if you can.
- Put each long item on its own line when the key is a list.
- Add manual line breaks inside each grid item when the key is a grid.
- Left-align the label text and avoid all-uppercase styling.
