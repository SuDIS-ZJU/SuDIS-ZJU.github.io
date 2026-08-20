---
title: "Forcing-KV 开源自回归视频扩散模型的混合 KV 缓存压缩方案"
date: "2026-05-10"
authors: ["SuDIS-ZJU Team"]
summary: "Forcing-KV 结合结构化剪枝与相似度剪枝，降低自回归视频扩散模型的 KV 缓存开销。"
---

<!--more-->

Forcing-KV 研究自回归视频扩散模型中不同注意力头的功能差异，提出混合 KV 缓存压缩策略：对静态头进行结构化剪枝，对动态头进行基于片段相似度的剪枝。

公开预印本报告了 NVIDIA H200 上超过 29 FPS 的生成速度、约 30% 的缓存显存降低，以及 1080P 分辨率下最高 2.82 倍加速；论文同时公开了代码和演示视频。

### 来源

- [arXiv](https://arxiv.org/abs/2605.09681)
- [GitHub](https://github.com/zju-jiyicheng/Forcing-KV)
- [WeChat 1](https://mp.weixin.qq.com/s/LaLNFStVAaQ49MtJRBk8fQ)
- [WeChat 2](https://mp.weixin.qq.com/s/AemiHYJigbEtswo5Gz0P6Q)
