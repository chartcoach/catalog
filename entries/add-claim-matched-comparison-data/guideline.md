---
id: add-claim-matched-comparison-data
title: Add comparison data that directly tests the claim
bibliography: references.bib
description: For explanatory comparison tasks, use comparison encodings on charts
  with a focal measure to improve insight and mitigate unsupported claims for readers
  who need the values put in perspective.
labels:
- purpose:refine
- basis:heuristic
- task:compare
- quality:insight:use
- lever:encoding
- measure:multi
- communication:context
---

## Add the comparison that proves the claim <!-- role: advice -->

Add comparison data that directly tests the point the chart is making. For example, compare a focal series with peer series, a competitor, earlier years, a global average, or outliers only when that comparison is the one that answers the chart's claim.

## Why claim-matched comparisons work <!-- role: reason -->

A lone series can show change, but it often cannot show why that change matters. Comparison data supplies the perspective that turns an interesting pattern into a supported point.

**Mechanism:** Matching the comparison to the claim lets readers judge the chart's statement from the marks themselves instead of relying on outside explanation.

**Evidence:** The post says comparison is what puts data into perspective, calls “What should I compare it to?” one of the most crucial questions in data visualization, and shows that the right added data depend on the point the chart is meant to make [@muth_better_charts_2017].

## Use when the chart needs perspective <!-- role: context -->

- **User Goal:** Prove why the focal value or trend is notable.
- **Task:** Compare a focal series against a relevant benchmark or peer.
- **Data:** A focal series already exists, and additional data can be added to test the claim.
- **Chart Setting:** The chart already has a stated point and needs evidence for it.
- **Success Criterion:** Readers can tell from the chart itself what makes the focal series special.

## Do not use irrelevant or unsupported comparisons <!-- role: exceptions -->

**Break it when:** The available comparison answers a different question than the chart's claim, or you cannot find data that actually supports the claim. **Why:** Then the chart stops proving its stated point, and you may need to change the story or go back and choose a different point.

## Tradeoffs of adding comparison data <!-- role: costs -->

**Sacrifice:** The chart becomes less minimal because it includes more data.
**Risk:** Extra series can distract if they serve a different goal than the main claim.
**Mitigation:** Add only the comparison that matches the point you want the chart to prove.

## Common comparison failure <!-- role: mistakes -->

**Mistake:** Leave the focal series alone or add a comparison that belongs to another question. **Why it fails:** The chart either lacks perspective or starts implying a different story than the title promises.

## How to check the comparison <!-- role: check -->

**Failure Sign:** The chart shows values or change, but not why they matter.
**Quick Check:** Ask “Compared with what?” If the chart cannot answer from the marks themselves, the comparison is missing.
**Stronger Test:** Ask a reviewer what makes the focal series special. If they need outside explanation, add or change the comparison data.

## How to fix the comparison <!-- role: fix -->

- Add the benchmark or peer series that directly addresses the chart's claim.
- Remove comparison data that belong to a different goal than the title.
- If no supporting comparison data exist, revise the claim before refining the chart further.
