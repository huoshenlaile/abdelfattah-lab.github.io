---
title: 'Quamba2: A Robust and Scalable Post-training Quantization Framework for Selective State Space Models'
authors:
  - key: hungyueh
  - key: chichih
  - key: natalia
  - key: kaichiang
  - key: mohamed
  - key: diana
venue: icml
year: 2025
date: 2025-07-01
teaser: ''
tags:
  - dnn compression
  - llm
  - gpu
  - quantization
materials:
  - name: PDF
    url: https://arxiv.org/pdf/2503.22879
    type: file-pdf
  - name: Code
    url: https://github.com/enyac-group/Quamba
    type: code
---
State Space Models (SSMs) are emerging as a compelling alternative to Transformers because of their consistent memory usage and high performance. Despite this, scaling up SSMs on cloud services or limited-resource devices is challenging due to their storage requirements and computational power. To overcome this, quantizing SSMs with low bit-width data formats can reduce model size and benefit from hardware acceleration. As SSMs are prone to quantization-induced errors, recent efforts have focused on optimizing a particular model or bit-width for efficiency without sacrificing performance. However, distinct bit-width configurations are essential for different scenarios, like W4A8 for boosting large-batch decoding speed, and W4A16 for enhancing generation speed in short prompt applications for a single user. To this end, we present Quamba2, compatible with W8A8, W4A8, and W4A16 for both Mamba1 and Mamba2 backbones, addressing the growing demand for SSM deployment on various platforms. Based on the channel order preserving and activation persistence of SSMs, we propose an offline approach to quantize inputs of a linear recurrence in 8-bit by sorting and clustering for input $x$, combined with a per-state-group quantization for input-dependent parameters $B$ and $C$. To ensure compute-invariance in the SSM output, we rearrange weights offline according to the clustering sequence. The experiments show that Quamba2-8B outperforms two state-of-the-art SSM quantization methods and delivers 1.3$\times$ and 3$\times$ speed-ups in the pre-filling and generation stages, respectively, while offering 4$\times$ memory reduction with only a $1.6\%$ average accuracy drop. The evaluation on MMLU shows the generalizability and robustness of our framework. The code and quantized models will be released at: https://github.com/enyac-group/Quamba.
