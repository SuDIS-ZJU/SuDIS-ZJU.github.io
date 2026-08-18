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
date: "2024-01-01"
publishDate: "2024-01-01"
publication_types:
  - "paper-conference"
publication: "The 62nd Annual Meeting of the Association for Computational Linguistics (ACL)"
slug: "paper-c031"
abstract: "an A100 GPU can take up to 100× longer than a sequence-level forward pass on the same number We present a novel inference scheme, self- of tokens, highlighting the substantial inefficiency speculative decoding, for accelerating Large [cs.CL] 20 May 2024 Language Models (LLMs) without the need for inherent in the current decoding process. an auxiliary model. This approach is charac- Established model compression techniques such terized by a two-stage process: drafting and as quantization (Han et al., 2015), pruning verification. The drafting stage generates draft (Molchanov et al., 2016), and distillation (Hinton tokens at a slightly lower quality but more et al., 2015) have been employed to alleviate these quickly, which is achieved by selectively skip- costs. While these solutions have proven extremely ping certain intermediate layers during draft- ing. Subsequently, the verification stage em- effective, they usually require changing the model ploys the original LLM to validate those draft architecture, changing the training procedure, re- output tokens in one forward pass. This pro- training or fine-tuning the models, and do not main- cess ensures the final output remains identi- tain identical outputs. cal to that produced by the unaltered LLM. In parallel to model compression, speculative Moreover, the proposed method requires no execution is being explored to accelerate the autore- additional neural network training and no extra gressive decoding process (Leviathan et al., 2023; memory footprint, making it a plug-and-play and cost-effective solution for inference accel- Chen et al., 2023). These methods train an auxiliary eration. Benchmarks with LLaMA-2 and its draft model that can quickly generate some draft variants demonstrated a speedup up to 1.99×.1 output tokens. Subsequently, the original LLM, referred to as the verify model, then checks the"
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
  - name: "DOI"
    url: "https://doi.org/10.18653/v1/2024.acl-long.607"
  - name: "DBLP"
    url: "https://dblp.org/rec/conf/acl/Zhang00S0CM24"
  - name: "arXiv"
    url: "https://arxiv.org/abs/2309.08168"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
