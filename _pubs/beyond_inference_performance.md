---
title: 'Beyond Inference: Performance Analysis of DNN Server Overheads for Computer Vision'
authors:
  - key: ahmed
  - key: susanne
  - key: deshanand
  - key: mohamed
venue: dac
year: 2024
date: 2024-06-01
teaser: ''
tags:
  - software
materials:
  - name: PDF
    url: https://arxiv.org/pdf/2403.12981.pdf
    type: file-pdf
---
Deep neural network (DNN) inference has become an important part of many data-center workloads. This has prompted focused efforts to design ever-faster deep learning accelerators such as GPUs and TPUs. However, an end-to-end DNN-based vision application contains more than just DNN inference, including input decompression, resizing, sampling, normalization, and data transfer. In this paper, we perform a thorough evaluation of computer vision inference requests performed on a throughput-optimized serving system. We quantify the performance impact of server overheads such as data movement, preprocessing, and message brokers between two DNNs producing outputs at different rates. Our empirical analysis encompasses many computer vision tasks including image classification, segmentation, detection, depth-estimation, and more complex processing pipelines with multiple DNNs. Our results consistently demonstrate that end-to-end application performance can easily be dominated by data processing and data movement functions (up to 56% of end-to-end latency in a medium-sized image, and $\sim$ 80% impact on system throughput in a large image), even though these functions have been conventionally overlooked in deep learning system design. Our work identifies important performance bottlenecks in different application scenarios, achieves 2.25$\times$ better throughput compared to prior work, and paves the way for more holistic deep learning system design.
