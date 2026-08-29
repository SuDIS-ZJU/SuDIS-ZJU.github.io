---
title: "Leveraging multimodal data and side users for diffusion cross-domain recommendation"
authors:
  - "Fan Zhang"
  - "Jinpeng Chen"
  - "Huan Li"
  - "et al"
author_links:
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2025-01-01"
publishDate: "2025-01-01"
publication_types:
  - "paper-conference"
publication: "The 33th ACM International Conference on Multimedia (MM)"
venue: "The 33th ACM International Conference on Multimedia (MM)"
publication_kind: "conference"
slug: "paper-c045"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-A"
abstract: "Cross-domain recommendation (CDR) aims to address the persistent cold-start problem in Recommender Systems. Current CDR research concentrates on transferring cold-start users' information from the auxiliary domain to the target domain. However, these systems face two main issues: the underutilization of multimodal data, which hinders effective cross-domain alignment, and the neglect of side users who interact solely within the target domain, leading to inadequate learning of the target domain's vector space distribution. To address these issues, we propose a model leveraging Multimodal data and Side users for diffusion Cross-domain recommendation (MuSiC). We first employ a multimodal large language model to extract item multimodal features and leverage a large language model to uncover user features using prompt learning without fine-tuning. Secondly, we propose the cross-domain diffusion module to learn the generation of feature vectors in the target domain. This approach involves learning feature distribution from side users and understanding the patterns in cross-domain transformation through overlapping users. Subsequently, the trained diffusion module is used to generate feature vectors for cold-start users in the target domain, enabling the completion of cross-domain recommendation tasks. Finally, our experimental evaluation of the Amazon dataset confirms that MuSiC achieves state-of-the-art performance, significantly outperforming all selected baselines. Our code is available: https://anonymous.4open.science/r/MuSiC-310A/."
keywords:
  - "leveraging"
  - "multimodal"
  - "data"
  - "side"
  - "users"
  - "diffusion"
  - "cross"
  - "domain"
  - "leverage (statistics)"
  - "recommender system"
doi: "10.1145/3746027.3754555"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/conf/mm/Zhang00W0WHKW25"
  - name: "arXiv"
    url: "https://arxiv.org/abs/2507.04000"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
