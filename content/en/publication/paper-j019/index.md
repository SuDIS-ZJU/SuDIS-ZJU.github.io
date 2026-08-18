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
date: "2025-01-01"
publishDate: "2025-01-01"
publication_types:
  - "paper-journal"
publication: "IEEE Transactions on Computer-Aided Design of Integrated Circuits and Systems (TCAD)"
slug: "paper-j019"
abstract: "Deep neural network (DNN) models are crucial for WiFi gateway Internet-of-Things (IoT) applications. In a multi-access edge Edge (Raspberry PI 4 Model B) computing (MEC) system, IoT devices dispatch their requests Text form factor: about 4000 to a nearby edge server to accelerate DNN inference. Recently, classification power consumption: 6.4 W processing-in-memory (PIM) accelerators have emerged for DNN GPU Object (Nvidia GEFORCE GTX 1080) inference due to their power and area efficiency. However, current detection form factor: about 3x104 scheduling methods primarily focus on single-DNN workloads power consumption: 180 W and do not fully utilize PIM’s potential for managing multi- Speech recognition PIM (NeuroSIM Model) DNN workloads in MEC scenarios. Additionally, PIM acceler- form factor: 100 ators face challenges such as inflexible resource allocation and IoT Devices Multi-access Edge Server power consumption: 1W costly write operations, constraining the direct application of GPU scheduling techniques. In this paper, we define the multi- Fig. 1. Streaming multi-DNN inference on an edge server [1], [50]. DNN scheduling problem on the PIM accelerator. To reduce the problem’s complexity, we propose a heuristic optimiza- tion algorithm, called Leader-Follower. Using this algorithm, are not affordable for MEC with tight form factor constraints we present P IM S HARE, a scheduler for the PIM accelerator to process multi-DNN workloads. P IM S HARE schedules multi- and power budget [58], [72]. DNN inference requests to enable both temporal and spatial Recently, processing-in-memory (PIM) accelerators have multiplexing, which can enhance hardware utilization. Compared shown efficiency in embedding neural computation into mem- with baseline scheduling methods, including those adapted from ory devices under similar constraints [15], [31]. In PIM GPU scheduling, P IM S HARE can achieve up to a two-order- accelerators, multiple memory devices form an array struc- of-magnitude improvement in throughput and scale the high throughput to workloads containing 18 DNN models. In addition, ture called “crossbar”, which can conduct a matrix-vector P IM S HARE reduces write operations and processing latency. multiplication (MVM) in a single cycle [45] without heavy on-chip data movement [24], [30]. With the usage of non"
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
  - name: "DOI"
    url: "https://doi.org/10.1109/tcad.2025.3641876"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
