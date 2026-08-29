---
title: "BoKA: Bayesian optimization based knowledge amalgamation for multi-unknown-domain text classification"
authors:
  - "Linzhu Yu"
  - "Huan Li"
  - "Ke Chen"
  - "Lidan Shou"
author_links:
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2024-01-01"
publishDate: "2024-01-01"
publication_types:
  - "paper-conference"
publication: "The 30th ACM SIGKDD Conference on Knowledge Discovery and Data Mining (KDD)"
venue: "The 30th ACM SIGKDD Conference on Knowledge Discovery and Data Mining (KDD)"
publication_kind: "conference"
slug: "paper-c028"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-A"
  - "CORE-A*"
abstract: "With breakthroughs in pretrained language models, a large number of finetuned models specialized in distinct domains have surfaced online. Yet, when faced with a fresh dataset covering multiple (sub)domains, their performance might degrade. Reusing these available finetuned models to train a new model is a more feasible solution than the finetuning method that demands extensive manual labeling. Knowledge Amalgamation (KA) is such a model reusing technique, which derives a new model (termed student model) by amalgamating those trained models (termed teacher models) tailored for distinct domains, bypassing the need for manual labeling. However, when the domains of text samples are unknown, selecting a number of appropriate teacher models (simply called a combination) for reuse becomes complicated. To learn an accurate student model, the classical KA method resorts to manual selections, a process both tedious and inefficient. Our study pioneers the automation of this combination selection process for KA in the fundamental text classification task, an area previously unexplored. In this paper, we introduce BoKA: an automatic knowledge amalgamation framework for identifying a combination that can learn a superior student model without human labor. Through the lens of Bayesian optimization, BoKA iteratively samples a subset of possible combinations for amalgamation instead of manual selections. Furthermore, we introduce a novel KA method tailored for text classification, which guides the student model using both soft and pseudo-hard labels from the teacher models when their predictions are closely aligned; in cases of significant disagreement, it uses randomly generated labels. Experiments on two public multi-domain datasets show that BoKA achieves remarkable efficiency by sampling only up to 5.5% of all potential combinations. Moreover, BoKA is capable of matching or even surpassing leading zero-shot large language models, despite having dozens of times fewer parameters."
keywords:
  - "boka"
  - "bayesian"
  - "optimization"
  - "knowledge"
  - "amalgamation"
  - "multi"
  - "unknown"
  - "domain"
  - "computer science"
  - "domain (mathematical analysis)"
doi: "10.1145/3637528.3671963"
aliases:
  - "/en/publication/dblp-confkdd-yu-00-s-24/"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/conf/kdd/Yu00S24"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
