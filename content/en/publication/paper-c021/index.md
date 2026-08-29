---
title: "Data imputation for sparse radio maps in indoor positioning"
authors:
  - "Xiao Li"
  - "Huan Li"
  - "Harry Kai-Ho Chan"
  - "Hua Lu"
  - "Christian S. Jensen"
author_links:
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2023-01-01"
publishDate: "2023-01-01"
publication_types:
  - "paper-conference"
publication: "The 39th IEEE International Conference on Data Engineering (ICDE)"
venue: "The 39th IEEE International Conference on Data Engineering (ICDE)"
publication_kind: "conference"
slug: "paper-c021"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-A"
  - "CORE-A*"
abstract: "Indoor location-based services rely on the availability of sufficiently accurate positioning in indoor spaces. A popular approach to positioning relies on so-called radio maps that contain pairs of a vector of Wi-Fi signal strength indicator values (RSSIs), called a fingerprint, and a location label, called a reference point (RP), in which the fingerprint was observed. The positioning accuracy depends on the quality of the radio maps and their fingerprints. Radio maps are often sparse, with many pairs containing vectors missing many RSSIs as well as RPs. Aiming to improve positioning accuracy, we present a complete set of techniques to impute such missing values in radio maps. We differentiate two types of missing RSSIs: missing not at random (MNAR) and missing at random (MAR). Specifically, we design a framework encompassing a missing RSSI differentiator followed by a data imputer for missing values. The differentiator identifies MARs and MNARs via clustering-based fingerprint analysis. Missing RSSIs and RPs are then imputed jointly by means of a novel encoder-decoder architecture that leverages temporal dependencies in data collection as well as correlations among fingerprints and RPs. A time-lag mechanism is used to consider the aging of data, and a sparsity-friendly attention mechanism is used to focus attention score calculation on observed data. Extensive experiments with real data from two buildings show that our proposal outperforms the alternatives with significant advantages in terms of imputation accuracy and indoor positioning accuracy."
keywords:
  - "data"
  - "imputation"
  - "sparse"
  - "radio"
  - "maps"
  - "indoor"
  - "positioning"
doi: "10.1109/icde55515.2023.00173"
aliases:
  - "/en/publication/dblp-conficde-li-0-c-0-j-23/"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/conf/icde/Li0C0J23"
  - name: "arXiv"
    url: "https://arxiv.org/abs/2302.13022"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
