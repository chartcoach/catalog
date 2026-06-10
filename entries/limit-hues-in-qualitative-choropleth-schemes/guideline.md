---
id: limit-hues-in-qualitative-choropleth-schemes
title: Limit hues in qualitative choropleth schemes
bibliography: references.bib
description: For unordered categorical regions on a choropleth, use as few hues as
  possible in a qualitative color scheme to improve readability and mitigate repeated
  legend lookup for readers decoding categories.
labels:
- purpose:refine
- basis:heuristic
- chart:choropleth
- data:categorical
- quality:readability
- lever:encoding
- channel:color-hue:use
- group-cardinality:few
---

## Qualitative hue count <!-- role: advice -->

Limit the number of hues in a qualitative choropleth so readers can remember what the colors mean. For example, keep the scheme to only a few colors when possible and avoid hue choices that look like a sequential or diverging scale.

## Why fewer category colors are easier to decode <!-- role: reason -->

Category memory gets harder as the number of hues increases.

**Mechanism:** With fewer hues, readers can hold the category-color mapping in memory and return to the legend less often. Avoiding ordered-looking palettes also prevents readers from inferring magnitude where none exists.

**Evidence:** The post says the more colors a map uses, the harder it is to remember what they mean, suggests using only three colors when possible, and warns against palettes that imply sequential or diverging order for unordered data [@muth_choroplethmaps_2018].

## Use when the categories are unordered <!-- role: context -->

- **User Goal:** Distinguish categorical regions without implying order.
- **Task:** Decode category membership from color.
- **Data:** Unordered regional categories.
- **Chart Setting:** A choropleth uses a qualitative color scheme.
- **Audience:** Readers who need to remember a legend while scanning the map.
- **Success Criterion:** Readers can keep the color meanings in mind without repeated legend checks.

## Do not use when the audience already knows the color encoding <!-- role: exceptions -->

**Break it when:** The readers already know the color mapping. **Why:** The post says more than three hues can work when the audience already knows the encoding, such as familiar party colors.

## Costs of keeping the palette small <!-- role: costs -->

**Sacrifice:** You reduce the number of categories you can encode comfortably by color alone.
**Risk:** Too many categories forced into too few hues will become ambiguous.
**Mitigation:** Expand beyond a few hues only when the audience already knows the mapping.

## Common categorical color failure <!-- role: mistakes -->

**Mistake:** Use many hues for a qualitative map or choose hues that look ordered. **Why it fails:** Readers forget the mapping more easily and may read false magnitude into the palette.

## Check whether the hue count is doing too much <!-- role: check -->

**Failure Sign:** The legend must be checked repeatedly to decode the map.
**Quick Check:** Count the distinct hues and ask whether the audience already knows the mapping.
**Stronger Test:** Inspect the palette and remove any hue sequence that suggests low-to-high order for unordered categories.

## Edit the qualitative palette <!-- role: fix -->

- Reduce the number of distinct hues.
- Replace ordered-looking hue sequences with clearly categorical colors.
- Keep extra hues only when the audience already knows the encoding.
- Recheck the legend to confirm each hue still has a distinct category meaning.
