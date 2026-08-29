---
title: "Draft & verify: Lossless large language model acceleration via self-speculative decoding"
authors:
  - "Jun Zhang"
  - "Jue Wang"
  - "Huan Li"
  - "Lidan Shou"
  - "Ke Chen"
  - "Gang Chen"
  - "Sharad Mehrotra"
author_links:
  - name: "Jun Zhang"
    url: "/authors/jun-zhang/home/"
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2024-01-01"
publishDate: "2024-01-01"
publication_types:
  - "paper-conference"
publication: "The 62nd Annual Meeting of the Association for Computational Linguistics (ACL)"
venue: "The 62nd Annual Meeting of the Association for Computational Linguistics (ACL)"
publication_kind: "conference"
slug: "paper-c031"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-A"
  - "CORE-A*"
abstract: "We present a novel inference scheme, self-speculative decoding, for accelerating Large Language Models (LLMs) without the need for an auxiliary model. This approach is characterized by a two-stage process: drafting and verification. The drafting stage generates draft tokens at a slightly lower quality but more quickly, which is achieved by selectively skipping certain intermediate layers during drafting. Subsequently, the verification stage employs the original LLM to validate those draft output tokens in one forward pass. This process ensures the final output remains identical to that produced by the unaltered LLM. Moreover, the proposed method requires no additional neural network training and no extra memory footprint, making it a plug-and-play and cost-effective solution for inference acceleration. Benchmarks with LLaMA-2 and its variants demonstrated a speedup up to 1.99$\\times$."
keywords:
  - "draft"
  - "verify"
  - "lossless"
  - "large"
  - "language"
  - "model"
  - "acceleration"
  - "self"
doi: "10.18653/v1/2024.acl-long.607"
aliases:
  - "/en/publication/dblp-confacl-zhang-00-s-0-cm-24/"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/conf/acl/Zhang00S0CM24"
  - name: "arXiv"
    url: "https://arxiv.org/abs/2309.08168"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
