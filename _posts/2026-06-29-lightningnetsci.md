---
layout: post
title: Dutch Netsci lightning talk
date: 2026-06-24 00:00:00
description: Dutch Netsci lightning talk
thumbnail: /assets/img/posts/fuzzy-lightning-thumbnail.png
chart:
  plotly: false
---

Explain your research in three minutes — that was the challenge for the lightning talks at the [Dutch Netsci conference in Leiden](https://www.netsci.nl/summer-symposium-2026/). What better way to do it than with a fuzzy mascot! My sister-in-law, Jaimy van Kessel ([Linkedin](https://www.linkedin.com/in/jaimy-van-kessel-48894439a/)), designed the mascot for my slides (she is also designing my PhD thesis cover — more on that soon!).

Here is a short version of the talk:

**Motivation:** Sharing pseudonymized network data does not guarantee privacy — people can still be re-identified from their position in the network structure.

**Solution and measure:** One solution is to anonymize the network so that everyone blends in — but first, we need a way to measure anonymity. We use _k_-anonymity: a node is "anonymous" only if at least one other node shares its exact structural signature (e.g., degree and triangle count).

**Key finding:** Strict uniqueness can be misleading — many "unique" nodes are only slightly different from others. Allowing just _10%_ difference in signature values on the Copnet Facebook network (a social network dataset) raises anonymity from _23.7%_ to _96.1%_ of nodes. Across a set of 19 real-world networks, allowing _5%_ difference renders _+64%_ of unique nodes anonymous, on average.

**Takeaway:** This fuzzy tolerance makes full network anonymization far more achievable, while still preserving privacy.

Slides: [PDF](/assets/pdf/slides-talks/2026-dutchnetsci.pdf) \
Paper: [Fuzzy k-anonymity in complex networks](https://doi.org/10.1038/s41598-026-59941-6)

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/posts/fuzzy-lightning-thumbnail.png" title="fuzzy-slide" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
