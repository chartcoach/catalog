---
id: use-pictographic-data-marks-under-memory-load
title: Use pictographic data marks when viewers must remember one chart while reading
  another
bibliography: references.bib
description: For recall tasks with intervening information, use pictographic data
  marks on simple quantitative charts to improve memory fidelity and mitigate interference
  between successive datasets for viewers keeping multiple charts in mind.
labels:
- purpose:refine
- basis:empirical
- task:retrieve
- chart:bar
- quality:fidelity
- lever:encoding
- channel:shape:use
- reading-mode:exact
---

## Data-mark pictographs <!-- role: advice -->

Encode the data marks themselves with pictographs when viewers must hold one chart in memory while seeing another. For example, replace simple geometric marks with object icons that carry the values in successive charts or other multi-step reading situations.

## Why pictographs help under load <!-- role: reason -->

When two datasets compete in memory, richer mark identities help keep them distinct. The shape and identity of the pictograph provide extra cues that simple shapes do not.

**Mechanism:** Pictographic marks expand the memory cue set for each dataset, which reduces interference when viewers must recall one chart after seeing another.

**Evidence:** In the 1-back memory task, charts with pictographic data marks produced less recall error than charts with simple shapes, while the earlier immediate-recall and speeded-reading tasks did not show a strong pictograph advantage [@harozISOTYPEVisualizationWorking2015].

## Use when memory is crowded <!-- role: context -->

- **User Goal:** Recall exact values from one chart after encountering another chart or other intervening information.
- **Task:** Delayed recall with memory load.
- **Data:** Small sets of quantitative category values.
- **Chart Setting:** A simple chart can encode values with pictographic marks or with simple geometric shapes.
- **Audience:** Viewers keeping multiple datasets in mind at once.
- **Success Criterion:** Lower recall error after the intervening material.

## Do not expect the same gain in immediate reading <!-- role: exceptions -->

**Break it when:** Viewers answer immediately from a single just-seen chart or when fast lookup is the only criterion. **Why:** The study found the pictograph benefit when memory was crowded, not in the immediate tasks.

## Tradeoffs of pictographic marks <!-- role: costs -->

**Sacrifice:** You give up some visual simplicity.
**Risk:** The extra detail can add complexity without helping when memory load is low.
**Mitigation:** Reserve pictographic marks for demanding recall situations.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Adding pictographs only as labels or background decoration instead of using them as the data marks. **Why it fails:** The memory benefit came from pictographs embedded in the value encoding.

## How to test it <!-- role: check -->

**Failure Sign:** Viewers confuse the current dataset with the previous one.
**Quick Check:** Run a 1-back style comparison: show chart A, then chart B, and ask for A's values using both pictograph-mark and simple-shape versions.
**Stronger Test:** Compare average absolute recall error after an intervening chart, not just immediate same-screen reading.

## What to change <!-- role: fix -->

- Replace simple geometric marks with pictographic marks that encode the same values.
- Keep the pictographs inside the value marks rather than as separate labels or background images.
- Revert to the simpler mark style if the task changes to immediate lookup instead of delayed recall.
