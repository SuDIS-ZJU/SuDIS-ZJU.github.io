---
title: "Train Small, Infer Large: Memory-efficient LoRA training for large language models"
authors:
  - "Jun Zhang"
  - "Jue Wang"
  - "Huan Li"
  - "Lidan Shou"
  - "Ke Chen"
  - "Yang You"
  - "Guiming Xie"
  - "Xuejian Gong"
  - "and Kunlong Zhou"
author_links:
  - name: "Jun Zhang"
    url: "/authors/jun-zhang/home/"
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2025-01-01"
publishDate: "2025-01-01"
publication_types:
  - "paper-conference"
publication: "The 13th International Conference on Learning Representations (ICLR)"
venue: "The 13th International Conference on Learning Representations (ICLR)"
publication_kind: "conference"
slug: "paper-c056"
design:
  css_class: single-language-section
venue_rankings:
  - "CORE-A*"
abstract: "Large Language Models (LLMs) have significantly advanced natural language processing with exceptional task generalization capabilities. Low-Rank Adaption (LoRA) offers a cost-effective fine-tuning solution, freezing the original model parameters and training only lightweight, low-rank adapter matrices. However, the memory footprint of LoRA is largely dominated by the original model parameters. To mitigate this, we propose LoRAM, a memory-efficient LoRA training scheme founded on the intuition that many neurons in over-parameterized LLMs have low training utility but are essential for inference. LoRAM presents a unique twist: it trains on a pruned (small) model to obtain pruned low-rank matrices, which are then recovered and utilized with the original (large) model for inference. Additionally, minimal-cost continual pre-training, performed by the model publishers in advance, aligns the knowledge discrepancy between pruned and original models. Our extensive experiments demonstrate the efficacy of LoRAM across various pruning strategies and downstream tasks. For a model with 70 billion parameters, LoRAM enables training on a GPU with only 20G HBM, replacing an A100-80G GPU for LoRA training and 15 GPUs for full fine-tuning. Specifically, QLoRAM implemented by structured pruning combined with 4-bit quantization, for LLaMA-3.1-70B (LLaMA-2-70B), reduces the parameter storage cost that dominates the memory usage in low-rank matrix training by 15.81× (16.95×), while achieving dominant performance gains over both the original LLaMA-3.1-70B (LLaMA-2-70B) and LoRA-trained LLaMA-3.1-8B (LLaMA-2-13B). Code is available at https://github.com/junzhang-zj/LoRAM."
keywords:
  - "train"
  - "small"
  - "infer"
  - "large"
  - "memory"
  - "efficient"
  - "lora"
  - "training"
doi: "https://openreview.net/forum?id=s7dkcgprxl"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/conf/iclr/ZhangW0SCYXGZ25"
  - name: "OpenReview"
    url: "https://openreview.net/pdf/cbca92115de2acffddff06a2424cae7b43f898ca.pdf"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
