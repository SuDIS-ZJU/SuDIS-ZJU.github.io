---
title: "PimShare: Scheduling for multi-DNN inference on processing-in-memory accelerated edge server"
authors:
  - "Xinyu Chen"
  - "Zhongle Xie"
  - "Huan Li"
  - "Ke Chen"
  - "Lidan Shou"
  - "Dawei Jiang"
  - "Gang Chen"
author_links:
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2025-01-01"
publishDate: "2025-01-01"
publication_types:
  - "paper-journal"
publication: "IEEE Transactions on Computer-Aided Design of Integrated Circuits and Systems (TCAD)"
venue: "IEEE Transactions on Computer-Aided Design of Integrated Circuits and Systems (TCAD)"
publication_kind: "journal"
slug: "paper-j019"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-A"
abstract: "Deep neural network (DNN) models are crucial for Internet-of-Things (IoT) applications. In a multi-access edge computing (MEC) system, IoT devices dispatch their requests to a nearby edge server to accelerate DNN inference. Recently, processing-in-memory (PIM) accelerators have emerged for DNN inference due to their power and area efficiency. However, current scheduling methods primarily focus on single-DNN workloads and do not fully utilize PIM’s potential for managing multiDNN workloads in MEC scenarios. Additionally, PIM accelerators face challenges such as inflexible resource allocation and costly write operations, constraining the direct application of GPU scheduling techniques. In this paper, we define the multiDNN scheduling problem on the PIM accelerator. To reduce the problem’s complexity, we propose a heuristic optimization algorithm, called Leader-Follower. Using this algorithm, we present PIMSHARE, a scheduler for the PIM accelerator to process multi-DNN workloads. PIMSHARE schedules multiDNN inference requests to enable both temporal and spatial multiplexing, which can enhance hardware utilization. Compared with baseline scheduling methods, including those adapted from GPU scheduling, PIMSHARE can achieve up to a two-orderof-magnitude improvement in throughput and scale the high throughput to workloads containing 18 DNN models. In addition, PIMSHARE reduces write operations and processing latency."
keywords:
  - "pimshare"
  - "scheduling"
  - "multi"
  - "dnn"
  - "inference"
  - "processing"
  - "memory"
  - "accelerated"
doi: "10.1109/tcad.2025.3641876"
links:
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
