---
id: combine-topical-relevance-with-visual-saliency-in-annotation-selection
title: Combine topical relevance with visual saliency in annotation selection
bibliography: references.bib
description: For contextual explanation over ordered time, use combined annotation
  selection on stock line charts to improve insight and address the tradeoff between
  topical relevance and visually grounded callouts for readers using article-linked
  graphics.
labels:
- purpose:refine
- basis:empirical
- time:ordered-time
- chart:line
- lever:text-annotation
- component:annotation:use
- communication:context
- quality:insight
---

## Combined annotation ranking <!-- role: advice -->

Combine topical relevance with visual saliency when one annotated stock chart must both stay on-topic and help explain the plotted history. For example, rank candidate weeks separately by article similarity and by visually salient stock behavior, combine those ranks, and annotate a representative article from the top combined weeks instead of selecting by one feature alone or at random.

## Why combined annotation ranking works <!-- role: reason -->

A context chart often has two jobs at once: stay aligned with the reader's article and comment on important visible moments in the data. A combined ranking keeps either objective from dominating completely.

**Mechanism:** Combined selection places annotations on graphically important periods while preserving a topical connection to the article that triggered the chart.

**Evidence:** The paper reports that the combined system better balances graphical salience and relevance than the baseline, while the evaluation also shows that single-feature versions optimize their own rating dimensions more strongly in isolation [@hullmanContextifierAutomaticGeneration2013].

**Notes:** The authors also included article-volume information in the full system, but they note that its independent contribution needs further investigation.

## Where combined annotation ranking applies <!-- role: context -->

- **User Goal:** Get one chart that is both relevant to the current article and useful for reading the stock history.
- **Data:** Stock time series paired with dated company articles.
- **Chart Setting:** Auto-generated annotated line chart embedded with a news article.
- **Audience:** Readers who need quick context rather than manual searching across many articles.
- **Success Criterion:** The annotations are both on-topic and placed on graphically important periods.

## When combined annotation ranking fails <!-- role: exceptions -->

**Break it when:** The user's need is mainly data-driven explanation or mainly content-driven background. **Why:** The paper suggests weighting saliency higher for data-driven needs and relevance higher for content-driven needs instead of forcing a fixed balance.

## Tradeoffs of combined annotation ranking <!-- role: costs -->

**Sacrifice:** You may not achieve the highest possible score on either relevance alone or saliency alone.\
**Risk:** Fixed feature weights can mismatch the user's immediate goal.\
**Mitigation:** Reweight the combined ranking toward saliency for data-driven needs and toward relevance for content-driven needs.

## Common mistakes with combined annotation ranking <!-- role: mistakes -->

**Mistake:** Optimizing only one feature when the chart must provide both context and visual explanation. **Why it fails:** The result either drifts off-topic or ignores important turns in the series.

## Check whether combined annotation ranking is working <!-- role: check -->

**Failure Sign:** Either salient weeks remain unannotated or annotated weeks feel off-topic relative to the input article.\
**Quick Check:** Inspect each selected annotation for both topical similarity to the input article and proximity to major stock changes.\
**Stronger Test:** Compare the combined output against a relevance-only version and a saliency-only version and confirm that the combined set does not fail either dimension outright.

## Fix combined annotation ranking <!-- role: fix -->

- Rank candidate weeks separately by linguistic relevance and visual saliency before making final selections.
- Combine the separate ranks instead of choosing annotations from only one ranking or at random.
- Select one representative article from each top-ranked combined week.
- Adjust the feature weights toward the user's primary need when the default balance is not appropriate.
