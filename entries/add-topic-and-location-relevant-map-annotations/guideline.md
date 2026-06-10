---
id: add-topic-and-location-relevant-map-annotations
title: Add annotations that match both the article topic and the mapped location
bibliography: references.bib
description: For single-result annotated news maps, use topic- and location-matched
  text annotations on mapped locations to maximize contextual explanation and address
  irrelevant annotation content for readers interpreting the map with the article.
labels:
- purpose:refine
- basis:empirical
- scope:single-result
- chart:map
- quality:insight
- lever:text-annotation
- component:annotation:use
- communication:context
---

## Matched text annotations <!-- role: advice -->

Attach annotation text only when it matches both the article topic and the specific mapped location. For example, find candidate articles about the same location and variable, rank them by similarity to the source article, and extract a sentence that mentions the location instead of attaching a random article sentence.

## Why matched annotations help <!-- role: reason -->

Annotations work as context only when readers can connect them to both the marked place and the story they are reading. Topic- and location-matched annotation text makes the callout feel explanatory instead of decorative or distracting.

**Mechanism:** Matching annotation content to the article and the annotated place adds relevant context that is not already in the map or the source article, helping readers understand why a location matters.

**Evidence:** Maps with article-similarity-based annotation content were rated much more relevant than versions that used random annotation articles, and the matched-annotation maps also received higher overall ratings [@gaoNewsViewsAutomatedPipeline2014].

## Use when the map needs explanatory context <!-- role: context -->

- **User Goal:** Understand why specific locations matter or differ.
- **Data:** A mapped location set is available, plus a text corpus that can supply context sentences.
- **Chart Setting:** A thematic map uses callouts or labels attached to locations.
- **Audience:** Readers may have little prior knowledge of the topic or the places shown.
- **Success Criterion:** Readers judge the annotations as relevant to both the article and the mapped details.

## Do not use topical callouts on location-only reference maps <!-- role: exceptions -->

**Break it when:** The display is only a reference map of mentioned places without a matched thematic measure. **Why:** The system uses simple place markers for that case rather than additive topic annotations.

## Costs of richer callouts <!-- role: costs -->

**Sacrifice:** Annotation boxes consume scarce screen space.
**Risk:** Callouts can overlap the map or each other.
**Mitigation:** Limit annotations to the most relevant locations and place them with available screen space in mind.

## Common annotation failure <!-- role: mistakes -->

**Mistake:** Pulling annotation text from unrelated articles or from sentences that do not mention the mapped location. **Why it fails:** The annotation stops feeling connected to the map and lowers perceived relevance.

## Check annotation relevance before publishing <!-- role: check -->

**Failure Sign:** An annotation mentions neither the mapped location nor the mapped measure clearly.
**Quick Check:** Verify that each annotation sentence explicitly mentions the target location and comes from a candidate article about the same variable.
**Stronger Test:** Compare the current annotations with a random-article annotation variant and ask reviewers which version feels more relevant.

## Fix weak annotation content <!-- role: fix -->

- Filter candidate context articles to those that mention both the target location and the mapped variable.
- Rerank those articles by similarity to the source article before selecting annotation content.
- Choose a sentence that mentions the location and has the strongest topical match.
- Remove or replace any annotation that cannot satisfy both the topic and location match.
