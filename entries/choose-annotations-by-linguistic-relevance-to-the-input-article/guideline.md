---
id: choose-annotations-by-linguistic-relevance-to-the-input-article
title: Choose annotations by linguistic relevance to the input article
bibliography: references.bib
description: For contextual reading over ordered time, use linguistically relevant
  text annotation on stock line charts to improve insight and address off-topic callouts
  for readers seeking background around the current article.
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

## Linguistically relevant annotation selection <!-- role: advice -->

Choose annotations by similarity to the input article when the chart's job is to provide background on the same issue or event. For example, build an input snippet from the article lead and company-mention sentences, compare candidate article snippets against it, and annotate the highest-similarity weeks with a representative article from each week.

## Why linguistically relevant annotation selection works <!-- role: reason -->

Company-related articles are not automatically topic-relevant. Similarity-based selection keeps the annotation set focused on the same thread the reader is already following.

**Mechanism:** Linguistic relevance filters out merely company-related news and surfaces articles that stay closer to the topic and events of the current article.

**Evidence:** In the paper's evaluation, relevance-selected annotations were rated significantly more relevant to the input article than random annotations, and the authors conclude that relevancy analysis produces topically appropriate graphs [@hullmanContextifierAutomaticGeneration2013].

## Where linguistically relevant annotation selection applies <!-- role: context -->

- **User Goal:** See other company information that is relevant to the article currently being read.
- **Data:** A corpus of dated company articles plus the text of the input article.
- **Chart Setting:** Stock line chart annotated with article titles or short summaries.
- **Audience:** Readers doing background research while reading company news.
- **Success Criterion:** The annotations stay on the same issue or event thread as the input article.

## When linguistically relevant annotation selection fails <!-- role: exceptions -->

**Break it when:** The main goal is explaining visible stock moves rather than staying tightly on the article topic. **Why:** Saliency-based selection better optimizes explanation of the line itself.

## Tradeoffs of linguistically relevant annotation selection <!-- role: costs -->

**Sacrifice:** You may give up some alignment with the chart's most visually salient points.\
**Risk:** Highly similar articles can fall on visually ordinary weeks.\
**Mitigation:** Combine linguistic relevance with visual saliency when the chart must do both jobs.

## Common mistakes with linguistically relevant annotation selection <!-- role: mistakes -->

**Mistake:** Selecting any article that mentions the company, regardless of whether it matches the input article's topic. **Why it fails:** The annotation set drifts into company news that does not add useful context for the current story.

## Check whether linguistically relevant annotation selection is working <!-- role: check -->

**Failure Sign:** The annotations are company-related but feel off-topic relative to the input article.\
**Quick Check:** Compare each annotation against the input article's lead sentences and company-mention sentences.\
**Stronger Test:** Generate snippets and similarity scores for candidate articles and verify that selected annotations come from the highest-similarity weeks.

## Fix linguistically relevant annotation selection <!-- role: fix -->

- Build the input query from the first three sentences of the article plus any sentences mentioning the company.
- Remove stop words and company identifiers before computing similarity so company-name repetition does not dominate the ranking.
- Cluster candidate articles by week and rank weeks by their average similarity to the input article.
- Choose a central article from each selected week instead of annotating an arbitrary match.
