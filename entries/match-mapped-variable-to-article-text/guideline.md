---
id: match-mapped-variable-to-article-text
title: Match the mapped variable to the article text
bibliography: references.bib
description: For single-result news article accompaniment, use article-to-variable
  text matching on thematic map data selection to maximize contextual relevance and
  address off-topic mapped measures for readers seeking explanatory geographic context.
labels:
- purpose:refine
- basis:empirical
- scope:single-result
- chart:choropleth
- data:geospatial
- quality:insight
- lever:encoding
- communication:context
---

## Mapped variable selection <!-- role: advice -->

Choose the mapped measure by matching article topic phrases to candidate variable labels, then keep only the highest-matching variables. For example, extract noun phrases from the first three sentences, compare them with cleaned variable phrases, and avoid using low-ranked variables once perceived relevance has dropped sharply beyond the top ranks.

## Why text-matched variables work <!-- role: reason -->

A thematic map helps only when its encoded measure is about the same topic as the article. Matching article phrases to variable labels keeps the map aligned with the story instead of attaching any available geographic measure.

**Mechanism:** Text-matched variable selection increases the chance that the mapped values explain the article's stated topic, so readers see relevant geographic context instead of an unrelated distribution.

**Evidence:** Human raters judged top-ranked article-matched variables more relevant than lower-ranked ones, and perceived relevance declined steadily with rank, dropping sharply around rank 30 in the tested set [@gaoNewsViewsAutomatedPipeline2014].

## Use when article-to-map relevance is the main constraint <!-- role: context -->

- **User Goal:** Add a geographic data view that explains the article's main topic.
- **Data:** Many candidate georeferenced measures are available for the same places.
- **Chart Setting:** One thematic map is being chosen to accompany one article.
- **Success Criterion:** Reviewers judge the mapped measure as relevant to the article content.

## Do not force a thematic variable when none matches <!-- role: exceptions -->

**Break it when:** No candidate variable has a strong article match. **Why:** Forcing a thematic measure creates off-topic context; the system uses a reference map in that situation instead of an unrelated thematic map.

## Costs of aggressive relevance filtering <!-- role: costs -->

**Sacrifice:** You give up some broader exploratory variety.
**Risk:** A weakly matched but potentially interesting comparison can be excluded.
**Mitigation:** Keep a short shortlist of the best-matching variables before final selection rather than locking to the first candidate.

## Common variable-selection failure <!-- role: mistakes -->

**Mistake:** Encoding the first available geographic measure or a low-ranked variable. **Why it fails:** Lower-ranked candidates were perceived as less relevant to the article.

## Check the variable-to-article match <!-- role: check -->

**Failure Sign:** The chosen measure appears far down the article-match ranking.
**Quick Check:** Rank candidate variables by article-text match and confirm the chosen measure stays in the top shortlist.
**Stronger Test:** Ask reviewers whether the chosen measure is relevant to the article and compare it with a higher-ranked alternative.

## Fix off-topic mapped measures <!-- role: fix -->

- Extract noun phrases from the first three sentences of the article.
- Rewrite candidate variable labels into comparable descriptive phrases before matching.
- Rerank variables by article-text match and remove low-ranked candidates from the map selection set.
- Replace the thematic map with a reference map if no candidate variable remains relevant enough.
