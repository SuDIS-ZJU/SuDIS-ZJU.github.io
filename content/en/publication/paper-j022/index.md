---
title: "TailorEdit: An Adaptive Framework for Instruction-Guided Fashion Image Editing"
authors:
  - "Xiaoling Gu"
  - "Lingda Zhu"
  - "Yongkang Wong"
  - "Zhou Yu"
  - "Huan Li"
  - "Zizhao Wu"
  - "and Mohan Kankanhalli"
author_links:
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2026-01-01"
publishDate: "2026-01-01"
publication_types:
  - "paper-journal"
publication: "IEEE Transactions on Circuits and Systems for Video Technology (TCSVT)"
venue: "IEEE Transactions on Circuits and Systems for Video Technology (TCSVT)"
publication_kind: "journal"
slug: "paper-j022"
venue_rankings:
  - "CCF-B"
abstract: "Fashion image editing has garnered significant at- I. I NTRODUCTION tention due to its growing demand in e-commerce, social media, and virtual try-on applications. However, existing methods are Due to the rising demand in e-commerce, social media, and typically designed for specific editing tasks in isolation, lacking a virtual try-on applications, fashion image editing has received unified framework capable of handling diverse editing require- widespread attention from both industry and academia [1], ments. This work addresses this limitation from two critical [2]. Existing methodologies primarily fall into three distinct perspectives. First, we construct InstructFashion, a large-scale, categories: image-based editing [3]-[7], text-driven editing [8], high-quality dataset specifically curated for instruction-guided fashion image editing. It is generated through carefully designed [9], and multi-modal conditioned editing [10], [11]. However, pipelines that cover four distinct editing tasks. Second, we these algorithms are typically designed independently for propose TailorEdit, an adaptive framework for instruction-guided specific tasks. This task-specific isolation leads to three key fashion image editing. It integrates human segmentation map- limitations: (1) redundant development efforts across simi- based denoising guidance, modular LoRA-based editing experts, lar editing paradigms, as each new task often requires re- and a dynamic expert routing mechanism to enable precise and semantically coherent modifications. Extensive quantitative and designing dedicated models; (2) inability to leverage shared qualitative evaluations demonstrate that TailorEdit consistently knowledge across tasks, limiting generalization of learned outperforms state-of-the-art methods in terms of realism, co- representations; and (3) increased complexity for end-users herence, and instruction adherence. Our code is available at who must navigate and switch between disparate tools. https://github.com/EndaJude/TailorEdit. In this work, we aim to develop a unified framework for"
keywords:
  - "tailoredit"
  - "adaptive"
  - "framework"
  - "instruction"
  - "guided"
  - "fashion"
  - "image"
  - "editing"
doi: "10.1109/tcsvt.2026.3657731"
links:
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
