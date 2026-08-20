---
title: "Forcing-KV Releases Hybrid KV Cache Compression for Autoregressive Video Diffusion"
date: "2026-05-10"
authors: ["SuDIS-ZJU Team"]
summary: "Forcing-KV combines structural and similarity-based pruning to reduce KV-cache memory in autoregressive video diffusion models."
---

<!--more-->

Forcing-KV studies the heterogeneous roles of attention heads in autoregressive video diffusion models and proposes a hybrid KV-cache compression strategy. Static heads use structured pruning, while dynamic heads use segment-wise similarity pruning.

The public preprint reports over 29 FPS on an NVIDIA H200, about 30% cache-memory reduction, and up to 2.82× speedup at 1080P. Code and demo videos are released with the paper.

### Sources

- [arXiv](https://arxiv.org/abs/2605.09681)
- [GitHub](https://github.com/zju-jiyicheng/Forcing-KV)
- [WeChat 1](https://mp.weixin.qq.com/s/LaLNFStVAaQ49MtJRBk8fQ)
- [WeChat 2](https://mp.weixin.qq.com/s/AemiHYJigbEtswo5Gz0P6Q)
