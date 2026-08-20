---
title: "Time-VLM: Exploring multimodal vision-language models for augmented time series forecasting"
authors:
  - "Siru Zhong"
  - "Weilin Ruan"
  - "Ming Jin"
  - "Huan Li"
  - "Qingsong Wen"
  - "Yuxuan Liang"
author_links:
  - name: "Huan Li"
    url: "/authors/huan-li/home/zh/"
date: "2025-01-01"
publishDate: "2025-01-01"
publication_types:
  - "paper-conference"
publication: "The 42th International Conference on Machine Learning (ICML)"
venue: "The 42th International Conference on Machine Learning (ICML)"
publication_kind: "conference"
slug: "paper-c055"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-A"
  - "CORE-A*"
abstract: "[cs.CV] 26 May 2025 Recent advancements in time series forecasting CNN Trend max have explored augmenting models with text or Temporal => Textual Projection ResNet vision modalities to improve accuracy. While text Line Graph median provides contextual understanding, it often lacks Vision ViT min Periodicity fine-grained temporal details. Conversely, vision MAE captures intricate temporal patterns but lacks se- Recurrence Plot Late Down Early Up … Steady Short Long Increase Conv mantic context, limiting the complementary po- Net [Context]: These are residential electricity usage patterns. [Dataset]: Electricity consumption peaks on weekday Stationarity tential of these modalities. To address this, we Conv evenings, drops during daytime, and reverses on rest days. NeXt [Statistic]: The input range from <min> to <max>, with a propose Time-VLM, a novel multimodal frame- Grayscale Image median of <median>. The overall trend is <upward>. work that leverages pre-trained Vision-Language ViLT CLIP BLIP GPT-2 GPT-3 T5 Llama BERT Models (VLMs) to bridge temporal, visual, and Vision-Text Text textual modalities for enhanced forecasting. Our framework comprises three key components: Figure 1: Our Time-VLM combines text (Right) and vision (1) a Retrieval-Augmented Learner, which ex- (Left) modalities to augment time series forecasting. tracts enriched temporal features through mem- (Idrees et al., 2019), climate (Karevan & Suykens, 2020), en- ory bank interactions; (2) a Vision-Augmented ergy (Deb et al., 2017), and transportation (Zheng & Huang, Learner, which encodes time series as informa- 2020). Accurate forecasting supports proactive risk mitiga- tive images; and (3) a Text-Augmented Learner, tion, efficient resource allocation, and data-driven decision- which generates contextual textual descriptions. making. Traditional models like ARIMA, while historically These components collaborate with frozen pre- dominant, struggle to capture complex nonlinear patterns. trained VLMs to produce multimodal embed- In contrast, deep learning methods-from recurrent neural dings, which are then fused with temporal fea- networks (RNNs) (Medsker et al., 2001) to Transformer- tures for final prediction. Extensive experiments based architectures (Li et al., 2019; Wu et al., 2021; Zhou demonstrate that Time-VLM achieves superior et al., 2021; Liu et al., 2022a; Zhou et al., 2022; Nie et al., performance, particularly in few-shot and zero- 2023)-leverage innovations such as patch-based feature shot scenarios, thereby establishing a new di- extraction, auto-correlation mechanisms, and frequency de- rection for multimodal time series forecasting. composition to model complex temporal dynamics. Despite Code is available at https://github.com/ their success, these models often fail to generalize across CityMind-Lab/ICML25-TimeVLM. domains or adapt to data-limited scenarios, particularly few- shot and zero-shot settings (Liang et al., 2024). 1."
keywords:
  - "time"
  - "vlm"
  - "exploring"
  - "multimodal"
  - "vision"
  - "language"
  - "models"
  - "augmented"
doi: "https://icml.cc/virtual/2025/poster/44762"
links:
  - name: "arXiv"
    url: "https://arxiv.org/abs/2502.04395"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
