---
id: show-the-mean-explicitly-when-readers-must-judge-the-mean
title: Show the mean explicitly when readers must judge the mean
bibliography: references.bib
description: For compare tasks on grouped value displays, use explicit mean encoding
  on the chart to improve fidelity and mitigate proxy judgments from raw marks for
  readers interpreting group averages.
labels:
- purpose:refine
- basis:empirical
- task:compare
- scope:grouped-result
- quality:fidelity
- lever:encoding
- operator:difference
---

## Add an explicit mean marker <!-- role: advice -->

Show the mean directly when the chart asks readers to compare group averages instead of making them infer it from multiple raw values. For example, add a visible mean mark or mean value for each group rather than relying on many bar tops, lengths, or areas to imply the average.

## Why an explicit mean helps <!-- role: reason -->

Inferring a mean from several marks forces readers to aggregate visually, and the experiments show that they can substitute simpler proxies instead. A direct mean representation turns the task into reading the intended summary rather than reconstructing it from raw marks.

**Mechanism:** Explicit mean encoding reduces the chance that readers will rely on summed area, total length, or other proxies when answering an average-comparison question.

**Evidence:** Viewers comparing averages from groups of bars often behaved as if they used summed area rather than the true average, and the paper identifies explicit representation of the mean as a direct design implication when the graph requires mean judgments [@yuanPerceptualProxiesExtracting2019].

**Notes:** This recommendation is stated as a design implication from the experiments rather than as a separately tested mean-marker condition.

## Use when the chart's question is about averages <!-- role: context -->

- **User Goal:** Decide which group has the higher mean.
- **Task:** Compare average values across multiple observations.
- **Data:** Quantitative groups with multiple values per group.
- **Chart Setting:** Displays that currently show raw bars or other raw marks without a direct mean readout.
- **Success Criterion:** More accurate reading of which group mean is larger.

## Do not add this when the chart is not about means <!-- role: exceptions -->

**Break it when:** The reader's task is about individual values rather than a group average. **Why:** An explicit mean does not address the main question in a single-value comparison.

## Tradeoffs of explicit mean encoding <!-- role: costs -->

**Sacrifice:** You add a derived summary element to the chart.
**Risk:** The chart now carries both raw values and a summary, which changes the display from raw-only to mixed raw-and-summary reading.
**Mitigation:** Use the mean marker when the intended judgment is explicitly about the average.

## Common mean-judgment mistake <!-- role: mistakes -->

**Mistake:** Leaving the mean implicit in a multi-value comparison and expecting readers to average the raw marks accurately. **Why it fails:** Readers may substitute summed area or length for the intended mean.

## How to check whether the mean is explicit enough <!-- role: check -->

**Failure Sign:** Readers must scan several raw marks and mentally average them to answer the chart's main question.
**Quick Check:** Ask whether each group's mean can be read directly from the chart without combining multiple raw values.
**Stronger Test:** Compare the same chart before and after adding an explicit mean representation and see whether the mean judgment becomes easier.

## How to fix implicit mean displays <!-- role: fix -->

- Add one explicit mean representation for each compared group.
- Make the mean a directly readable part of the chart instead of leaving it to visual aggregation.
- When raw bars remain, use the mean representation to answer the average-comparison question directly.
