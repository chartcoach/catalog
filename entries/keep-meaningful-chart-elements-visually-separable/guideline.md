---
id: keep-meaningful-chart-elements-visually-separable
title: Keep meaningful chart elements visually separable
bibliography: references.bib
description: For visual interpretation of charts where adjacent elements touch or
  overlap, use visible separation and unobscured placement on primary marks and text
  to improve accessibility and mitigate merged marks, hidden labels, and obscured
  elements for viewers who must visually distinguish chart content.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:layout-structure
- polish:spacing
---

## Separate marks and text <!-- role: advice -->

Preserve visible separation between primary marks and text. For example, add at least 1px white space between touching stacked-bar segments or pie slices, and reposition overlapping points or labels when they obscure the elements readers must distinguish.

## Why separation improves perception <!-- role: reason -->

When adjacent marks touch or overlap, readers can lose the boundary between one meaningful element and the next. Visible spacing and unobscured text restore figure-ground separation so required chart elements can be perceived as distinct parts.

**Mechanism:** Separating adjacent marks and keeping text clear prevents visually merged elements, so readers can distinguish the content that carries meaning.

**Evidence:** Chartability defines this perceivable check as keeping primary chart elements from being obscured, requiring at least 1px white space between adjacent touching elements, and preventing any text from being obscured or overlapped. The linked distinguishability guidance frames the goal as making foreground content separable, and the linked chart examples show added white space to separate overlapping marks [@elavskyHowAccessibleMy2022; @w3c_understanding_distinguishable; @observablehq_contrast_and].

**Notes:** This guideline is about distinguishability, not only contrast.

## When mark separation matters <!-- role: context -->

- **User Goal:** Distinguish one chart element from another and read all visible text.
- **Data:** Adjacent categories or overlapping marks where separability is required to understand the chart.
- **Chart Setting:** Charts with touching elements or overlap, such as stacked segments, pie slices, overlapping points, or labels placed near marks.
- **Audience:** Viewers who rely on visual discrimination of marks and text.
- **Success Criterion:** Each required element is visibly separate, and no text is covered or unreadable.

## When separation is not required <!-- role: exceptions -->

**Break it when:** The chart does not require readers to discriminate or separate the touching or overlapped elements to understand it. **Why:** The source treats obscuring as a failure only when discriminability or separability is required for understanding.

## Costs of added separation <!-- role: costs -->

**Sacrifice:** Added separation uses space that could otherwise be given to tightly packed marks.
**Risk:** Applying separation indiscriminately can spend room on elements that do not need to be distinguished.
**Mitigation:** Reserve spacing and overlap fixes for primary marks and text whose separation is required to read the chart.

## Common separation failures <!-- role: mistakes -->

- **Mistake:** Let touching segments or slices meet edge to edge with no white space. **Why it fails:** Adjacent elements can merge when readers need to tell them apart.
- **Mistake:** Place text where marks, lines, or other text overlap it. **Why it fails:** Any obscured text becomes unreadable.
- **Mistake:** Layer other chart elements over primary marks. **Why it fails:** The primary chart elements are no longer clearly distinguishable.

## Check mark separation <!-- role: check -->

**Failure Sign:** Adjacent marks visually merge, or text is covered by marks, lines, or other text.
**Quick Check:** Inspect every touching boundary and verify at least 1px white space between adjacent elements such as stacked segments or pie slices, and verify that no text is overlapped.
**Stronger Test:** If understanding the chart requires separating two elements, confirm that each one can be visually distinguished without guessing where one ends and the other begins.

## Fix merged or obscured elements <!-- role: fix -->

- Add at least 1px white space between adjacent elements that touch.
- Reposition or reorder overlapping marks so primary chart elements are not obscured.
- Move text so no mark, line, or other text overlaps it.
- If the current arrangement still merges required elements, change the layout so the needed elements are visually separable.
